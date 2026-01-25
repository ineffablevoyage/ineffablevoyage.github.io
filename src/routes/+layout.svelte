<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';
	import "$lib/zine_style.css";

	let { children } = $props();
</script>

<nav class="navbar bg-base-100 shadow-sm" id="header_menu">
	<a class="btn btn-ghost text-xl" href="/">Menu</a>
	<a class="btn btn-ghost text-xl" href="/ineffableVoyageZine">Ineffable Voyage zine</a>
	<a class="btn btn-ghost text-xl" href="/ineffableCuisineZine">Ineffable Cuisine zine</a>
	<a class="btn btn-ghost text-xl" href="/about">About</a>
	<!-- <h2>Menu</h2> -->
</nav>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}
