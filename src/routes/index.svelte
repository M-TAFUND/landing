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

<h1 class="mainTitle">{content_en.title}</h1>

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
</style>
