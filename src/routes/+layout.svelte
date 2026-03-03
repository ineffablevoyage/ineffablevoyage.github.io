<!-- Main Layout -->
 
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
		<a class="btn btn-ghost text-xl" href="{resolve("/")}">Home</a>
		<a class="btn btn-ghost text-xl" href="{resolve("/ineffableVoyageZine")}">Ineffable Voyage zine</a>
		<a class="btn btn-ghost text-xl" href="{resolve("/ineffableCuisineZine")}">Ineffable Cuisine zine</a>
		<a class="btn btn-ghost text-xl" href="{resolve("/about")}">About</a>
	</div>
	<div class="navbar-end">
		<label class="swap swap-rotate text-4xl">
			<!-- this hidden checkbox controls the state -->
			<input type="checkbox" class="theme-controller" value="crowley" />

			<div class="swap-on">😈</div>
			<div class="swap-off">😇</div>
		</label>
	</div>
</nav>


<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}
