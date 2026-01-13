<script lang="ts">
	import './layout.css';
	import { dev } from '$app/environment';
	import { injectAnalytics } from '@vercel/analytics/sveltekit';
	// import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();

	injectAnalytics();
</script>

<svelte:head>
	<link rel="icon" href="favicon.png" />
	<title>Shrine</title>
	<meta
		name="description"
		content="Make and code a project about your favorite fictional character, get a grant to buy merch of your character!"
	/>
</svelte:head>
{@render children()}
