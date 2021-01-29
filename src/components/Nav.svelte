<script>

	const handleClick = () => {
		console.log('123')
		console.log('123')
	}

	export let segment;

</script>

<style>
	nav {
		height: 6vh;
	}
	.navItems {
		max-width: 70em;
	}
	a.current {
		color: white;
	}
</style>

<nav class="flex fixed top-0 z-30 w-screen bg-gradient-to-l from-indigo-900 via-lightBlue-700 to-cyan-600">
	<div class="w-full mx-auto navItems flex items-center justify-between">
		<div on:click={handleClick} class="flex items-center">
				<img src="highseas-blue.svg" alt="highseas logo" class="inline-block h-8 p-1">
				<p class="inline-block ml-2 pb-1 text-white text-2xl md:text-3xl font-light">highseas</p>
		</div>
		<div class="inline-block align-right">
			<a rel=prefetch class="px-0 font-xs sm: font-sm md:px-4 md:font-base xl:px-6 text-amber-400 hover:text-yellow-300 uppercase inline-block" class:current={segment === undefined} href=".">introduction</a>
			<a rel=prefetch class="px-0 font-xs sm: font-sm md:px-4 md:font-base xl:px-6 text-amber-400 hover:text-yellow-300 uppercase inline-block" class:current={segment === "tailwind"} href="tailwind">tailwind</a>
			<a rel=prefetch class="px-0 font-xs sm: font-sm md:px-4 md:font-base xl:px-6 text-amber-400 hover:text-yellow-300 uppercase inline-block" class:current={segment === "showcase"} href="showcase">showcase</a>
			<a rel=prefetch class="px-0 font-xs sm: font-sm md:px-4 md:font-base xl:px-6 text-amber-400 hover:text-yellow-300 uppercase inline-block" class:current={segment === "analysis"} href="analysis">analysis</a>
		</div>
	</div>
</nav>
