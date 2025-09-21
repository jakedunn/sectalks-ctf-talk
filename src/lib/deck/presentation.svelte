<script lang="ts">
	import Slide from './slide.svelte'
	import Code from './code.svelte'
	import Markdown from './markdown.svelte'
	import Notes from './notes.svelte'
</script>

<Slide>
	<div class="h-full flex flex-col justify-between">
		<div class="flex-1 flex flex-col items-center justify-center">
			<p class="capitalize">How to run a CTF</p>
			<p class="capitalize">💻🔥😅🇦🇺</p>
		</div>
		<div class="flex justify-center">
			<img src="/sectalks.png" alt="Sectalks" class="w-48 h-48 object-contain"/>
		</div>
	</div>
</Slide>

<Slide>
	<p class="lowercase">whoami</p>
	<div class="flex items-center justify-center gap-12">
		<img src="/nomad.jpeg" alt="Nomad" class="w-48 h-48 rounded-full object-cover" />
		<div class="flex flex-col text-xl space-y-2">
			<p class="font-bold">@nomad / Jake</p>
			<ul class="list-disc list-inside space-y-1">
				<li>Division 5 - Head of Assurance</li>
				<li>Bsides Brisbane - CTF Organiser</li>
				<li>Sectalks Brisbane - Co-Organiser</li>
			</ul>
			<hr class="my-2 border-gray-400" />
			<ul class="list-disc list-inside space-y-1">
				<li>Pentester - ~7 years</li>
				<li>Dev/Freelancer - ~5 years</li>
			</ul>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="capitalize">What is a CTF?</p>
</Slide>

<Slide id="animate" animate>
	<p class="capitalize">What is a CTF?</p>
	<p class="capitalize">Capture The Flag</p>
</Slide>

<Slide id="animate" animate>
	<p>Great so what's a flag?</p>
</Slide>
<Slide id="animate" animate>
	<p>Great so what's a flag?</p>
	<p class="text-xl">flag&lbrace;my-cool-flag&rbrace;</p>
</Slide>
<Slide id="animate" animate>
	<p>Great so what's a flag?</p>
	<p class="text-xl">flag&lbrace;my-cool-flag&rbrace;</p>
	<p class="text-xl">flag&lbrace;my-c00l-fl4g&rbrace;</p>
</Slide>
<Slide id="animate" animate>
	<p>Great so what's a flag?</p>
	<p class="text-xl">flag&lbrace;my-cool-flag&rbrace;</p>
	<p class="text-xl">flag&lbrace;my-c00l-fl4g&rbrace;</p>
	<p class="text-xl">flag&lbrace;7131aed82d64caa5cee66c0ee1ebf5d3&rbrace;</p>
</Slide>
<Slide id="animate" animate>
	<p>Great so what's a flag?</p>
	<p class="text-xl">flag&lbrace;my-cool-flag&rbrace;</p>
	<p class="text-xl">flag&lbrace;my-c00l-fl4g&rbrace;</p>
	<p class="text-xl">flag&lbrace;7131aed82d64caa5cee66c0ee1ebf5d3&rbrace;</p>
	<p class="text-xl">bsides&lbrace;my-cool-flag&rbrace;</p>
</Slide>

<Slide id="animate" animate>
	<p>What do you need to host a CTF?</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-2xl">Content / Challenges</li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<p>What do you need to host a CTF?</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-gray-500">Content / Challenges</li>
		<li class="text-2xl">Infrastructure</li>
	</ul>
</Slide>
<Slide id="animate" animate>
	<p>What do you need to host a CTF?</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-gray-500">Content / Challenges</li>
		<li class="text-gray-500">Infrastructure</li>
		<li class="text-2xl">Platform</li>
	</ul>
