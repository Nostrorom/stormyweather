<script>
    let innerWidth;
  	$: showMenu = innerWidth >= 1024;

	const toggleMenu = () => {
		showMenu = !showMenu;
	}

	export let segment;
</script>

<svelte:window bind:innerWidth />

<nav class="flex flex-wrap items-center justify-between">
    <button on:click={toggleMenu} class="block lg:hidden" type="button">Button</button>
    <div class="lg:flex flex-grow items-center justify-end">
    <ul class="flex flex-col lg:flex-row text-right" class:hidden={showMenu === false}>
        <li>
            <a href=".">Home</a>
        </li>
        <li>
            <a href="link_A">link_A</a>
        </li>
        <li>
            <a href="link_B">link_B</a>
        </li>
    </ul>
    </div>
</nav>
