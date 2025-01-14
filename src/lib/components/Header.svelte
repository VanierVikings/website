<script>
    import HeaderLink from "./HeaderLink.svelte";
    export let setDropdown;
    const aboutContent = {title: "About Us", links: [
        {title: "Meet The Team", link: "/our-team"},
        {title: "Sponsors", link: "/sponsors"},
        {title: "Awards", link: "/awards"},
        ]};
</script>

<div class="flex sticky top-0 z-50 bg-gvss-lmaroon border-b-8 border-gvss-lyellow h-20">
    <div class="flex justify-center items-center w-2/5">
        <a href="/" class="flex justify-center h-full items-center">
            <img src="/images/logo.webp" class="h-full py-2" alt="">
        </a>
    </div>
    <div class="flex justify-around items-center text-lg text-center font-semibold w-3/5">
    <HeaderLink content={aboutContent} setDropdown={setDropdown}/>
    <a href="/robots" class="cursor-pointer text-white after:block after:transition-all after:duration-200 after:relative after:w-0 after:bottom-0 after:left-1/2 after:h-0.5 after:bg-gvss-lyellow hover:after:w-full hover:after:left-0">Robots</a>
    <a href="https://www.firstinspires.org/" target="_blank" class="gap-2 flex flex-row items-center cursor-pointer text-white "><h1 class="after:block after:transition-all after:duration-200 after:relative after:w-0 after:bottom-0 after:left-1/2 after:h-0.5 after:bg-gvss-lyellow hover:after:w-full hover:after:left-0">FIRST</h1><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-box-arrow-up-right" viewBox="0 0 16 16">
        <path fill-rule="evenodd" d="M8.636 3.5a.5.5 0 0 0-.5-.5H1.5A1.5 1.5 0 0 0 0 4.5v10A1.5 1.5 0 0 0 1.5 16h10a1.5 1.5 0 0 0 1.5-1.5V7.864a.5.5 0 0 0-1 0V14.5a.5.5 0 0 1-.5.5h-10a.5.5 0 0 1-.5-.5v-10a.5.5 0 0 1 .5-.5h6.636a.5.5 0 0 0 .5-.5"/>
        <path fill-rule="evenodd" d="M16 .5a.5.5 0 0 0-.5-.5h-5a.5.5 0 0 0 0 1h3.793L6.146 9.146a.5.5 0 1 0 .708.708L15 1.707V5.5a.5.5 0 0 0 1 0z"/>
      </svg></a>
      <a href="https://www.firstinspires.org/robotics/frc/game-and-season" target="_blank" class="gap-2 flex flex-row items-center cursor-pointer text-white "><h1 class="after:block after:transition-all after:duration-200 after:relative after:w-0 after:bottom-0 after:left-1/2 after:h-0.5 after:bg-gvss-lyellow hover:after:w-full hover:after:left-0">Reefscape</h1><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-box-arrow-up-right" viewBox="0 0 16 16">
        <path fill-rule="evenodd" d="M8.636 3.5a.5.5 0 0 0-.5-.5H1.5A1.5 1.5 0 0 0 0 4.5v10A1.5 1.5 0 0 0 1.5 16h10a1.5 1.5 0 0 0 1.5-1.5V7.864a.5.5 0 0 0-1 0V14.5a.5.5 0 0 1-.5.5h-10a.5.5 0 0 1-.5-.5v-10a.5.5 0 0 1 .5-.5h6.636a.5.5 0 0 0 .5-.5"/>
        <path fill-rule="evenodd" d="M16 .5a.5.5 0 0 0-.5-.5h-5a.5.5 0 0 0 0 1h3.793L6.146 9.146a.5.5 0 1 0 .708.708L15 1.707V5.5a.5.5 0 0 0 1 0z"/>
      </svg></a>
    </div>
</div>