</Slide>
<Slide id="animate" animate>
	<p>What do you need to host a CTF?</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-gray-500">Content / Challenges</li>
		<li class="text-gray-500">Infrastructure</li>
		<li class="text-gray-500">Platform</li>
		<li class="text-2xl">Event</li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-2xl">web</li>
			</ul>
		</div>
		<div class="text-2xl text-center">
			<p>Web application challenges - SQLi, XSS, SSRF, RCE, etc.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-2xl">pwn</li>
			</ul>
		</div>
		<div class="text-2xl text-center">
			<p>Binary exploitation - Buffer overflows, ROP, heap exploitation</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-gray-500">pwn</li>
				<li class="text-2xl">rev</li>
			</ul>
		</div>
		<div class="text-xl text-center">
			<p>Reverse engineering - Static/dynamic analysis, crackmes, licesnse bypasses, etc.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-gray-500">pwn</li>
				<li class="text-gray-500">rev</li>
				<li class="text-2xl">crypto</li>
			</ul>
		</div>
		<div class="text-2xl text-center">
			<p>Encryption, RSA, AES, smart stuff.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-gray-500">pwn</li>
				<li class="text-gray-500">rev</li>
				<li class="text-gray-500">crypto</li>
				<li class="text-2xl">forensics</li>
			</ul>
		</div>
		<div class="text-2xl text-center">
			<p>Log analysis, network traffic, memory dumps</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-gray-500">pwn</li>
				<li class="text-gray-500">rev</li>
				<li class="text-gray-500">crypto</li>
				<li class="text-gray-500">forensics</li>
				<li class="text-2xl">osint</li>
			</ul>
		</div>
		<div class="text-xl text-center">
			<p>trawling the Internet, figure out where a photo was taken, etc.</p>
		</div>
	</div>
</Slide>
<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-gray-500">pwn</li>
				<li class="text-gray-500">rev</li>
				<li class="text-gray-500">crypto</li>
				<li class="text-gray-500">forensics</li>
				<li class="text-gray-500">osint</li>
				<li class="text-2xl">hardware</li>
			</ul>
		</div>
		<div class="text-xl text-center">
			<p>busting protocols, hacking electronics, SCADA/ICS, etc.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-gray-500">pwn</li>
				<li class="text-gray-500">rev</li>
				<li class="text-gray-500">crypto</li>
				<li class="text-gray-500">forensics</li>
				<li class="text-gray-500">osint</li>
				<li class="text-gray-500">hardware</li>
				<li class="text-2xl">misc</li>
			</ul>
		</div>
		<div class="text-xl text-center">
			<p>Everything Else - Steganography, logic puzzles, the world is your oyster.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">How do we get content / challenges?</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-2xl">CTF Admins</li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">How do we get content / challenges?</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-gray-500">CTF Admins</li>
		<li class="text-2xl">Volunteer Submission</li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">What makes a good challenge?</p>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">What makes a good challenge?</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-2xl">Unique</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Based around some attack primative, or some interesting concept.</p>
			<p>Realism is nice, but not necessary.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">What makes a good challenge?</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Unique</li>
				<li class="text-2xl">Solvable</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Players should have a reasonable chance of solving it during the event.</p>
			<p>Find a 0-day in Windows 10 is a bad challenge, unless it's pwn2own.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">What makes a good challenge?</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Unique</li>
				<li class="text-gray-500">Solvable</li>
				<li class="text-2xl">Balanced</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Players will come from varying skill levels.</p>
			<p>There should be a mix of easy and hard challenges.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">What makes a good challenge?</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Unique</li>
				<li class="text-gray-500">Solvable</li>
				<li class="text-gray-500">Balanced</li>
				<li class="text-2xl">Deployable</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Challenges should be easy enough to host</p>
			<p>with many players connecting to it.</p>
		</div>
	</div>
	<Notes>
		Chals such as Stored XSS, RCE, SSTI, Race conditions - need instances chals to be successful chals
	</Notes>
</Slide>

<Slide id="animate" animate>
		<p>Platform</p>
</Slide>
<Slide id="animate" animate>
	<p>Platform</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center justify-center w-1/3">
			<p class="text-4xl">CTFd</p>
		</div>
		<div class="w-2/3">
			<img src="/score-board.png" alt="CTFd" class="w-full h-full object-contain" />
		</div>
	</div>
</Slide>
<Slide id="animate" animate>
	<p>Platform</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center justify-center w-1/3">
			<p class="text-4xl">CTFd</p>
		</div>
		<div class="w-2/3">
			<img src="/score-board-2.png" alt="CTFd" class="w-full h-full object-contain" />
		</div>
	</div>
</Slide>


<Slide id="animate" animate>
	<p>infrastructure</p>
</Slide>
<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-2xl">Description Only</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Easy. Upload the challenge description to the platform and call it a day</p>
		</div>
	</div>
</Slide>
<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Description Only</li>
				<li class="text-2xl">Static</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Easy. Upload the challenge files to the platform and call it a day</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Description Only</li>
				<li class="text-gray-500">Static File</li>
				<li class="text-2xl">Shared Hosting</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Each player is connecting to the same instance.</p>
			<p>Fairly easy to set up - Typically, Docker Compose.</p>
			<p>Probably still fronted with a Load Balancer for TLS</p>
		</div>
	</div>
