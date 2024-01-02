<script>
	import Breadcrumbs from './lib/Breadcrumbs.svelte';

	const items = [
		{ text: 'Home', href: '/' },
		{ text: 'Projects', href: '/projects' },
		{ text: 'Svelte Breadcrumb' },
	];
</script>

<main>
	<div class="HomePage">
		Images of Life xxx
		<div class="grid_container">
			<div class="home_header">home_header <Breadcrumbs {items} /></div>
			<Breadcrumbs {items} />
			<div class="home_left_navigation">
				left_navigation
				<div class="home_nav">
					What do you want to see?
					<nav class="home_left_nav">
						<li class="nav_list">
							<a href="src/Places.svelte">Places</a>
						</li>
						<li class="nav_list">Trips</li>
						<li class="nav_list">Pictures</li>
						<li class="nav_list">People</li>
						<li class="nav_list">Me</li>
					</nav>
				</div>
			</div>
			<div class="home_body">home_body</div>
			<div class="home_right_navigation">right_navigation</div>
			<div class="home_footer">home_footer</div>
		</div>
	</div>
</main>

<style>
	.HomePage {
		width: 100vw;

		background-color: antiquewhite;
	}
	.grid_container {
		display: grid;
		grid-template-columns: 15vw repeat(8, 10vw) 15dvw;
		grid-template-rows: 15rem repeat(6, 15rem) 15rem;
	}
	.home_left_navigation {
		background-color: aquamarine;
		font-size: 25px;
		color: red;
		grid-column: 1/1;
		grid-row: 2/8;
	}
	.home_nav {
		font-size: 25px;
		color: red;
		width: 8rem;
		margin: auto;
		display: flex;
		flex-direction: column;
		text-align: left;
	}

	.home_right_navigation {
		background-color: rgb(49, 108, 177);
		font-size: 25px;
		color: red;
		grid-column: 10/11;
		grid-row: 2/8;
	}
	.home_header {
		background-color: rgb(230, 227, 100);
		font-size: 25px;
		color: red;
		grid-column: 1/11;
		grid-row: 1/1;
	}
	.home_body {
		background-color: rgb(236, 208, 81);
		font-size: 25px;
		color: red;
		grid-column: 2/10;
		grid-row: 2/8;
	}
	.home_footer {
		background-color: rgb(240, 169, 240);
		font-size: 25px;
		color: red;
		grid-column: 1/11;
		grid-row: 8/8;
	}
	.logo:hover {
		filter: drop-shadow(0 0 2em #646cffaa);
	}
	.logo.svelte:hover {
		filter: drop-shadow(0 0 2em #ff3e00aa);
	}
</style>
