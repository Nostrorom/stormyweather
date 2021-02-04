<script>
	let innerWidth;
  	$: showMenu = innerWidth >= 1024;
	
	const toggleMenu = () => {
		showMenu = !showMenu;
	}

	export let segment;
</script>

<svelte:window bind:innerWidth />

<style>
	nav {
		height: 6vh;
	}
	.navItems {
		max-width: 70em;
	}
</style>


<nav class="flex fixed top-0 z-30 w-screen mb-0 flex-wrap items-center justify-between px-2 py-3 navbar-expand-lg bg-gradient-to-l from-indigo-900 via-lightBlue-700 to-cyan-600">
	<div class="container navItems px-4 mx-auto flex flex-wrap items-center justify-between">
	  <div class="w-full relative flex justify-between lg:w-auto px-4 lg:static lg:block lg:justify-start">
		<a sapper:prefetch class="flex cursor-pointer items-center" href=".">
			<img src="highseas-blue.svg" alt="highseas logo" class="inline-block h-8 p-1">
			<p class="inline-block ml-2 pb-1 text-white text-2xl md:text-3xl font-light">highseas</p>			
		</a>
		<button on:click={toggleMenu} class="cursor-pointer leading-none h-8 py-1 ml-8 block lg:hidden focus:outline-none text-amber-400 align-right" type="button">
			<svg class="h-full" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
				<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
			</svg>
		</button>
	  </div>
	  <div class="lg:flex flex-grow items-center justify-end">
		<ul class="flex flex-col lg:flex-row list-none ml-auto text-right" class:hidden={showMenu === false}>
			<li class="text-amber-400">
				<a sapper:prefetch class="rounded-md p-1 font-xs sm:font-sm md:px-4 md:font-base xl:px-6 hover:text-yellow-200 hover:bg-blue-900 hover:bg-opacity-60 focus:bg-lightBlue-700 focus:bg-opacity-80 uppercase inline-block focus:outline-none" class:text-yellow-200={segment === undefined} href=".">Home</a>
			</li>
			<li class="text-amber-400">
				<a sapper:prefetch class="rounded-md p-1 font-xs sm:font-sm md:px-4 md:font-base xl:px-6 hover:text-yellow-200 hover:bg-blue-900 hover:bg-opacity-60 focus:bg-lightBlue-700 focus:bg-opacity-80 uppercase inline-block focus:outline-none" class:text-yellow-200={segment === "tailwind"} href="tailwind">tailwind</a>
			</li>
			<li class="text-amber-400">
				<a sapper:prefetch class="rounded-md p-1 font-xs sm:font-sm md:px-4 md:font-base xl:px-6 hover:text-yellow-200 hover:bg-blue-900 hover:bg-opacity-60 focus:bg-lightBlue-700 focus:bg-opacity-80 uppercase inline-block focus:outline-none" class:text-yellow-200={segment === "analysis"} href="analysis">Color palette analysis</a>
			</li>
		</ul>
	  </div>
	</div>
  </nav>