</Slide>
<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Description Only</li>
				<li class="text-gray-500">Static File</li>
				<li class="text-gray-500">Shared Hosting</li>
				<li class="text-2xl">Instanced</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Each player / team is connecting to their own instance.</p>
			<p>Requires clustered infrastructure - K8s, ECS, etc.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Description Only</li>
				<li class="text-gray-500">Static File</li>
				<li class="text-gray-500">Shared Hosting</li>
				<li class="text-gray-500">Instanced</li>
				<li class="text-2xl">Lab</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Players are given a full lab environment, usually many flags in the lab.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Description Only</li>
				<li class="text-gray-500">Static File</li>
				<li class="text-gray-500">Shared Hosting</li>
				<li class="text-gray-500">Instanced</li>
				<li class="text-gray-500">Lab</li>
				<li class="text-2xl">Hardware</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Hardware setup in CTF village, players have to phyically go there an hack stuff</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-2xl">Automate as much as possible</li>
		<li class="text-2xl">IaC with some gitops keeps things reliable</li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-2xl">Monorepo of challenges</li>
		<li class="text-2xl">GitHub Actions watching repo for changes</li>
		<li class="text-2xl">GHA -&gt; AWS ECR -&gt; Terraform -&gt; ECS Cluster(s)</li>
		<li class="text-2xl">Challenge yml files scripted to deploy challenge metadata</li>
	</ul>
</Slide>


<Slide id="animate" animate>
	<p>infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center justify-center w-1/3">
			<p class="text-2xl">Each Team Has Their Own ECS Cluster</p>
		</div>
		<div class="w-2/3">
			<img src="/ECS.png" alt="ECS" class="w-full h-full object-contain" />
		</div>
	</div>
</Slide>
<Slide id="animate" animate>
	<img src="/ECS.png" alt="ECS" class="w-full h-full object-contain" />
</Slide>
<Slide id="animate" animate>
	<p>infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center justify-center w-1/3">
			<p class="text-4xl">Lots of clusters</p>
		</div>
		<div class="w-2/3">
			<img src="/cluster.png" alt="ECS" class="w-full h-full object-contain" />
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<img src="/cluster.png" alt="ECS" class="w-full h-full object-contain" />
</Slide>
<Slide id="animate" animate>
	<p>infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center justify-center w-1/3">
			<p class="text-4xl">AD Lab</p>
		</div>
		<div class="w-2/3">
			<img src="/apex.png" alt="ECS" class="w-full h-full object-contain" />
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<img src="/apex.png" alt="ECS" class="w-full h-full object-contain" />
</Slide>
<Slide id="animate" animate>
	<p>infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center justify-center w-1/3">
			<p class="text-4xl">Monitoring</p>
		</div>
		<div class="w-2/3">
			<img src="/monitor1.png" alt="ECS" class="w-full h-full object-contain" />
			<img src="/monitor2.png" alt="ECS" class="w-full h-full object-contain" />
		</div>
	</div>
</Slide>
<Slide id="animate" animate>
	<p>lessons learned</p>
</Slide>

<Slide id="animate" animate>
	<p>lessons learned</p>
	<p class="text-4xl">#1 rule</p>
	<p class="text-2xl">Don't fuck up DNS.</p>
</Slide>
<Slide id="animate" animate>
	<p>lessons learned</p>
	<p class="text-2xl">Automation is key</p>
	<p class="text-2xl">Brings reliability to spaghetti</p>
</Slide>
<Slide id="animate" animate>
	<p>lessons learned</p>
	<p class="text-2xl">Automation is key</p>
	<p class="text-2xl">Brings reliability to spaghetti</p>
	<p class="text-2xl">... and helps not fuck up DNS.</p>
</Slide>
<Slide id="animate" animate>
	<p>lessons learned</p>
	<p class="text-2xl">terraform is amazing</p>
	<p class="text-2xl">but large statefiles are not.</p>
</Slide>
<Slide id="animate" animate>
	<p>lessons learned</p>
	<p class="text-2xl">AWS Application Load balancers are amazing</p>
	<p class="text-2xl">unless you need more than 100 rules.</p>
</Slide>
<Slide id="animate" animate>
	<p>lessons yet to learn</p>
	<p class="text-2xl">You should not start prepping the CTF with only weeks to go</p>
