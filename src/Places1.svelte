<script>
	import Breadcrumbs from './lib/Breadcrumbs.svelte';
	import Counter from './lib/Counter.svelte';
	const items = [
		{ text: 'Home', href: '/' },
		{ text: 'Projects', href: '/projects' },
		{ text: 'Svelte Breadcrumb' },
	];

	// console.log('In Breadcrumbs');
</script>

<div class="places_home">
	<h2>before breadcrumbs</h2>

	<h1>This is where view by locations and places visited</h1>

</div>
<style>
	.places_home {
		color: blue;
		font-size: large;
	}
</style>