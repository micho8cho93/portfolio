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

<!-- Fullscreen overlay for animation and greeting -->
<div
	class="fixed inset-0 w-full h-full z-50 flex flex-col pointer-events-auto transition-opacity duration-500 bg-indigo-950"
	class:opacity-0={showContent}
	class:pointer-events-none={showContent}
>
	<!-- Top-left IntroAnimation -->
	<div class="absolute top-0 left-0 p-4">
		<IntroAnimation />
	</div>
	<!-- Centered greeting -->
	<div class="flex-1 flex items-center justify-center">
		<span class="text-6xl font-bold font-mono text-center">{displayed}</span>
	</div>
</div>

<!-- Main content, only visible after animation -->
<div class="main-content transition-opacity duration-500" class:opacity-100={showContent} class:opacity-0={!showContent}>
	<slot />
</div>

<style>
	.main-content {
		transition: opacity 2.5s ease-in-out;
	}
</style>