</Slide>
<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<a href="https://github.com/BsidesBNE-CTF/infrastructure/tree/main/terraform">Code Demo</a>
</Slide>

<Slide id="animate" animate>
	<div class="flex items-center justify-center gap-6">
		<p class="text-4xl">Sectalks CTF</p>
		<img src="/sectalks-sm.png" alt="Sectalks" class="w-24 h-24 rounded-full object-cover" />
	</div>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-2xl">Late November</li>
		<li class="text-2xl">Collaborating with other Sectalks Chapters</li>
		<li class="text-2xl">Need volunteer challenge contributers!</li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<div class="flex items-center justify-center gap-6">
		<p class="text-4xl">Sectalks CTF</p>
		<img src="/sectalks-sm.png" alt="Sectalks" class="w-24 h-24 rounded-full object-cover" />
	</div>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-2xl">Speak to me (@nomad) via Slack to get involved</li>
		<li class="text-2xl"><a href="https://github.com/sectalks-bne/submission-template">Challenge Submission Template</a></li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<p>Questions?</p>
	<p class="text-lg">:wq</p>
</Slide>

<Slide id="animate" animate>
	<p>Thank you Sponsors!</p>
	<div class="flex flex-col justify-center items-center space-y-8">
		<div class="w-42 h-42 flex items-center justify-center">
			<div class="text-6xl mr-8">🏢: </div>
			<img src="/bdo-logo.png" alt="BDO" class="w-full h-full object-contain" />
		</div>
		<div class="w-70 h-70 flex items-center justify-center">
			<div class="text-6xl mr-8">🍕: </div>
			<img src="/Division5-Logo.webp" alt="Division5" class="w-full h-full object-contain" />
		</div>
	</div>
	<p class="pt-16 text-sm">ps: if you're not in sectalks Slack, speak to one of the organizers after the talk</p>
</Slide><script lang="ts">
	import Slide from './slide.svelte'
	import Code from './code.svelte'
	import Markdown from './markdown.svelte'
	import Notes from './notes.svelte'
</script>

<Slide>
	<div class="h-full flex flex-col justify-between">
		<div class="flex-1 flex flex-col items-center justify-center">
			<p class="capitalize">How to run a CTF</p>
			<p class="capitalize">💻🔥😅🇦🇺</p>
		</div>
		<div class="flex justify-center">
			<img src="/sectalks.png" alt="Sectalks" class="w-48 h-48 object-contain"/>
		</div>
	</div>
</Slide>

<Slide>
	<p class="lowercase">whoami</p>
	<div class="flex items-center justify-center gap-12">
		<img src="/nomad.jpeg" alt="Nomad" class="w-48 h-48 rounded-full object-cover" />
		<div class="flex flex-col text-xl space-y-2">
			<p class="font-bold">@nomad / Jake</p>
			<ul class="list-disc list-inside space-y-1">
				<li>Division 5 - Head of Assurance</li>
				<li>Bsides Brisbane - CTF Organiser</li>
				<li>Sectalks Brisbane - Co-Organiser</li>
			</ul>
			<hr class="my-2 border-gray-400" />
			<ul class="list-disc list-inside space-y-1">
				<li>Pentester - ~7 years</li>
				<li>Dev/Freelancer - ~5 years</li>
			</ul>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="capitalize">What is a CTF?</p>
</Slide>

<Slide id="animate" animate>
	<p class="capitalize">What is a CTF?</p>
	<p class="capitalize">Capture The Flag</p>
</Slide>

<Slide id="animate" animate>
	<p>Great so what's a flag?</p>
</Slide>
<Slide id="animate" animate>
	<p>Great so what's a flag?</p>
	<p class="text-xl">flag&lbrace;my-cool-flag&rbrace;</p>
</Slide>
<Slide id="animate" animate>
	<p>Great so what's a flag?</p>
	<p class="text-xl">flag&lbrace;my-cool-flag&rbrace;</p>
	<p class="text-xl">flag&lbrace;my-c00l-fl4g&rbrace;</p>
</Slide>
<Slide id="animate" animate>
	<p>Great so what's a flag?</p>
	<p class="text-xl">flag&lbrace;my-cool-flag&rbrace;</p>
	<p class="text-xl">flag&lbrace;my-c00l-fl4g&rbrace;</p>
	<p class="text-xl">flag&lbrace;7131aed82d64caa5cee66c0ee1ebf5d3&rbrace;</p>
