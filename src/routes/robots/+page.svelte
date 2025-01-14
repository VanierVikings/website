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
<div class="bg-gvss-dmaroon h-full">
    <img class="w-full h-[50vh] object-cover blur-[1px] brightness-50" src="/images/building.JPG">
</div>
<div class="bg-gvss-dmaroon flex flex-col items-center py-4 px-4">
    <h1 class="text-8xl font-bold text-gvss-dyellow">Robots</h1>
    <p class="text-4xl p-6 text-center text-white leading-loose tracking-wide">Each of our robots have a special place in our hearts. Check out the evolution of our designs below!</p>
	<br>
	<h2 class="text-6xl font-bold text-gvss-dyellow">Meet the Robots!</h2>
	<br>
	<LeadTile image="/images/robots/conswervo.JPG" name="(2024)" title="Conswervo" description="Consurgo's cousin with a swerve drivetrain, improved bumpers, dual hook hang, and more! Used during Crescendo offseason events."/>
	<LeadTile image="/images/robots/consurgo.webp" name="(2024)" title="Consurgo" description="The start of it all. Consurgo is a modified kitbot that has a ground intake, speaker ability, and a widely anticipated functional hang. Used during Crescendo regular season."/>
</div>
<Footer/>