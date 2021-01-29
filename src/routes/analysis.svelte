<script>
	import ContentBox from '../components/ContentBox.svelte';
	import Card from '../components/Card.svelte';
</script>

<svelte:head>
  <title>Analysis</title>
</svelte:head>

<div class="w-4/5 mx-auto py-4">
	<ContentBox
		title="There was so much more to say"
		text="The idea was to use the HSL data points on all of the colors to try to find a function that could be applied to other colors in between.
		HSL was chosen because it makes sense on a human-perception perspective to determine what works. You will find below some samples. The end insight is that the curves have enough similarities to allow such a function to be calculated, and could generate the current palette with the exception of a couple outliers here and there, but that woudl not statistically change the result"
	/>

	<Card
		title="red"
		image="red.png"
	/>
	<Card
		title="lime"
		image="lime.png"
	/>
	<Card
		title="blue"
		image="blue.png"
	/>
	<Card
		title="fuchsia"
		image="fuchsia.png"
	/>
</div>