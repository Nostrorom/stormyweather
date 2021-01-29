<script>
    export let title;
    export let text;
    export let image;
    export let thumbnail;
    export let link;
</script>

<div class="my-4 py-6 rounded-lg shadow-lg overflow-hidden bg-gradient-to-tr from-white to-coolGray-50">
    {#if title}
        <h4 class="pb-4 text-center text-lg text-amber-600">{title}</h4>
    {/if}
    {#if image}
        <img src={image} alt={image} class="w-full">
    {/if}
    {#if thumbnail}
        <img src={thumbnail} alt={thumbnail} class="w-1/3 float-left mr-2 mb-2 rounded-lg">
    {/if}   
    {#if text}
        <p class="text-coolGray-600 text-md px-8">{@html text}</p>
    {/if}
    {#if link}
    <div class="flex justify-center items-center mt-4">
        <a target="_blank" href={link} class="items-center rounded-full p-2 pb-1 uppercase text-amber-500 bg-gray-100 shadow hover:bg-amber-500 hover:text-white hover:shadow-lg">
            <svg class="w-6 pb-1 inline-block" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 9l3 3m0 0l-3 3m3-3H8m13 0a9 9 0 11-18 0 9 9 0 0118 0z" />
            </svg>
        </a>
    </div>
    {/if} 
</div>