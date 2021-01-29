<script>
    export let title;
    export let subtitle;
</script>

<style>

</style>

<div class="relative"> 
	<div class="max-w-7xl mx-auto">
	  	<div class="flex relative z-10 mx-6 pb-8 sm:pb-16 md:pb-20 lg:max-w-2xl lg:w-full lg:pb-28 xl:pb-32">
			<svg class="hidden lg:block absolute right-0 inset-y-0 h-full text-white transform translate-x-1/2 " fill="white" viewBox="0 0 100 100" preserveAspectRatio="none" aria-hidden="true">
				<polygon points="0,0 100,0 50,100 0,100" />
			</svg>
			<div class="mt-10 mx-auto max-w-7xl px-4 sm:mt-12 sm:px-6 md:mt-16 lg:mt-20 lg:pl-8 lg:pr-0 xl:mt-28">
				<div class="relative z-20 text-center lg:text-left">
					<h1 class="text-5xl font-light text-lightBlue-800 sm:text-6xl md:text-7xl lg:text-9xl">
						{title}
					</h1>
					<p class="pl-1.5 pt-2 mt-3 text-base text-blueGray-400 sm:mt-5 sm:text-lg sm:max-w-xl sm:mx-auto md:mt-5 md:text-xl lg:text-3xl lg:mx-0">
						{subtitle}
					</p>
					<div class="mt-5 sm:mt-8 sm:flex sm:justify-center lg:justify-start">
						<div class="mt-3 sm:mt-0 sm:ml-3">
							<img src="arnaud.png" alt="arnaud" class="inline-block w-32 rounded-full shadow-lg">
							<div class="inline-block ml-4">
								<p class="block text-lg text-lightBlue-800">Arnaud Fouché</p>
								<div class="block">
									<a target="_blank" href="https://github.com/Nostrorom/highseas">
										<img src="github.svg" alt="github" class="inline-block h-6 mx-1 hover:shadow">
									</a>									
									<a target="_blank" href="https://www.linkedin.com/in/arnaud-fouch%C3%A9-4261b56b/">
										<img src="linkedin.svg" alt="linkedin" class="inline-block h-6 mx-1 hover:shadow">
									</a>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
	  	</div>
	</div>
	<div class="lg:absolute max-h-full lg:inset-y-0 lg:right-0 lg:w-1/2 bg-gradient-to-t from-indigo-900 via-lightBlue-700 to-cyan-600">
		<img class="p-6 h-56 w-full object-contain sm:h-72 md:h-96 lg:w-full lg:h-full" src="highseas-white.svg" alt="highseas logo">
	</div>
</div>