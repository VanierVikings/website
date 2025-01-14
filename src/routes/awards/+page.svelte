<script>
	import Header from "$lib/components/Header.svelte";
	import HeaderDropdown from "$lib/components/HeaderDropdown.svelte";
	import Footer from "../../lib/components/Footer.svelte";
	import LeadTile from "../../lib/components/LeadTile.svelte";
  
	let selectedDropdown;
	const setDropdown = (content) => {
		selectedDropdown = content;
	}
</script>

<Header setDropdown={setDropdown}/>
<HeaderDropdown content={selectedDropdown}/>
<div class="flex flex-col items-center gap-16 py-8 px-2">
    <div class="grid grid-cols-2 h-[50vh]">
        <div class="bg-gvss-dmaroon flex flex-col justify-center items-center">
            <h1 class="text-gvss-lyellow text-center text-5xl">Sucessful Rookie Season</h1>
            <h2 class="text-white text-3xl">March 10th, 2024</h2>
        </div>
        <div class="flex justify-center items-center">
            <img class="w-3/4 rounded-lg aspect-[3/2]" src="images/awards/rookie_season.jpg">
        </div>
      </div>
      <div class="grid grid-cols-2 h-[50vh]">
        <div class="bg-gvss-dmaroon flex flex-col justify-center items-center">
            <h1 class="text-gvss-lyellow text-center text-5xl">Rookie Inspiration Award</h1>
            <h2 class="text-white text-3xl">March 10th, 2024</h2>
        </div>
        <div class="flex justify-center items-center">
            <img class="w-3/4 rounded-lg aspect-[3/2]" src="images/awards/rookie_inspiration.jpg">
        </div>
      </div>
      <div class="grid grid-cols-2 h-[50vh]">
        <div class="bg-gvss-dmaroon flex flex-col justify-center items-center">
            <h1 class="text-gvss-lyellow text-center text-5xl">Rookie Allstar Award (District Level)</h1>
            <h2 class="text-white text-3xl">March 23rd, 2024</h2>
        </div>
        <div class="flex justify-center items-center">
            <img class="w-3/4 rounded-lg aspect-[3/2]" src="images/awards/rookie_allstar_district.jpg">
        </div>
      </div>
      <div class="grid grid-cols-2 h-[50vh]">
        <div class="bg-gvss-dmaroon flex flex-col justify-center items-center">
            <h1 class="text-gvss-lyellow text-center text-5xl">University of Waterloo District Event Winner</h1>
            <h2 class="text-white text-3xl">March 23rd, 2024</h2>
        </div>
        <div class="flex justify-center items-center">
            <img class="w-3/4 rounded-lg aspect-[3/2]" src="images/awards/waterloo_event_winner_2024.jpg">
        </div>
      </div>
      <div class="grid grid-cols-2 h-[50vh]">
        <div class="bg-gvss-dmaroon flex flex-col justify-center items-center">
            <h1 class="text-gvss-lyellow text-center text-5xl">Rookie Allstar Award (Provincial Level)</h1>
            <h2 class="text-white text-3xl">April 6th, 2024</h2>
        </div>
        <div class="flex justify-center items-center">
            <img class="w-3/4 rounded-lg aspect-[3/2]" src="images/awards/rookie_allstar_provincial.jpg">
        </div>
      </div>
      <div class="grid grid-cols-2 h-[50vh]">
        <div class="bg-gvss-dmaroon flex flex-col justify-center items-center">
            <h1 class="text-gvss-lyellow text-center text-5xl">Robots@CNE 2024 Offseason Event Winner</h1>
            <h2 class="text-white text-3xl">September 1st, 2024</h2>
        </div>
        <div class="flex justify-center items-center">
            <img class="w-3/4 rounded-lg aspect-[3/2]" src="images/awards/cne_winner.png">
        </div>
      </div>
</div>
<Footer/>