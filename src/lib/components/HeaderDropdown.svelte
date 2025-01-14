<script>
	import { afterUpdate, beforeUpdate } from "svelte";
    export let content;
    let show;
    
    beforeUpdate(() => {
        show = content!=null
    })
</script>

<div id="header-dropdown"  class="bg-gvss-dmaroon fixed top-20 left-0 w-full z-50 transition-all duration-250 delay {show?"h-[calc(100vh-5rem)] opacity-100":"h-0 opacity-0"} flex gap-10">
    <div class="w-1/4 flex flex-col justify-start pl-2 py-4">
        {#if content}
            {#each content["links"] as link}
                <div class="flex justify-end">
                    <a class="text-5xl text-right text-white hover:text-gvss-lyellow transition-colors duration-200 active:text-gvss-dyellow" href="{link["link"]}">{link["title"]}</a>
                </div>
            {/each}
        {/if}
    </div>
    <div class="w-3/4 bg-cover" style="background-image:url(/images/meeting.jpg)">
    </div>
</div>  