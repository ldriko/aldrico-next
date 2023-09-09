<script>
	import '../app.css';
	import { dev } from '$app/environment';
	import { inject } from '@vercel/analytics';

	inject({ mode: dev ? 'development' : 'production' });
</script>

<svelte:head>
	<title>Heaven Aldrico</title>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous" />
	<link
		href="https://fonts.googleapis.com/css2?family=Balsamiq+Sans:wght@400;700&display=swap"
		rel="stylesheet"
	/>
</svelte:head>

<slot />

<style lang="postcss">
	:global(body) {
		@apply py-4;
		@apply px-4;
		@apply lg:px-4;
		@apply lg:py-16;
		font-family: 'Balsamiq Sans', 'comic sans ms', sans-serif;
		@apply text-lg;
		@apply cursor-default;
	}
</style>