</Slide>
<Slide id="animate" animate>
	<p>Great so what's a flag?</p>
	<p class="text-xl">flag&lbrace;my-cool-flag&rbrace;</p>
	<p class="text-xl">flag&lbrace;my-c00l-fl4g&rbrace;</p>
	<p class="text-xl">flag&lbrace;7131aed82d64caa5cee66c0ee1ebf5d3&rbrace;</p>
	<p class="text-xl">bsides&lbrace;my-cool-flag&rbrace;</p>
</Slide>

<Slide id="animate" animate>
	<p>What do you need to host a CTF?</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-2xl">Content / Challenges</li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<p>What do you need to host a CTF?</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-gray-500">Content / Challenges</li>
		<li class="text-2xl">Infrastructure</li>
	</ul>
</Slide>
<Slide id="animate" animate>
	<p>What do you need to host a CTF?</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-gray-500">Content / Challenges</li>
		<li class="text-gray-500">Infrastructure</li>
		<li class="text-2xl">Platform</li>
	</ul>
</Slide>
<Slide id="animate" animate>
	<p>What do you need to host a CTF?</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-gray-500">Content / Challenges</li>
		<li class="text-gray-500">Infrastructure</li>
		<li class="text-gray-500">Platform</li>
		<li class="text-2xl">Event</li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-2xl">web</li>
			</ul>
		</div>
		<div class="text-2xl text-center">
			<p>Web application challenges - SQLi, XSS, SSRF, RCE, etc.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-2xl">pwn</li>
			</ul>
		</div>
		<div class="text-2xl text-center">
			<p>Binary exploitation - Buffer overflows, ROP, heap exploitation</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-gray-500">pwn</li>
				<li class="text-2xl">rev</li>
			</ul>
		</div>
		<div class="text-xl text-center">
			<p>Reverse engineering - Static/dynamic analysis, crackmes, licesnse bypasses, etc.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-gray-500">pwn</li>
				<li class="text-gray-500">rev</li>
				<li class="text-2xl">crypto</li>
			</ul>
		</div>
		<div class="text-2xl text-center">
			<p>Encryption, RSA, AES, smart stuff.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-gray-500">pwn</li>
				<li class="text-gray-500">rev</li>
				<li class="text-gray-500">crypto</li>
				<li class="text-2xl">forensics</li>
			</ul>
		</div>
		<div class="text-2xl text-center">
			<p>Log analysis, network traffic, memory dumps</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-gray-500">pwn</li>
				<li class="text-gray-500">rev</li>
				<li class="text-gray-500">crypto</li>
				<li class="text-gray-500">forensics</li>
				<li class="text-2xl">osint</li>
			</ul>
		</div>
		<div class="text-xl text-center">
			<p>trawling the Internet, figure out where a photo was taken, etc.</p>
		</div>
	</div>
</Slide>
<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-gray-500">pwn</li>
				<li class="text-gray-500">rev</li>
				<li class="text-gray-500">crypto</li>
				<li class="text-gray-500">forensics</li>
				<li class="text-gray-500">osint</li>
				<li class="text-2xl">hardware</li>
			</ul>
		</div>
		<div class="text-xl text-center">
			<p>busting protocols, hacking electronics, SCADA/ICS, etc.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="lowercase">challenges</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">web</li>
				<li class="text-gray-500">pwn</li>
				<li class="text-gray-500">rev</li>
				<li class="text-gray-500">crypto</li>
				<li class="text-gray-500">forensics</li>
				<li class="text-gray-500">osint</li>
				<li class="text-gray-500">hardware</li>
				<li class="text-2xl">misc</li>
			</ul>
		</div>
		<div class="text-xl text-center">
			<p>Everything Else - Steganography, logic puzzles, the world is your oyster.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">How do we get content / challenges?</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-2xl">CTF Admins</li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">How do we get content / challenges?</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-gray-500">CTF Admins</li>
		<li class="text-2xl">Volunteer Submission</li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">What makes a good challenge?</p>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">What makes a good challenge?</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-2xl">Unique</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Based around some attack primative, or some interesting concept.</p>
			<p>Realism is nice, but not necessary.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">What makes a good challenge?</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Unique</li>
				<li class="text-2xl">Solvable</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Players should have a reasonable chance of solving it during the event.</p>
			<p>Find a 0-day in Windows 10 is a bad challenge, unless it's pwn2own.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">What makes a good challenge?</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Unique</li>
				<li class="text-gray-500">Solvable</li>
				<li class="text-2xl">Balanced</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Players will come from varying skill levels.</p>
			<p>There should be a mix of easy and hard challenges.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">What makes a good challenge?</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Unique</li>
				<li class="text-gray-500">Solvable</li>
				<li class="text-gray-500">Balanced</li>
				<li class="text-2xl">Deployable</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Challenges should be easy enough to host</p>
			<p>with many players connecting to it.</p>
		</div>
	</div>
	<Notes>
		Chals such as Stored XSS, RCE, SSTI, Race conditions - need instances chals to be successful chals
	</Notes>
