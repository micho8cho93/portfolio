<script lang="ts">
	export let activeSection: string;
	import { Mail } from 'lucide-svelte';
	import { Linkedin } from 'lucide-svelte';
	import { Github } from 'lucide-svelte';
</script>

<header class="lg:sticky lg:top-0 lg:flex lg:max-h-screen lg:w-1/2 lg:flex-col lg:justify-around">
	<div class="flex flex-col items-center lg:items-start">
		<h1
			class="text-center text-4xl font-bold tracking-tight text-slate-200 sm:text-5xl lg:text-left"
		>
			Michel Honoré
		</h1>

		<p class="max-w-m mt-4 leading-normal">Computer Science Teacher & Software Tinkerer</p>
		<!-- Navigation -->
		<nav class="nav hidden lg:block" aria-label="In-page jump links">
			<ul class="mt-8 w-max">
				<li>
					<a class="group active flex items-center py-3" href="#about">
						<span
							class="nav-indicator mr-4 h-px transition-all
                group-hover:w-16 group-hover:bg-slate-200
                motion-reduce:transition-none
                {activeSection === 'about' ? 'w-16 bg-slate-200' : 'w-8 bg-slate-600'}"
						></span>
						<span
							class="nav-text text-xs font-bold tracking-widest uppercase
                group-hover:text-slate-200
                {activeSection === 'about' ? 'text-slate-200' : 'text-slate-500'}"
						>
							About
						</span>
					</a>
				</li>
				<li>
					<a class="group flex items-center py-3" href="#experience">
						<span
							class="nav-indicator mr-4 h-px transition-all
                group-hover:w-16 group-hover:bg-slate-200
                motion-reduce:transition-none
                {activeSection === 'experience' ? 'w-16 bg-slate-200' : 'w-8 bg-slate-600'}"
						></span>
						<span
							class="nav-text text-xs font-bold tracking-widest uppercase
                group-hover:text-slate-200
                {activeSection === 'experience' ? 'text-slate-200' : 'text-slate-500'}"
						>
							Experience
						</span>
					</a>
				</li>
				<li>
					<a class="group flex items-center py-3" href="#projects">
						<span
							class="nav-indicator mr-4 h-px transition-all
                group-hover:w-16 group-hover:bg-slate-200
                motion-reduce:transition-none
                {activeSection === 'projects' ? 'w-16 bg-slate-200' : 'w-8 bg-slate-600'}"
						></span>
						<span
							class="nav-text text-xs font-bold tracking-widest uppercase
                group-hover:text-slate-200
                {activeSection === 'projects' ? 'text-slate-200' : 'text-slate-500'}"
						>
							Projects
						</span>
					</a>
				</li>
			</ul>
		</nav>
		<br />

		<!-- Skills -->
		<section class="nav hidden lg:block" aria-label="skillset">
			<span
				class="nav-text text-xs font-bold tracking-widest text-slate-500 uppercase group-hover:text-slate-200 group-focus-visible:text-slate-200"
			>
				Programming Languages
			</span>
			<ul class="mt-2 flex w-50 flex-wrap space-y-1 space-x-1">
				<li>
					<div
						class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs leading-5 font-medium text-teal-300"
					>
						Python
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs leading-5 font-medium text-teal-300"
					>
						JavaScript
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs leading-5 font-medium text-teal-300"
					>
						Arduino/C++
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs leading-5 font-medium text-teal-300"
					>
						HTML
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs leading-5 font-medium text-teal-300"
					>
						Tailwind/CSS
					</div>
				</li>
			</ul>
			<br />

			<span
				class="nav-text text-xs font-bold tracking-widest text-slate-500 uppercase group-hover:text-slate-200 group-focus-visible:text-slate-200"
			>
				Frameworks & Tools
			</span>
			<ul class="mt-2 flex w-50 flex-wrap space-y-1 space-x-1">
				<li>
					<div
						class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs leading-5 font-medium text-blue-300"
					>
						Git
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs leading-5 font-medium text-blue-300"
					>
						GitHub
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs leading-5 font-medium text-blue-300"
					>
						Streamlit
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs leading-5 font-medium text-blue-300"
					>
						Django
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs leading-5 font-medium text-blue-300"
					>
						Vercel
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs leading-5 font-medium text-blue-300"
					>
						Railway
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs leading-5 font-medium text-blue-300"
					>
						SQLite
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs leading-5 font-medium text-blue-300"
					>
						PostgreSQL
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs leading-5 font-medium text-blue-300"
					>
						Crontab
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs leading-5 font-medium text-blue-300"
					>
						Gemini CLI
					</div>
				</li>
			</ul>
			<br />

			<span
				class="nav-text text-xs font-bold tracking-widest text-slate-500 uppercase group-hover:text-slate-200 group-focus-visible:text-slate-200"
			>
				Education
			</span>
			<ul class="mt-2 flex w-50 flex-wrap space-y-1 space-x-1">
				<li>
					<div
						class="flex items-center rounded-full bg-fuchsia-400/10 px-3 py-1 text-xs leading-5 font-medium text-fuchsia-300"
					>
						CS Principles
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-fuchsia-400/10 px-3 py-1 text-xs leading-5 font-medium text-fuchsia-300"
					>
						Project-based Learning
					</div>
				</li>
				<li>
					<div
						class="flex items-center rounded-full bg-fuchsia-400/10 px-3 py-1 text-xs leading-5 font-medium text-fuchsia-300"
					>
						Robotics
					</div>
				</li>
			</ul>
		</section>

		<!-- Social Links -->
		<ul class="mt-8 ml-1 flex items-center" aria-label="Social media">
			<li class="mr-5 text-xs">
				<a
					class="block hover:text-teal-300"
					href="https://github.com/micho8cho93"
					target="_blank"
					rel="noreferrer"
				>
					<Github class="h-6 w-6" />
				</a>
			</li>
			<li class="mr-5 text-xs">
				<a
					class="block hover:text-sky-300"
					href="https://www.linkedin.com/in/michel-honore-95a08549/"
					target="_blank"
					rel="noreferrer"
				>
					<Linkedin class="h-6 w-6" />
				</a>
			</li>
			<li class="mr-5 text-xs">
				<a
					class="block hover:text-pink-300"
					href="mailto:michelvahonore@gmail.com"
					target="_blank"
					rel="noreferrer"
				>
					<Mail class="h-6 w-6" />
				</a>
			</li>
		</ul>
	</div>
</header>
