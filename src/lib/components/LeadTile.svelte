<script>
    export let image, title, name, description;
</script>

<div class="w-full h-[50vh] grid grid-cols-2 grid-rows-1 justify-center items-center border-t-2 border-gvss-dgray">
    <div class="w-full h-full flex items-center justify-center">
    <img class="h-5/6 w-auto object-cover rounded border border-gvss-dyellow aspect-square" src="{image}">
    </div>
    <div class="flex flex-col justify-around w-full h-full">
        <div>
        <h3 class="text-6xl font-bold text-gvss-dyellow">{title}</h3>
        <h2 class="text-4xl text-white">{name}</h2>
        </div>
        <p class="text-2xl text-white">{description}</p>
    </div>
</div>