<script>
	import Nav from '../components/Nav.svelte';
	import Footer from '../components/Footer.svelte';
	import { stores } from '@sapper/app';
    import GA_G from '../components/GA_G.svelte';
    import GA_UA from '../components/GA_UA.svelte';

	export let segment;
</script>

<style>
	main {
		margin-top: 6vh;
    	max-width: 70em;
	}
</style>

<GA_G />
<GA_UA />
<Nav {segment}/>

<body class="bg-gradient-to-br from-blueGray-50 to-white">
	<main class="absolute mx-auto pb-16 shadow-md bg-white rounded-b-lg">
		<slot></slot>
	</main>
</body>

<Footer />
