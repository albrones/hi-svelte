<script lang="ts">
	export let enterprise: string;
	export let position: string;
	export let team: string = '';
	export let period: string;
	let hidden: boolean = true;

	function toggleDetails() {
		hidden = !hidden;
	}
</script>

<div
	class="resume-line"
	on:click={toggleDetails}
	role="button"
	tabindex="0"
	on:keydown|preventDefault={(e) => (e.key === 'o' ? toggleDetails() : () => {})}
>
	{#if team}
		<div>
			<div class="left"><b>{enterprise}</b> - {position} in <b>{team}</b></div>
			<div class="line" />
			<div class="right">{period}</div>
		</div>
		{#if !hidden}
			<div>
				<slot />
			</div>
		{/if}
	{:else}
		<div>
			<h3 class="left"><b>{position}</b> at <b>{enterprise}</b></h3>
			<div class="line" />
			<h3 class="right">{period}</h3>
		</div>
	{/if}
</div>

<style>
	.resume-line {
		border: solid 0.1em gray;
		margin: 4px;
		padding: 4px;
	}
	.resume-line > div {
		display: flex;
		flex-direction: row;
		align-items: center;
	}
	.line {
		border-bottom: 1px dashed grey;
		position: relative;
		width: 100%;
		z-index: -1;
	}
	.left {
		padding-right: 15px;
		max-width: max-content;
		width: 100%;
	}
	.right {
		padding-left: 15px;
		max-width: max-content;
		width: 100%;
		font-weight: bold;
	}
</style>
