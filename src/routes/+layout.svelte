<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';
	import "$lib/zine_style.css";

	let { children } = $props();
</script>

<nav class="header" id="header_menu">
        <h2>Menu</h2>
</nav>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}
