<script>
	import Hero from '../components/Hero.svelte';
	import ContentBox from '../components/ContentBox.svelte';
	import Card from '../components/Card.svelte';
</script>

<svelte:head>
  <title>Showcase</title>
</svelte:head>

<div class="w-4/5 mx-auto py-4">
	<ContentBox
		title="Here is some of my previous work"
		text="Nothing fancy on the coding side, it's all WordPress so very limited. But it's those very limits that made me want to dig further and learn modern javascript frameworks to rebuild them all."
	/>
	
	<Card
		title="Yumiwork"
		text="There isn't much in terms of functionality but it's easy to navigate, has a funky style, it was a fun one to build from groudn to bottom (logo and colour range as well)."
		link="https://www.yumiwork.com"
	/>

	<Card
	title="Raise"
	text="WordPress plug-ins again, in a different more classically elegant style, with a tropical twist. The logo is my own work as well"
	link="https://www.raise-vanuatu.com"
	/>

	<ContentBox
		title="Svelte component for this website"
		code="{`
		<script>
			export let title;
			export let thumbnail;
			export let text;
			export let code;
			export let quote;
			export let info;
			export let author;
			export let bio;
		</script>

		<div class="py-2 px-0">
			{#if title}
				<h3 class="py-6 text-center text-2xl text-lightBlue-800">{@html title}</h3>
			{/if}
			<div class="">
				{#if thumbnail}
					<img src={thumbnail} alt={thumbnail} class="w-1/3 float-left mr-2 mb-2 rounded-lg">
				{/if}        
				{#if text}
					<p class="text-coolGray-600 text-lg">{@html text}</p>
				{/if}
				{#if code}
					<div class="my-4 py-4 px-6 border-l-2 border-amber-500 bg-warmGray-50 text-amber-600 shadow-sm">
						<pre>
							<code>
								{code}
							</code>
						</pre>
					</div>
				{/if}
			</div>
			{#if quote}
				<div class="my-4 pb-2 px-6 rounded border-l-4 border-lightBlue-700 bg-blueGray-100 shadow-md">
					{#if info}
						<h6 class="font-bold text-lightBlue-900">{info}</h6>
					{/if}
						<p class="text-blueGray-700 py-4">{quote}</p>
					{#if author}
						<p class="text-right text-lightBlue-800">{author}</p>
					{/if}        
					{#if bio}
						<p class="text-right text-blueGray-500">{bio}</p>
					{/if}
				</div>
			{/if}
		</div>
		`}"	
	/>

	<ContentBox
		text="I'm pretty happy about this, because it's rather short in terms of code and it contains almost all the building blocks of this website. It's simple, streamlined, yet allows multiple options for displaying elements. It's the kind of design ethos I'd like to bring. Easy and versatile, empowering users."
	/>

</div>