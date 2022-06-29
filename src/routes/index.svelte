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
	<div id="content"><h1 class="mainTitle">{content_en.title}</h1></div>
	<div id="sad"><p>Sad</p></div>
	<div id="confused"><p>Confused</p></div>
</main>

<!-- ===================
	COMPONENT STYLE  
=================== -->
<style>
	:root {
		background-color: #191032;
	}

	.mainTitle {
		color: white;
	}

	main {
		display: flex;
		flex-direction: row;
		justify-content: space-around;
		text-align: center;
	}

	#content {
		order: 2;
		flex-grow: 1;
	}

	#sad {
		order: 3;
		flex-grow: 10;
	}
</style>
