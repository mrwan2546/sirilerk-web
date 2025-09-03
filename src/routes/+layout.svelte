<script lang="ts">
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>Sirilerk | Home</title>
	<meta name="description" content="Made with by passion and make it happen." />
	<meta property="og:url" content="https://sirilerk.com" />
	<meta property="og:site_name" content="Sirilerk" />
	<meta property="og:title" content="Sirilerk" />
	<meta property="og:description" content="Made with by passion and make it happen." />
	<meta property="og:image" content="/image/banner.png" />
</svelte:head>

{@render children?.()}
