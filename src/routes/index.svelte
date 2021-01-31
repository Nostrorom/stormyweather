<script>
	import Hero from '../components/Hero.svelte';
	import ContentBox from '../components/ContentBox.svelte';
	import Card from '../components/Card.svelte';
</script>

<svelte:head>
  <title>Intro</title>
</svelte:head>

<Hero
	title="highseas"
	subtitle="the little app that went way overboard"
/>

<div class="w-4/5 mx-auto py-6">

	<ContentBox
		title="Hi ! And welcome to <em>highseas</em>, the application that turned into an application..."
		text="It started as a job application for an open position at Tailwind, that I named Highseas. I ran short of time to properly do all what I wanted, so I made a copy to continue my work.

		It has now evolved into a personal project in this repo called Sotrmyweather. Yeah, I'm not one to let go of a good sailing metaphor ;) 
		
		It's now both a sandbox to practise the tools, and an end-result offering thoughts on them, mainly Tailwind to start with."	
	/>

	<ContentBox
		title="Tools used"
		text="This is built with:

		* Svelte + Sapper
		* Tailwindcss
		
		I'll be updating it with a data visualization tool, probably one of: 
		
		* D3js
		* Chartjs"
	/>

</div>





