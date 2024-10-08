<script>
	export const name = 'Mike Bond';
	const summaryLines = [
		'Full-Stack developer with an affinity for UX. Experienced in working on internal and customer facing applications. Passionate about building reliable software by managing technical depth and writing thoughtfull clean code together in a streamlined team.',
	];
</script>

<div class="header">
	<h1 class="my-name">{name}</h1>
	<div class="summary">
		{#each summaryLines as line, i}
			<div class="summary-line-{i}">
				{@html line}
			</div>
		{/each}
	</div>
</div>

<style>
	.header {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		margin-bottom: var(--vertical-space-between-sections);
	}

	.my-name {
		text-transform: uppercase;
		color: var(--accent-color);
		font-family: var(--accent-font);
		font-size: 3em;
		margin: 0;
	}

	.summary {
		width: 78%;
		margin-top: 5px;
		font-size: 1.05em;
		font-weight: 300;
		font-family: var(--accent-font);
		line-height: 1.5em;
		color: #000;
	}
</style>
