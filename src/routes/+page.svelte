<script>
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
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
		<h3 class="left">Consultant at Zenika</h3>
		<div class="line" />
		<h3 class="right">Jan. 2018 - Today</h3>
	</div>
	<div>
		<ul>
			<li>
				<div class="left"><b>Hellowork</b> - Tech Lead on <b>Seekube Squad</b></div>
				<div class="line" />
				<div class="right">Oct. 2023 - Today</div>
			</li>
			<li>
				<div class="left"><b>HelloAsso</b> - Front-end Developer on <b>Plateform Squad</b></div>
				<div class="line" />
				<div class="right">Jan. 2023 - Sept. 2023</div>
			</li>
			<li>
				<div class="left"><b>PlayPlay</b> - Front-end Developer on <b>Katana Squad</b></div>
				<div class="line" />
				<div class="right">May 2022 - Jul. 2023</div>
			</li>
			<li>
				<div class="left">
					<b>Splio</b> - Front-end Developer on <b>Marketing Automation Squad</b>
				</div>
				<div class="line" />
				<div class="right">May 2021 - May 2022</div>
			</li>
			<li>
				<div class="left"><b>ManoMano</b> - Back-end Developer on <b>Seller-Order Squad</b></div>
				<div class="line" />
				<div class="right">Jul. 2020 - Apr. 2021</div>
			</li>
			<li>
				<div class="left">
					<b>DSI Pôle Emploi</b> - Scrum Master on <b>Mon Portefeuille Squad</b>
				</div>
				<div class="line" />
				<div class="right">Jan. - Mar. 2020</div>
			</li>
			<li>
				<div class="left">
					<b>Fatec</b> - Front-end Developer & Scrum Master on <b>Starfleet Squad</b>
				</div>
				<div class="line" />
				<div class="right">Dec. 2018 - Jan.2020</div>
			</li>
			<li>
				<div class="left"><b>Dotic</b> - Fullstack Developer on <b>Connect-Control Squad</b></div>
				<div class="line" />
				<div class="right">Jul. - Nov. 2018</div>
			</li>
			<li>
				<div class="left">
					<b>SQLi - La Banque Postale</b> - Front-end Developer on <b>Q4Q Squad</b>
				</div>
				<div class="line" />
				<div class="right">Jan. - Jun. 2018</div>
			</li>
		</ul>
	</div>
	<ul />
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: left;
		align-items: left;
		flex: 0.2;
	}
	section > div,
	li {
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

	h1,
	ul {
		width: 100%;
	}
</style>
