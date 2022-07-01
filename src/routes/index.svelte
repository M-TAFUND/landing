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

<main>
	<div id="content">
		<div class="contentDivLeft">
			<!-- svelte-ignore a11y-img-redundant-alt -->
			<img src="/assets/img/metafund_logo.svg" alt="MetaFund Logo" width="170" height="32" />
			<h1>{content_en.title}</h1>
			<text1>{content_en.subtitle}</text1>
		</div>
	</div>
	<div id="sad"><p>Sad</p></div>
</main>

<!-- ===================
	COMPONENT STYLE  
=================== -->
<style>
	:root {
		background-color: #191032;
	}

	.contentDivLeft {
		padding: 400px;
		width: 1350px;
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
		order: 1;
		flex-grow: 1;
	}

	#sad {
		order: 2;
		flex-grow: 10;
	}
</style>
