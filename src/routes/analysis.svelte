<script>
	import ContentBox from '../components/ContentBox.svelte';
	import Card from '../components/Card.svelte';
</script>

<svelte:head>
  <title>Analysis</title>
</svelte:head>

<div class="w-4/5 mx-auto py-4">
	<ContentBox
		title="Anlysing the color palette of Tailwind 2.0"
		text="The idea was to use the HSL data points on all of the colors to try to find a function that could be applied to other colors in between.
		HSL was chosen because it makes sense on a human-perception perspective to determine what works. You will find below some samples. The end insight is that the curves have enough similarities to allow such a function to be calculated, and could generate the current palette with the exception of a couple outliers here and there, but that woudl not statistically change the result"
	/>

	<Card
		title="Hue curves"
		image="hue_curves.png"
	/>

	<ContentBox
	text=""
	/>

	<Card
		title="Hue curves compared to Color-500"
		image="hue_d500.png"
	/>

	<ContentBox
	text=""
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