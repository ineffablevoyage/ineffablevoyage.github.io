<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';
	import "$lib/zine_style.css";

	let { children } = $props();
</script>

<nav class="navbar bg-base-100 shadow-sm" id="header_menu">
	<div class="navbar-start">
	</div>
	<div class="navbar-center">
		<a class="btn btn-ghost text-xl" href="/">Menu</a>
		<a class="btn btn-ghost text-xl" href="/ineffableVoyageZine">Ineffable Voyage zine</a>
		<a class="btn btn-ghost text-xl" href="/ineffableCuisineZine">Ineffable Cuisine zine</a>
		<a class="btn btn-ghost text-xl" href="/about">About</a>
	</div>
	<div class="navbar-end">
	</div>
</nav>



<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}
