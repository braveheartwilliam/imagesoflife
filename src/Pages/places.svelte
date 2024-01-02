<script>
	import Breadcrumbs from '../lib/Breadcrumbs.svelte';

	const items = [
		{ text: 'Home', href: '/' },
		{ text: 'Projects', href: '/projects' },
		{ text: 'Svelte Breadcrumb' },
	];

	console.log('In Breadcrumbs');
</script>

<div class="places_home">
	<h2>before breadcrumbs</h2>
	<div>
		<Breadcrumbs {items} />
	</div>
	<h1>This is where view by locations and places visited</h1>
</div>

<style>
	.places_home {
		color: blue;
		font-size: large;
	}
</style>
