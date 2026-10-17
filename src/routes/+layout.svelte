<script lang="ts">
	import DemoLinks from './demo/DemoLinks.svelte';
	import Homepage from './home/+page.svelte';
	import favicon from '#lib/assets/favicon.svg';
	import type { LayoutProps } from './$types';

	let { children }: LayoutProps = $props();
</script>

<a href="/">Doggopolis</a>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}
<DemoLinks />
