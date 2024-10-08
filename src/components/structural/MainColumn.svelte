<script>
	import Section from './Section.svelte';
	export let sections;
</script>

<div class="main-column">
	{#each sections as { label, details, type }}
		<Section {label} {details} {type} />
	{/each}
</div>

<style>
	.main-column {
		width: var(--main-column-width);
		margin: 0 var(--horizontal-space-between-columns);
		display: flex;
		flex-direction: column;
		justify-content: space-between;
	}
</style>
