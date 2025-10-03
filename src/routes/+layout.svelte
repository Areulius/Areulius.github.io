export const prerender = true;

<script lang="ts">
	import favicon from '$lib/assets/VA_Logo1.2.webp';


	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children?.()}
