<script>
    export let image;
    export let title;
    export let text;
</script>

<div class="flex">
    <div class="flex-shrink-0">
        <div class="flex items-center justify-center h-40 w-40 rounded-lg shadow-md overflow-hidden">
            <img src={image} alt={image} class="overflow-hidden"> 
        </div>
    </div>
    <div class="ml-4">
        <dt class="text-lg leading-6 font-medium text-lightBlue-800">
            {title}
        </dt>
        <dd class="mt-2 text-base text-coolGray-600">
            {@html text}
        </dd>
    </div>
</div>