</Slide>

<Slide id="animate" animate>
		<p>Platform</p>
</Slide>
<Slide id="animate" animate>
	<p>Platform</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center justify-center w-1/3">
			<p class="text-4xl">CTFd</p>
		</div>
		<div class="w-2/3">
			<img src="/score-board.png" alt="CTFd" class="w-full h-full object-contain" />
		</div>
	</div>
</Slide>
<Slide id="animate" animate>
	<p>Platform</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center justify-center w-1/3">
			<p class="text-4xl">CTFd</p>
		</div>
		<div class="w-2/3">
			<img src="/score-board-2.png" alt="CTFd" class="w-full h-full object-contain" />
		</div>
	</div>
</Slide>


<Slide id="animate" animate>
	<p>infrastructure</p>
</Slide>
<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-2xl">Description Only</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Easy. Upload the challenge description to the platform and call it a day</p>
		</div>
	</div>
</Slide>
<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Description Only</li>
				<li class="text-2xl">Static</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Easy. Upload the challenge files to the platform and call it a day</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Description Only</li>
				<li class="text-gray-500">Static File</li>
				<li class="text-2xl">Shared Hosting</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Each player is connecting to the same instance.</p>
			<p>Fairly easy to set up - Typically, Docker Compose.</p>
			<p>Probably still fronted with a Load Balancer for TLS</p>
		</div>
	</div>
</Slide>
<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Description Only</li>
				<li class="text-gray-500">Static File</li>
				<li class="text-gray-500">Shared Hosting</li>
				<li class="text-2xl">Instanced</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Each player / team is connecting to their own instance.</p>
			<p>Requires clustered infrastructure - K8s, ECS, etc.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Description Only</li>
				<li class="text-gray-500">Static File</li>
				<li class="text-gray-500">Shared Hosting</li>
				<li class="text-gray-500">Instanced</li>
				<li class="text-2xl">Lab</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Players are given a full lab environment, usually many flags in the lab.</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center border-r-4 border-red-700 pr-8">
			<ul class="list-disc list-inside space-y-2 text-xl">
				<li class="text-gray-500">Description Only</li>
				<li class="text-gray-500">Static File</li>
				<li class="text-gray-500">Shared Hosting</li>
				<li class="text-gray-500">Instanced</li>
				<li class="text-gray-500">Lab</li>
				<li class="text-2xl">Hardware</li>
			</ul>
		</div>
		<div class="text-lg text-right">
			<p>Hardware setup in CTF village, players have to phyically go there an hack stuff</p>
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-2xl">Automate as much as possible</li>
		<li class="text-2xl">IaC with some gitops keeps things reliable</li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-2xl">Monorepo of challenges</li>
		<li class="text-2xl">GitHub Actions watching repo for changes</li>
		<li class="text-2xl">GHA -&gt; AWS ECR -&gt; Terraform -&gt; ECS Cluster(s)</li>
		<li class="text-2xl">Challenge yml files scripted to deploy challenge metadata</li>
	</ul>
</Slide>


<Slide id="animate" animate>
	<p>infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center justify-center w-1/3">
			<p class="text-2xl">Each Team Has Their Own ECS Cluster</p>
		</div>
		<div class="w-2/3">
			<img src="/ECS.png" alt="ECS" class="w-full h-full object-contain" />
		</div>
	</div>
</Slide>
<Slide id="animate" animate>
	<img src="/ECS.png" alt="ECS" class="w-full h-full object-contain" />
