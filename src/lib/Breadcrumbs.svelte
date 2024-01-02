<script>
	export let items = [];
</script>

<div style="font-size: large; color: blueviolet;">in breadcrumbs</div>
<nav aria-label="breadcrumb">
	<ul class="breadcrumb">
		{#each items as item, i}
			<li class="breadcrumb-item">
				{#if item.href}
					<a href={item.href}>{item.text}</a>
				{:else}
					<span>{item.text} Crumb Text</span>
				{/if}
			</li>
			{#if i !== items.length - 1}
				<li class="breadcrumb-item separator">..</li>
			{/if}
		{/each}
	</ul>
</nav>

<style>
	.breadcrumb {
		display: flex;
	}
	.breadcrumb-item {
		color: black;
		font-size: medium;
	}
	breadcrumb-item separator {
	}
</style>
