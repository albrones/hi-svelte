<script lang="ts">
	export let name: string;
</script>

<div class={name ? `tag ${name.toLowerCase()}` : 'tag'}>
	{name.toLowerCase()}
</div>

<style>
	.tag {
		border: solid 1px grey;
		border-radius: 16px;
		margin-right: 4px;
		text-align: center;
		padding: 4px;
	}
	.reactjs {
		background-color: blue;
	}
	.nodejs {
		background-color: green;
	}
	.tailwindcss {
		background-color: cyan;
	}
</style>
