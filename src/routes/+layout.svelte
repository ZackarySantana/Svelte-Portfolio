<script lang="ts">
	import Navbar from './Navbar.svelte';
</script>

<svelte:head>
	<title>Zackary's Portfolio</title>
	<meta name="description" content="Zackary Santana's custom portfolio!" />
	<meta
		name="keywords"
		content="New Grad, Portfolio, Projects, Web Development, Node.js, React.js, Remix.js, CSS, Developer, Coder, Programmer, Programming, Languages, Software, Zackary Santana"
	/>

	<link rel="manifest" href="/manifest.json" />

	<link rel="icon" type="image/ico" href="/favicon/favicon.ico" />
	<link rel="apple-touch-icon" sizes="180x180" href="/favicon/apple-touch-icon.png" />
	<link rel="icon" type="image/png" sizes="32x32" href="/favicon/favicon-32x32.png" />
	<link rel="icon" type="image/png" sizes="16x16" href="/favicon/favicon-16x16.png" />

	<meta httpEquiv="Content-Type" content="text/html; charset=utf-8" />
	<meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=5" />
</svelte:head>

<Navbar />
<slot />

<style>
	:global(html) {
		scroll-behavior: smooth;
	}

	:global(body) {
		background-color: #1e1e1e;
		width: 100vw;
		max-width: 100%;
		padding-block: 5vh;
		margin: 0;
		overflow-x: hidden;
		font-family: 'Besley', sans-serif;
		font-weight: 300;
	}

	:global(h1, h2, h3, .logo) {
		font-family: 'Queensides', sans-serif;
		font-weight: 600;
	}

	@font-face {
		font-family: 'Queensides';
		src: url('/fonts/QueensidesLight.ttf') format('truetype');
		font-weight: 400;
	}

	@font-face {
		font-family: 'Queensides';
		src: url('/fonts/QueensidesMedium.ttf') format('truetype');
		font-weight: 500;
	}

	@font-face {
		font-family: 'Queensides';
		src: url('/fonts/QueensidesHeavy.ttf') format('truetype');
		font-weight: 600;
	}

	@font-face {
		font-family: 'Besley';
		src: url('/fonts/Besley.ttf') format('truetype');
	}
</style>
