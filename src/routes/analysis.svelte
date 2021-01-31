<script>
	import ContentBox from '../components/ContentBox.svelte';
	import Card from '../components/Card.svelte';
</script>

<svelte:head>
  <title>Analysis</title>
</svelte:head>

<div class="w-4/5 mx-auto py-4">
	<ContentBox
		title="Choice of color range for analysis"
		text="While <code>RGB/Hex</code> seems natural for developpers to look at, it is not a very easy to apprehend as an end-user looking at the color. While we may have a rough idea of how a color evolves if we change values by 10 or 20, it's harder to really guess if you do + or - 50 on all dimensions for example."
	/>

	<ContentBox
		text="<code>HSL</code> is much easier to grasp from a human perspective, if you are just a bit familira with it you can pretty easily guess a color by looking at the a <code>HSL</code> value, or how it would look if you change some parameters."
	/>
	
	<ContentBox
		text="As with any assumption, it's still needs to be tested to be discarded. A cursory <code>RGB</code> analysis did indeed not provide much insight into how the colors relate to each other."
	/>

	<ContentBox
		title="Color-500 as a point of reference"
		text="In many cases, we need some point of refrence to see the different values changing throughout teh range, and also to provide and easy entry to compare different hues. The <code>500</code> value is what you could describe as the 'main' color, of which teh rest are tints and shades. Before the introduction of the <code>50</code> value it also was the middle point. The choice is arbitrary but seems the most logical."
	/>

	<ContentBox
		title="Hue curves"
		text="By looking at the raw data, it's easy to see that apart from <code>Red</code> which is fully flat, all other colors have some sort of progression through the range. Plotting the curves should show if this progression is more or less linear."
	/>

	<Card
		title="Hue curves"
		image="hue_curves.png"
	/>

	<ContentBox
		text="We can see a group that has descending <code>H</code> value throughout the range, roughly in the <code>350-50</code> band, that we could describe as 'warm' colors, from <code>Rose</code> to <code>Yellow</code>, with the only outlier being <code>Red</code>. The rest of the colors have a mostly ascending curve."
	/>

	<ContentBox
		text="To better compare the slopes, let's plot them together with <code>color-500</code> as the reference <code>H</code> value, the others being noted as the difference."
	/>

	<Card
		title="Hue curves compared to Color-500"
		image="hue_d500.png"
	/>

	<ContentBox
		text="Seems to confirm the first view. Let's zoom in to see better."
	/>

	<Card
		title="Hue curves compared to Color-500"
		image="hue_d500_exp.png"
	/>

	<ContentBox
	text=""
	/>

	<Card
		title="Saturation curves"
		image="sat_curves.png"
	/>

	<ContentBox
	text=""
	/>

	<Card
		title="Saturation curves compared to Color-500"
		image="sat_d500.png"
	/>

	<ContentBox
	text=""
	/>

	<Card
		title="Lightness curves"
		image="light_curves.png"
	/>

	<ContentBox
	text=""
	/>

	<Card
		title="Lightness curves compared to Color-500"
		image="light_d500.png"
	/>

	<ContentBox
	text=""
	/>

</div>