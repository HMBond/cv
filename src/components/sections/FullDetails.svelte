<script>
	import FullDetail from '../items/FullDetail.svelte';
	export let details;
</script>

<div>
	{#each details as { ...props }}
		<FullDetail {...props} />
	{/each}
</div>
