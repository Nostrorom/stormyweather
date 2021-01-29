<script>
    export let link;
    export let name;
</script>

{#if link}
<div class="flex justify-center items-center my-8">
    <div class="items-center rounded-full pt-2 pb-1 pl-4 pr-3 uppercase text-amber-500 bg-gray-100 shadow hover:bg-amber-500 hover:text-white hover:shadow-lg">
        <a target="_blank"  href={link}>{name}</a>
        <svg class="w-6 pb-1 inline-block" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 9l3 3m0 0l-3 3m3-3H8m13 0a9 9 0 11-18 0 9 9 0 0118 0z" />
        </svg>
    </div>
</div>
{/if} 