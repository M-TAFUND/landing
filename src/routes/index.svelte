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
	<a id="cool"><p /></a>
</top>
<main>
	<div id="content">
		<!-- svelte-ignore a11y-img-redundant-alt -->
		<img src="/assets/img/metafund_logo.svg" alt="MetaFund Logo" width="170" height="32" />
		<h1>{content_en.title}</h1>
		<text1>{content_en.subtitle}</text1>
	</div>
	<div id="sad"><p /></div>
	<div id="happy" />
</main>

<!-- ===================
	COMPONENT STYLE  
=================== -->
<style>
	:root {
		background-color: #191032;
	}

	top a#cool {
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
		display: flex;
		flex-direction: row;
		justify-content: space-around;
	}

	#content {
		padding: 400px;
		max-width: 1400px;
		order: 1;
		flex-grow: 1;
	}

	#sad {
		margin-top: 180px;
		order: 2;
		flex-grow: 10;
		/* Gradient/VioletGradient */

		background: linear-gradient(180deg, #5722c9 0%, #8653f4 100%);
	}

	#happy {
		margin-left: -100px;
		order: 3;
		flex-grow: 10;
	}
</style>
