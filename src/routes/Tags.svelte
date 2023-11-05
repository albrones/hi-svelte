<script lang="ts">
	import Tag from './Tag.svelte';

	export let data: string[] = [];
</script>

<p class="resume-line-tags">
	{#each data as item}
		<Tag name={item} />
	{/each}
</p>

<style>
	.resume-line-tags {
		display: flex;
	}
</style>
