<!-- Main Layout -->
 
<script lang="ts">
	import { resolve } from '$app/paths';
	import favicon from '$lib/assets/favicon.svg';
	import "$lib/zine_style.css";

	// const resolved = resolve("/");

	let { children } = $props();
</script>


<div class="drawer">
	<input id="navigation-drawer" type="checkbox" class="drawer-toggle" />
	<div class="drawer-content flex flex-col">
		<!-- Navbar -->
		<nav class="navbar bg-base-300 shadow-sm w-full" id="header_menu">
			<div class="flex-none md:hidden">
				<label for="navigation-drawer" aria-label="open sidebar" class="btn btn-square btn-ghost">
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
			<div class="navbar-center hidden flex-none md:block">
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
				<!-- Empty div to avoid side scrolling due to the label -->
				<div class="w-1"></div>
			</div>
		</nav>

	</div>
	<div class="drawer-side">
		<label for="navigation-drawer" aria-label="close sidebar" class="drawer-overlay"></label>
		<ul class="menu bg-base-200 min-h-full w-80 p-4 pt-10">
			<!-- Sidebar content here -->
			<!-- NB : Forced compiler to not pay attention to potentially null component with "!" -->
			<a class="btn btn-ghost text-xl" onclick={() => {document.getElementById('navigation-drawer')!.click()}} href="{resolve("/")}">Home</a>
			<a class="btn btn-ghost text-xl" onclick={() => {document.getElementById('navigation-drawer')!.click()}} href="{resolve("/ineffableVoyageZine")}">Ineffable Voyage zine</a>
			<a class="btn btn-ghost text-xl" onclick={() => {document.getElementById('navigation-drawer')!.click()}} href="{resolve("/ineffableCuisineZine")}">Ineffable Cuisine zine</a>
			<a class="btn btn-ghost text-xl" onclick={() => {document.getElementById('navigation-drawer')!.click()}} href="{resolve("/about")}">About</a>
			<button class="btn btn-ghost" aria-label="close button" onclick={() => {document.getElementById('navigation-drawer')!.click()}}>
					<svg
						class="swap-on fill-current"
						xmlns="http://www.w3.org/2000/svg"
						width="32"
						height="32"
						viewBox="0 0 512 512">
						<polygon
						points="400 145.49 366.51 112 256 222.51 145.49 112 112 145.49 222.51 256 112 366.51 145.49 400 256 289.49 366.51 400 400 366.51 289.49 256 400 145.49" />
					</svg>
			</button>
		</ul>
	</div>
</div>


<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}