</Slide>
<Slide id="animate" animate>
	<p>infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center justify-center w-1/3">
			<p class="text-4xl">Lots of clusters</p>
		</div>
		<div class="w-2/3">
			<img src="/cluster.png" alt="ECS" class="w-full h-full object-contain" />
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<img src="/cluster.png" alt="ECS" class="w-full h-full object-contain" />
</Slide>
<Slide id="animate" animate>
	<p>infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center justify-center w-1/3">
			<p class="text-4xl">AD Lab</p>
		</div>
		<div class="w-2/3">
			<img src="/apex.png" alt="ECS" class="w-full h-full object-contain" />
		</div>
	</div>
</Slide>

<Slide id="animate" animate>
	<img src="/apex.png" alt="ECS" class="w-full h-full object-contain" />
</Slide>
<Slide id="animate" animate>
	<p>infrastructure</p>
	<div class="flex items-center justify-between h-full">
		<div class="flex items-center justify-center w-1/3">
			<p class="text-4xl">Monitoring</p>
		</div>
		<div class="w-2/3">
			<img src="/monitor1.png" alt="ECS" class="w-full h-full object-contain" />
			<img src="/monitor2.png" alt="ECS" class="w-full h-full object-contain" />
		</div>
	</div>
</Slide>
<Slide id="animate" animate>
	<p>lessons learned</p>
</Slide>

<Slide id="animate" animate>
	<p>lessons learned</p>
	<p class="text-4xl">#1 rule</p>
	<p class="text-2xl">Don't fuck up DNS.</p>
</Slide>
<Slide id="animate" animate>
	<p>lessons learned</p>
	<p class="text-2xl">Automation is key</p>
	<p class="text-2xl">Brings reliability to spaghetti</p>
</Slide>
<Slide id="animate" animate>
	<p>lessons learned</p>
	<p class="text-2xl">Automation is key</p>
	<p class="text-2xl">Brings reliability to spaghetti</p>
	<p class="text-2xl">... and helps not fuck up DNS.</p>
</Slide>
<Slide id="animate" animate>
	<p>lessons learned</p>
	<p class="text-2xl">terraform is amazing</p>
	<p class="text-2xl">but large statefiles are not.</p>
</Slide>
<Slide id="animate" animate>
	<p>lessons learned</p>
	<p class="text-2xl">AWS Application Load balancers are amazing</p>
	<p class="text-2xl">unless you need more than 100 rules.</p>
</Slide>
<Slide id="animate" animate>
	<p>lessons yet to learn</p>
	<p class="text-2xl">You should not start prepping the CTF with only weeks to go</p>
</Slide>
<Slide id="animate" animate>
	<p class="text-4xl">infrastructure</p>
	<a href="https://github.com/BsidesBNE-CTF/infrastructure/tree/main/terraform">Code Demo</a>
</Slide>

<Slide id="animate" animate>
	<div class="flex items-center justify-center gap-6">
		<p class="text-4xl">Sectalks CTF</p>
		<img src="/sectalks-sm.png" alt="Sectalks" class="w-24 h-24 rounded-full object-cover" />
	</div>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-2xl">Late November</li>
		<li class="text-2xl">Collaborating with other Sectalks Chapters</li>
		<li class="text-2xl">Need volunteer challenge contributers!</li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<div class="flex items-center justify-center gap-6">
		<p class="text-4xl">Sectalks CTF</p>
		<img src="/sectalks-sm.png" alt="Sectalks" class="w-24 h-24 rounded-full object-cover" />
	</div>
	<ul class="list-disc list-inside space-y-2 text-xl">
		<li class="text-2xl">Speak to me (@nomad) via Slack to get involved</li>
		<li class="text-2xl"><a href="https://github.com/sectalks-bne/submission-template">Challenge Submission Template</a></li>
	</ul>
</Slide>

<Slide id="animate" animate>
	<p>Questions?</p>
	<p class="text-lg">:wq</p>
</Slide>

<Slide id="animate" animate>
	<p>Thank you Sponsors!</p>
	<div class="flex flex-col justify-center items-center space-y-8">
		<div class="w-42 h-42 flex items-center justify-center">
			<div class="text-6xl mr-8">🏢: </div>
			<img src="/bdo-logo.png" alt="BDO" class="w-full h-full object-contain" />
		</div>
		<div class="w-70 h-70 flex items-center justify-center">
			<div class="text-6xl mr-8">🍕: </div>
			<img src="/Division5-Logo.webp" alt="Division5" class="w-full h-full object-contain" />
		</div>
	</div>
	<p class="pt-16 text-sm">ps: if you're not in sectalks Slack, speak to one of the organizers after the talk</p>
</Slide>
