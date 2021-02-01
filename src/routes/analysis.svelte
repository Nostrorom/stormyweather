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
		text="Zooming to have a clearer view of the different slopes. We can indeed see that there is a 'warm' group that has a different profile than the others."
	/>

	<Card
		title="Hue curves compared to Color-500"
		image="hue_d500_exp.png"
	/>

	<ContentBox
	text="Now performing a similar plotting of the <code>S</code> values. Already interesting is the fact that apart from a small offset, the curves have a decently recognizable profile throughout the <code>50-900</code> band, which means a pattern can surely be determined in the end."
	/>
	
	<ContentBox
		text="It is already pretty noticeable that the curves depend on the hue range. What we could call 'intense' vs 'soft' colors, i.e. the reds-purples-blues have a lower <code>S</code> value because they are percieved by the human eye as stronger for a given saturation value, so to have the same feel to the eye, the <code>S</code> needs to be a bit lower."
	/>

	<Card
		title="Saturation curves"
		image="sat_curves.png"
	/>

	<ContentBox
	text="Again, plotting against <code>color-500</code> to make comparison easier."
	/>

	<Card
		title="Saturation curves compared to Color-500"
		image="sat_d500.png"
	/>

	<ContentBox
	text="The <code>L</code> values also show curves that follow a comparable pattern, with a similar groupings compared to <code>S</code> curves, though with the yellow-oranges closer to the red-purples than the blue-greens this time."
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
		title="Observing the S and L values depending on the hue range"
		text="The previous curves show that we could extract a pattern for the whole palette, with variations depending on the hue range. A more complete analysis will be necesasry to define rules for each of the <code>50-900</code> variations, but for the sake of example we can look at the <code>500</code> as the 'main' variation, then <code>50</code> and <code>900</code> at both ends."
	/>

	<Card
		title="A cursory look at the gaps in the palette for Color-500"
		image="hh_500.png"
	/>

	<Card
		title="Saturation data for Color-500"
		image="hs_500.png"
	/>

	<Card
		title="Lightness data for Color-500"
		image="hl_500.png"
	/>
	<ContentBox
		text="In both plot charts above, a profile is pretty recognizable: there's a function that can be calculated, which would enable us to generate the <code>S</code> and <code>L</code> values for a given <code>H</code>, thus extending the color palette to any hue a user would like. Though less obvious, patterns can also been seen for the <code>50</code> and <code>900</code> values."
	/>

	<Card
		title="Saturation data for Color-50"
		image="hs_50.png"
	/>

	<Card
		title="Lightness data for Color-50"
		image="hl_50.png"
	/>

	<Card
		title="Saturation data for Color-900"
		image="hs_900.png"
	/>

	<Card
		title="Lightness data for Color-900"
		image="hl_900.png"
	/>

</div>