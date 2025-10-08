<script>
	import favicon from '$lib/assets/favicon.svg';
	import Navigation from '$lib/components/navigation.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<header>
<h1>My Awesome Website</h1>
<Navigation />
</header>

{@render children?.()}

<style>
	:global(body){
		font-family: Verdana, Geneva, Tahoma, sans-serif;
	}
	
</style>
