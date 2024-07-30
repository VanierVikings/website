<script>
    const linkClicked = (event) => {
        const targetButton = event.target.closest(".header-link");
        const links = document.getElementsByClassName("header-link")
        const state = targetButton.dataset.clicked;
        targetButton.dataset.clicked = state=="false"?"true":"false";
        for(const link of links){
            if(link == targetButton){
                continue;
            }
            link.dataset.clicked = false;
        }
    }
</script>

<div class="flex bg-gvss-lmaroon border-b-8 border-gvss-lyellow h-20">
    <div class="flex justify-center items-center w-1/4">
        <img src="/images/logo.png" alt="">
        <h1 class="text-white">Vanier Vikings</h1>
    </div>
    <div class="flex justify-around items-center w-3/4">
        <button on:click={linkClicked} data-clicked="false" class="header-link flex items-center h-full text-white group cursor-pointer">
            <h1 class="after:block after:transition-all after:duration-200 after:relative after:w-0 after:bottom-0 after:left-1/2 after:h-0.5 after:bg-gvss-lyellow group-hover:after:w-full group-hover:after:left-0">
                About Us
            </h1>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="size-6 transition-all duration-300 group-data-[clicked=true]:-rotate-180">
                <path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
              </svg>
              
        </button>
    </div>
</div>