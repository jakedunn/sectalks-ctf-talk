<script lang="ts">
	import Slide from './slide.svelte'
	import Code from './code.svelte'
	import Markdown from './markdown.svelte'
	import Notes from './notes.svelte'
</script>

<!-- <Markdown name="example.md" external /> -->


<Slide animate>
	<Code id="code" lines="1|3">
		{`
			<Slide animate>
				<!-- .. -->
			</Slide>
		`}
	</Code>
</Slide>

<Slide animate>
	<Code id="code" lines="2|4">
		{`
			<Slide animate>
				<Code lines>
					<!-- ... -->
				</Code>
			</Slide>
		`}
	</Code>
</Slide>

<Slide animate>
	<Code id="code" lines="3-5|1-7">
		{`
			<Slide animate>
				<Code lines>
					{code\`
						...
					\`}
				</Code>
			</Slide>
		`}
	</Code>
</Slide>

<Slide id="boxes" animate>
	<p class="capitalize">Cool transitions</p>
	<div class="flex gap-2 place-content-center">
		<div data-id="box-1" class="w-[100px] h-[100px] bg-gray-400" />
		<div data-id="box-2" class="w-[100px] h-[100px] bg-gray-400" />
		<div data-id="box-3" class="w-[100px] h-[100px] bg-gray-400" />
	</div>
</Slide>

<Slide id="boxes" animate>
	<p class="capitalize">Moving boxes</p>
	<div class="flex gap-2 place-content-center">
		<div data-id="box-1" class="w-[200px] h-[200px] bg-red-400" />
		<div data-id="box-2" class="w-[200px] h-[200px] bg-green-400" />
		<div data-id="box-3" class="w-[200px] h-[200px] bg-blue-400" />
	</div>
	<p class="capitalize">Cool transitions</p>
</Slide>

<Slide id="boxes" animate>
	<p>Moving boxes</p>
	<div class="flex gap-2 place-content-center">
		<div data-id="box-1" class="w-[200px] h-[200px] bg-gray-400" />
		<img src="https://i.giphy.com/media/ToMjGpnXBTw7vnokxhu/giphy.webp" alt="Whoa" />
		<div data-id="box-3" class="w-[200px] h-[200px] bg-gray-400" />
	</div>
	<p>Whoa!</p>
</Slide>