<script>
    export let title;
    export let thumbnail;
    export let text;
    export let code;
    export let quote;
    export let info;
    export let author;
    export let bio;
</script>

<style>

</style>

<div class="py-2 px-0">
    {#if title}
        <h3 class="py-6 text-center text-2xl text-lightBlue-800">{@html title}</h3>
    {/if}
    <div class="">
        {#if thumbnail}
            <img src={thumbnail} alt={thumbnail} class="w-1/3 float-left mr-2 mb-2 rounded-lg">
        {/if}        
        {#if text}
            <p class="text-coolGray-600 text-lg">{@html text}</p>
        {/if}
        {#if code}
            <div class="my-4 py-4 px-2 border-l-2 border-amber-500 bg-warmGray-50 text-amber-600 shadow-sm">
                <pre>
                    <code>
                        {code}
                    </code>
                </pre>
            </div>
        {/if}
    </div>
    {#if quote}
        <div class="my-4 pb-2 px-6 rounded border-l-4 border-lightBlue-700 bg-blueGray-100 shadow-md">
            {#if info}
                <h6 class="font-bold text-lightBlue-900">{info}</h6>
            {/if}
                <p class="text-blueGray-700 py-4">{quote}</p>
            {#if author}
                <p class="text-right text-lightBlue-800">{author}</p>
            {/if}        
            {#if bio}
                <p class="text-right text-blueGray-500">{bio}</p>
            {/if}
        </div>
    {/if}
</div>