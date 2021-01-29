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
		text="So one day, I was perusing the Tailwind documentation to build a website and an app that inspires me, and this led me to here.
		As a preamble, let me kindly suggest that this quote: "	
	/>
	<ContentBox
		quote="[...] we're a tiny company so we need T-shaped people more than we need specialists."
		author="Adam W."
		bio="somebody you may have heard of"
	/>

	<ContentBox
		text="...is going ot be put seriously to the test. It's this one and a similar tone that convinced my to apply. In my case, we're talking more of a squashed T, with quite a wide horizontal bar and rather shorter vertical one. I have no doubt that there will be more experienced or skilled designers applying, that's not where my strengths lie. It's in the breadth of interests, the quickness and eagerness to learn, discover, explore each and eveything that may come my way."	
	/>

	<ContentBox
		text="So without further ado, here is how this site is organised:"
	/>

	<Card
		title="Introduction"
		text="This section right here, where I talk about stuff that I find relevant, past or future experiences. This is not a resume, there's LinkedIn for that ;)"
	/>
	
	<Card
		title="Tailwind"
		text="Where I give my thoughts on what was posted in the job description. Maybe not on everything, and some I talk more lengthily about. Some things inspires me, what I'd look forward to work on, etc. Sidenote: I may have found a mistake in a Tailwind UI element (teaser, hah hah !)."
		link="tailwind"
	/>
	
	<Card
		title="Showcase"
		text="You'll quickly realise that my previous work is not expert-level, but that does give a sense of the progression. 2 years ago, I had never written a single line of code (apart a vague attempt at an tabletop game website in 1999), and it's the frustration with the limits of the technology I was using as well as my own skills that landed me here. There are two things that really enthuse me, it's Svelte and Tailwind: simple, clean, elegant, flexible. My best work so far is the very website you are looking at. It's also the very first app I deploy. And the first one I built with Svelte/Sapper. And the first one I used Tailwind on. I expand a bit on the parts am the more happy with."
		link="showcase"
	/>
	
	<Card
		title="Analysis"
		text="If there's one feature I'd really like to see in Tailwind, it's the possibility to generate your own palette. I mean, the palette is beautiful, for sure, but you know how that goes: people will always want <em>that particular hue</em> and it's variants. Sometime you work on a brand with a given color, or there's one you really like, all sorts of reasons really. So I got thinking into how that could work."
		link="analysis"
	/>

	<ContentBox
		title="Last minute uneforeseen issues"
		text="So as these things always do, deployment bailed on me at the last minute. I tried to troubleshoot but didn't succeed. <code>npm run dev</code> works fine, Heroku gives success messges, but somehow I can't access the app."	
	/>

	<ContentBox
		text="That means this section is going to remain pretty empty, as I'll try to publish as much content as I can in the meantime, and the content is going to remain a bit flimsier than I would have liked. In the interest of fairness for other applicants, I'll stop modifying the repo at deadline time."	
	/>

	<ContentBox
		text="Let me just try to recap that I am very ethusiastic about Tailwind and the possibilities it brings to web development. Being a part of it would be a very exciting prospect for me. And while I am not the most skilled or experiences, I have a wide variety of experience and skills that cna bring a fresh eye and a different angle to many things that you guys do. I'm endlessly curious and learn very fast, any sort of things. Science, languages (I can hold a conversation in about 6/7), travel (visited about 80 countries, and counting), history, you name it."	
	/>

	<ContentBox
		text="Friends and colleagues usually praise my knowledge of many subjects, and my eagerness to keep learning more, my analytical mind that understands concepts easily, my kindness and human skills that make me a great teacher as well and a fun person to be around."	
	/>	

	<ContentBox
		text="What is in this website is just the surface of the work I've done for this application, and also of what I think I can bring to Tailwind. I hope there is enough to pique your curiosity and that we may have the opportunity to talk to go further :)"	
	/>	

</div>





