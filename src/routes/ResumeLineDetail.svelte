<script lang="ts">
	export let description: string;
	export let stack: string;
</script>

<div class="resume-line-detail">
	<p>{description}</p>
	<p>Stack: {stack}</p>
</div>

<style>
	.resume-line-detail {
		border: solid 0.07em gray;
		margin: 4px;
		padding: 0 1em;
		display: flex;
		flex-direction: column;
		text-align: justify;
	}
	p {
		width: 100%;
	}
</style>
