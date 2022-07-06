<!-- ===================
	COMPONENT JS - BASIC 
=================== -->
<script>
	//	import DefaultPage from '$lib/components/default/default.svelte';
	// import { Default } from '$lib/components/default/default.svelte';
	import contentJson from '$lib/content_en.json';
	import '../styles/global.css';

	let content_en = contentJson;
</script>

<!-- ===================
	COMPONENT HTML 
=================== -->
<top>
	<div id="cool"><p /></div>
</top>
<main>
	<div id="content" />
	<div id="awesome">
		<!-- svelte-ignore a11y-img-redundant-alt -->
		<div id="logo_metafund">
			<a href="https://metafund.vision" target="_blank">
				<img src="/assets/img/metafund_logo.svg" alt="MetaFund Logo" width="170" height="32" /></a
			>
		</div>
		<div>
			<h1>{content_en.title}</h1>
		</div>
		<div>
			<text1>{content_en.subtitle}</text1>
		</div>
		<div id="github_button">
			<a href="https://github.com/M-TAFUND" target="_blank"
				><img src="/assets/img/github_button.svg" alt="Github Logo" width="153" height="48" /></a
			>
		</div>
	</div>
	<div id="satisfied"><p /></div>
	<div id="sad"><div id="logo_cover" /></div>
	<div id="happy" />
</main>

<!-- ===================
	COMPONENT STYLE  
=================== -->
<style>
	:root {
		background-color: #191032;
	}

	top #cool {
		min-height: 220px;
		max-height: 500px;
		order: 1;
		flex-grow: 1;
	}

	h1 {
		color: white;
		text-align: left;
	}

	text1 {
		color: white;
	}

	main {
		overflow: hidden;
		display: flex;
		flex-direction: row;
		justify-content: space-around;
	}

	#content {
		order: 1;
		flex-grow: 1;
		min-height: 820px;
		max-height: 1000px;
		min-width: 220px;
		max-width: 340px;
	}

	#awesome {
		order: 2;
		flex-grow: 1;
		min-width: 262px;
		max-width: 600px;
		padding-top: 6%;
	}

	#logo_metafund {
		margin-bottom: 70px;
	}

	#github_button {
		margin-top: 50px;
	}

	#satisfied {
		order: 3;
		flex-grow: 1;
		min-width: 120px;
		max-width: 160px;
	}

	#logo_cover {
		height: 100%;
		background-image: url('/assets/img/metafund_logo_cover.svg');
		background-position: right 80px top 0px;
		background-repeat: no-repeat;
		background-size: 150%;
	}

	#sad {
		order: 4;
		flex-grow: 10;
		min-width: 424px;
		max-width: 540px;
		/* Gradient/VioletGradient */

		background: linear-gradient(180deg, #5722c9 0%, #8653f4 100%);
	}

	#happy {
		order: 5;
		flex-grow: 10;
		min-width: 220px;
		max-width: 340px;
	}

	/* DESKTOP RESOLUTIONS */

	@media only screen and (min-width: 500px) and (max-width: 1550px) {
		#logo_cover {
			background-position: right -160px top -160px;
			background-repeat: no-repeat;
			background-size: auto;
		}
	}
</style>
