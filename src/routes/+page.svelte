<script>
	import Carousel from "$lib/components/Carousel.svelte";
	import Header from "$lib/components/Header.svelte";
	import HeaderDropdown from "$lib/components/HeaderDropdown.svelte";
	import Footer from "../lib/components/Footer.svelte";
	import SponsorBar from "../lib/components/SponsorBar.svelte";
  
	
	const imageList = ["/images/carousel/OTS_Consurgo_B.JPG", "/images/carousel/OTS_Consurgo_R.JPG", "/images/carousel/OTS_Cheer.png"];
	let selectedDropdown;
	const setDropdown = (content) => {
		selectedDropdown = content;
	}
  </script>
  
  <Header setDropdown={setDropdown}/>
  <HeaderDropdown content={selectedDropdown}/>
  <Carousel images={imageList}/>
  <SponsorBar></SponsorBar>
  <div class="flex flex-col">
	<div class="grid grid-cols-2 h-[50vh] border-y-4 border-gvss-lyellow">
		<div class="bg-gvss-dmaroon flex items-center flex-col justify-center">
			<h3 class="text-5xl font-bold text-gvss-dyellow">2025 Vanier Vikings</h3>
			<a href="/our-team"><h2 class="text-4xl underline underline-offset-2 cursor-pointer hover:scale-110 transition-all text-white">Meet the team!</h2></a>
		</div>
		<div class="bg-gvss-lmaroon flex items-center overflow-hidden">
			<img class="w-full object-cover" src="/images/2025_team.jpg">
		</div>
  	</div>
	  <div class="grid grid-cols-2 h-[50vh] border-y-4 border-gvss-lyellow">
		<div class="bg-gvss-lmaroon flex items-center overflow-hidden">
			<img class="w-full object-cover" src="/images/OTS_Consurgo_B.JPG">
		</div>
		<div class="bg-gvss-dmaroon flex items-center flex-col justify-center">
			<h3 class="text-5xl font-bold text-gvss-dyellow">Conswervo</h3>
			<a href="/our-team"><h2 class="text-4xl underline underline-offset-2 cursor-pointer hover:scale-110 transition-all text-white">Our Robots!</h2></a>
		</div>
  	</div>
</div>
<Footer/>
