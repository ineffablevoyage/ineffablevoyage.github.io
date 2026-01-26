<script lang="ts">
	import { resolve } from '$app/paths';
	import favicon from '$lib/assets/favicon.svg';
	import "$lib/zine_style.css";

	// const resolved = resolve("/");

	let { children } = $props();
</script>

<nav class="navbar bg-base-300 shadow-sm" id="header_menu">
	<div class="navbar-start">
	</div>
	<div class="navbar-center">
		<a class="btn btn-ghost text-xl" href="{resolve("/")}">Menu</a>
		<a class="btn btn-ghost text-xl" href="{resolve("/ineffableVoyageZine")}">Ineffable Voyage zine</a>
		<a class="btn btn-ghost text-xl" href="{resolve("/ineffableCuisineZine")}">Ineffable Cuisine zine</a>
		<a class="btn btn-ghost text-xl" href="{resolve("/about")}">About</a>
	</div>
	<div class="navbar-end">
	</div>
</nav>


<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}
