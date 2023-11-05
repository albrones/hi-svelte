<script>
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
	import ResumeLine from './ResumeLine.svelte';
	import ResumeLineDetail from './ResumeLineDetail.svelte';
	import resumeData from './resumeData.json';

	const data = resumeData;
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Alexis Brones website" />
</svelte:head>

<h1>
	<span class="page-title">Alexis Brones Resume</span>
</h1>
<h2>Fullstack developer / Scrum Master / Responsible digital - SIT</h2>
<section>
	<h2>Experiencies</h2>
	<div>
		<ResumeLine
			enterprise={'Zenika'}
			position={'Consultant Dev. Fullstack, Agility & GreenIT'}
			period={'Jan. 2018 - Today'}
		/>
	</div>
	<div>
		{#each data as item}
			<ResumeLine
				enterprise={item.enterprise}
				position={item.position}
				team={item.team}
				period={item.period}
			>
				<ResumeLineDetail description={item.description} stack={item.stack} tags={item.tags} />
			</ResumeLine>
		{/each}
	</div>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: left;
		align-items: left;
		flex: 0.2;
	}
</style>
