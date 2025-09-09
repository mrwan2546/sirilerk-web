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

	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
	<link
		href="https://fonts.googleapis.com/css2?family=Noto+Sans+Thai:wght@400..700&display=swap"
		rel="stylesheet"
	/>
</svelte:head>

<div class="container mx-auto mt-8 h-[64px] max-w-[1024px]">
	<aside class="rounded-full bg-[#1E1E1E] p-4 text-white shadow-sm shadow-black/40">
		<ul
			class="flex flex-row items-center justify-center gap-4 font-semibold tracking-wide uppercase"
		>
			<li class="hover-underline duration-300 hover:scale-[1.05]">
				<a href="/" aria-label="Home">{'<Home />'}</a>
			</li>
			<li class="hover-underline duration-300 hover:scale-[1.05]">
				<a href="/showcase" aria-label="My showcase">{'<Showcase />'}</a>
			</li>
			<li class="hover-underline duration-300 hover:scale-[1.05]">
				<a href="/projects" aria-label="My projects">{'<Project />'}</a>
			</li>
		</ul>
	</aside>
</div>

{@render children?.()}
