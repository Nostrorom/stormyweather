<script>
	import ContentBox from '../components/ContentBox.svelte';
	import GridCard from '../components/GridCard.svelte';
</script>

<svelte:head>
  <title>HS - Portfolio</title>
</svelte:head>

<div class="w-4/5 mx-auto py-4">

	<ContentBox
		title="Design work"
		text="Websites and logos designed by yours truly."
	/>

    <div class="mt-10">
        <dl class="space-y-10 md:space-y-0 md:grid md:grid-cols-2 md:gap-x-8 md:gap-y-10">

            <GridCard 
                image="logo_ymw.png"
                title="yumiwork"
                text="Vanuatu's first coworking space."
            />
            
            <GridCard 
                image="logo_kw.png"
                title="Kava World"
                text="A scocial network around kava, a locla traditonal drink."
            />           

            <GridCard 
                image="logo_raise_rect.png"
                title="Raise"
                text="Vanuatu's first crowdfunding platform."
            />

            <GridCard 
                image="logo_gpsv.png"
                title="GPS Vanuatu"
                text="Installing tracking devices."
            />

        </dl>
    </div>
</div>  