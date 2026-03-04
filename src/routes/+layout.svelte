<!-- Main Layout -->
 
<script lang="ts">
	import { resolve } from '$app/paths';
	import favicon from '$lib/assets/favicon.svg';
	import "$lib/zine_style.css";

	// const resolved = resolve("/");

	let { children } = $props();
</script>


<div class="drawer">
	<input id="my-drawer-2" type="checkbox" class="drawer-toggle" />
	<div class="drawer-content flex flex-col">
		<!-- Navbar -->
		<nav class="navbar bg-base-300 shadow-sm w-full" id="header_menu">
			<div class="flex-none lg:hidden">
				<label for="my-drawer-2" aria-label="open sidebar" class="btn btn-square btn-ghost">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="none"
					viewBox="0 0 24 24"
					class="inline-block h-6 w-6 stroke-current"
				>
					<path
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					d="M4 6h16M4 12h16M4 18h16"
					></path>
				</svg>
				</label>
			</div>
			<div class="navbar-start"></div>
			<div class="navbar-center hidden flex-none lg:block">
				<ul class="menu menu-horizontal">
				<!-- Navbar menu content here -->
					<a class="btn btn-ghost text-xl" href="{resolve("/")}">Home</a>
					<a class="btn btn-ghost text-xl" href="{resolve("/ineffableVoyageZine")}">Ineffable Voyage zine</a>
					<a class="btn btn-ghost text-xl" href="{resolve("/ineffableCuisineZine")}">Ineffable Cuisine zine</a>
					<a class="btn btn-ghost text-xl" href="{resolve("/about")}">About</a>
				</ul>
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

	</div>
	<div class="drawer-side">
		<label for="my-drawer-2" aria-label="close sidebar" class="drawer-overlay"></label>
		<ul class="menu bg-base-200 min-h-full w-80 p-4">
			<!-- Sidebar content here -->
			<a class="btn btn-ghost text-xl" href="{resolve("/")}">Home</a>
			<a class="btn btn-ghost text-xl" href="{resolve("/ineffableVoyageZine")}">Ineffable Voyage zine</a>
			<a class="btn btn-ghost text-xl" href="{resolve("/ineffableCuisineZine")}">Ineffable Cuisine zine</a>
			<a class="btn btn-ghost text-xl" href="{resolve("/about")}">About</a>
		</ul>
	</div>
</div>


<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}
