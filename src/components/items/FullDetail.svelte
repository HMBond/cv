<script>
	const { title, subtitle, link, dates, location, description, list } = $$props;
	let linkDetail = { text: link };
	let locationDetail = { text: location };
</script>

<div class="full-detail detail-container">
	<div class="bottom">
		{#if description}
			<div class="description">
				{@html description}
			</div>
		{/if}
		{#if list}
			<ul class="list">
				{#each list as listItem}
					<li class="list-item">
						{@html listItem}
					</li>
				{/each}
			</ul>
		{/if}
	</div>
</div>

<style>
	.description {
		white-space: pre-line;
	}
</style>
