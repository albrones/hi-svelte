<script>
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
	import ResumeLine from './ResumeLine.svelte';
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
		<ResumeLine enterprise={'Hellowork'} position={'Tech Lead'} period={'Jan. 2018 - Today'} />
	</div>
	<div>
		<ResumeLine
			enterprise={'Hellowork'}
			position={'Tech Lead'}
			team={'Seekube Squad'}
			period={'Oct. 2023 - Today'}
		/>
		<ResumeLine
			enterprise={'HelloAsso'}
			position={'Front-end Developer'}
			team={'Plateform Squad'}
			period={'Jan. 2023 - Sept. 2023'}
		/>
		<ResumeLine
			enterprise={'PlayPlay'}
			position={'Front-end Developer'}
			team={'Katana Squad'}
			period={'May 2022 - Jul. 2023'}
		/>
		<ResumeLine
			enterprise={'Splio'}
			position={'Front-end Developer'}
			team={'Marketing Automation Squad'}
			period={'May 2021 - May 2022'}
		/>
		<ResumeLine
			enterprise={'ManoMano'}
			position={'Back-end Developer'}
			team={'Seller-Order Squad'}
			period={'Jul. 2020 - Apr. 2021'}
		/>
		<ResumeLine
			enterprise={'DSI Pôle Emploi'}
			position={'Scrum Master'}
			team={'Mon Portefeuille Squad'}
			period={'Jan. - Mar. 2020'}
		/>
		<ResumeLine
			enterprise={'Fatec Group'}
			position={'Front-end Developer & Scrum Master'}
			team={'Starfleet Squad'}
			period={'Dec. 2018 - Jan.2020'}
		/>
		<ResumeLine
			enterprise={'Dotic'}
			position={'Fullstack Developer'}
			team={'Connect-Control Squad'}
			period={'Jul. - Nov. 2018'}
		/>
		<ResumeLine
			enterprise={'SQLi - La Banque Postale'}
			position={'Front-end Developer'}
			team={'Q4Q Squad'}
			period={'Jan. - Jun. 2018'}
		/>
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
	section > div {
		/* display: flex;
		flex-direction: row;
		align-items: center; */
	}

	h1,
	ul {
		width: 100%;
	}
</style>
