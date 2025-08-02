<script lang="ts">
	import '../app.css';
	import IntroAnimation from '$lib/components/IntroAnimation.svelte';
	import { onMount } from 'svelte';

	let showContent = false;
	const greetings = [
		'Hello!', 'Hola!', 'Hallo!', 'Bonjour!', 'Bom dia!', 'Moien!', 'Aloha!'
	];
	let greeting = "";
	let displayed = "";

	onMount(() => {
		// Pick a random greeting
		greeting = greetings[Math.floor(Math.random() * greetings.length)];
		typeWriter();
		setTimeout(() => {
			showContent = true;
		}, 2500); // Adjust this duration to match your animation's length
	});

	function typeWriter(i = 0) {
		if (i <= greeting.length) {
			displayed = greeting.slice(0, i);
			setTimeout(() => typeWriter(i + 1), 80);
		}
	}
</script>

<!-- Animation container -->
<div>
	<!-- Top-left IntroAnimation -->
	<div
		class="fixed top-0 left-0 z-50 transition-opacity duration-500"
		class:opacity-0={showContent}
		class:pointer-events-none={showContent}
	>
		<IntroAnimation />
	</div>
	<!-- Centered Welcome message -->
	<div
		class="text-6xl font-bold font-mono fixed inset-0 z-20 flex items-center justify-center bg-indigo-950 transition-opacity duration-500"
		class:opacity-0={showContent}
		class:pointer-events-none={showContent}
	>
		{displayed}
	</div>
</div>
<!-- Main content -->
<div class="main-content transition-opacity duration-500" class:opacity-100={showContent}>
	<slot />
</div>

<style>
	.main-content {
		transition: opacity 2.5s ease-in-out;
	}
</style>