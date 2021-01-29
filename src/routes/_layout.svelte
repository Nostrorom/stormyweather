<script>
	import Nav from '../components/Nav.svelte';
	import Footer from '../components/Footer.svelte';
	import { stores } from '@sapper/app';
    import GA from '../components/GA.svelte';

	export let segment;
</script>

<style>
	main {
		margin-top: 6vh;
    	max-width: 70em;
	}
</style>

<GA />
<Nav {segment}/>

<body class="bg-gradient-to-br from-blueGray-50 to-white">
	<main class="relative mx-auto pb-16 shadow-md bg-white rounded-b-lg">
		<slot></slot>
	</main>
</body>

<Footer />
