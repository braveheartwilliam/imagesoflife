<script
	lang="js"
	type="module"
>
	import Breadcrumbs from '../lib/Breadcrumbs.svelte';
	import Counter from '../lib/Counter.svelte';
	const item = [
		{ text: 'Home', href: '/' },
		{ text: 'Projects', href: '/projects' },
		{ text: 'Svelte Breadcrumb' },
	];
</script>

<div class="places_home">
	<h2>before breadcrumbs</h2>
	<Breadcrumbs />
	<h1>This is where view by locations and places visited</h1>
</div>

<style>
	.places_home {
		color: blue;
		font-size: large;
	}
</style>
