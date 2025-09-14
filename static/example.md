## Slide 1

You can write the entire presentation in Markdown using an external Markdown file.

---

## Slide 2

```hcl [2|1-3]
# calculator Task Resources

resource "aws_cloudwatch_log_group" "calculator" {
  name              = "/ecs/${var.team}-calculator-task"
  retention_in_days = 7
  tags = {
    Name = "${var.team}-calculator-logs"
  }
}

resource "aws_ecs_task_definition" "calculator" {
  family                   = "${var.team}-calculator-task"
  network_mode             = "awsvpc"
  requires_compatibilities = ["FARGATE"]
  cpu                      = var.cpu
  memory                   = var.memory
  execution_role_arn       = aws_iam_role.ecs_execution.arn
  task_role_arn            = aws_iam_role.ecs_task.arn
  container_definitions = jsonencode([
    {
      name  = "${var.team}-calculator"
      image = "860914184352.dkr.ecr.ap-southeast-2.amazonaws.com/bsidesbne-ctf/2025:calculator-latest"
      portMappings = [
        {
          containerPort = 3000
          protocol      = "tcp"
        }
      ]
      environment = [
        {
          name  = "TEAM"
          value = var.team
        }
      ]
      logConfiguration = {
        logDriver = "awslogs"
        options = {
          awslogs-group         = "/ecs/${var.team}-calculator-task"
          awslogs-region        = "ap-southeast-2"
          awslogs-stream-prefix = "ecs"
        }
      }
    }
  ])
  tags = {
    Name = "${var.team}-calculator-task-definition"
  }
}

resource "aws_lb_target_group" "calculator_tg" {
  name        = "${var.team}-calc-tg"
  port        = 3000
  protocol    = "HTTP"
  vpc_id      = var.vpc_id
  target_type = "ip"
  health_check {
    enabled             = true
    healthy_threshold   = 2
    interval            = 60
    matcher             = "200"
    path                = "/"
    port                = "traffic-port"
    protocol            = "HTTP"
    timeout             = 30
    unhealthy_threshold = 3
  }
  tags = {
    Name = "${var.team}-calculator-target-group"
  }
}

resource "aws_ecs_service" "calculator" {
  name            = "${var.team}-calculator-service"
  cluster         = aws_ecs_cluster.team_ecs.id
  task_definition = aws_ecs_task_definition.calculator.arn
  desired_count   = var.desired_count
  launch_type     = "FARGATE"
  
  depends_on = [aws_lb_listener_rule.calculator]
  
  network_configuration {
    subnets          = var.private_subnet_ids
    security_groups  = [aws_security_group.team_ecs.id]
    assign_public_ip = false
  }
  load_balancer {
    target_group_arn = aws_lb_target_group.calculator_tg.arn
    container_name   = "${var.team}-calculator"
    container_port   = 3000
  }
  tags = {
    Name = "${var.team}-calculator-service"
  }
}

resource "aws_lb_listener_rule" "calculator" {
  listener_arn = var.alb_listener_arn
  priority     = 3000 + var.team_index
  action {
    type             = "forward"
    target_group_arn = aws_lb_target_group.calculator_tg.arn
  }
  condition {
    host_header {
      values = ["calculator.${var.team}.ctf.bsidesbne.com"]
    }
  }
  tags = {
    Name = "${var.team}-calculator-rule"
  }
}

resource "aws_route53_record" "calculator" {
  zone_id = var.route53_zone_id
  name    = "calculator.${var.team}.ctf.bsidesbne.com"
  type    = "A"
  alias {
    name                   = var.alb_dns_name
    zone_id                = var.alb_zone_id
    evaluate_target_health = true
  }
} 
```