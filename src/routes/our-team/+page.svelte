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
    <img class="w-full h-[50vh] object-cover blur-[1px] brightness-50" src="/images/waterloo.jpg">
</div>
<div class="bg-gvss-dmaroon flex flex-col items-center py-4 px-4">
    <h1 class="text-8xl font-bold text-gvss-dyellow">Our Team</h1>
    <p class="text-4xl p-6 text-center text-white leading-loose tracking-wide">The Vanier Vikings are a sophomore FRC team from Georges Vanier Secondary School, founded in late 2023 by Sevara, with guidance from mentors Vincent Furlin and Stanley Duong. The team quickly made a mark in the FRC community, winning the district event at the University of Waterloo and claiming the Rookie All-Star award at the provincial level. Their hard work and innovation led them to the world championship in Houston, Texas, marking a remarkable achievement in their debut season.</p>
	<br>
	<h2 class="text-6xl font-bold text-gvss-dyellow">Meet the Leads!</h2>
	<br>
	<LeadTile image="/images/leads/jayden.jpg" name="Jayden" title="Team Manager" description="My name is Jayden and I am the team manager of the Vanier Vikings, my main role is facilitating organization and communication within the team!"/>
	<LeadTile image="/images/leads/faris.jpg" name="Faris" title="Business Lead" description="I love to study and make money 💸"/>
	<LeadTile image="/images/leads/arjun.jpg" name="Arjun" title="Programming Lead" description="I program the robot 👍"/>
	<LeadTile image="/images/leads/dayyan.jpg" name="Dayyan" title="CAD Lead" description="I design the robot 🔥"/>
	<LeadTile image="/images/leads/eric.jpg" name="Eric" title="Design Lead" description="I joined robotics to gain a better understanding of engineering and all that goes behind it. My favourite part of robotics is definitely competition, after all winning is always fun."/>
	<LeadTile image="/images/leads/hayden.jpg" name="Hayden" title="Mechanical Lead" description="Hi! My name is Hayden and I joined robotics as the mech lead because I love assembling robots and working with tools and metal!"/>
	<LeadTile image="/images/leads/tiana.jpg" name="Tiana" title="Mechanical Lead" description="Hi!!! My name is Tiana and I am the mechanical lead! I've been doing robotics for 6 years and have gone to worlds 4 times!"/>
	<LeadTile image="/images/leads/rafia.png" name="Rafia" title="Electrial Lead" description="Hi! I'm Rafia, this year's Electrical Lead. I've always had a passion for engineering which led me to spend two summers as a lab assistant at the Lassonde School of Engineering."/>
	<LeadTile image="/images/leads/mohan.jpg" name="Mohan" title="Media/Outreach Lead" description="Hi, I'm Mohan, this year's Media Lead. I run the Team 9659 Instagram. Something about me is that I love music, whether I'm playing the guitar or just listening to songs. My hobbies are photography and biking."/>
	<LeadTile image="/images/leads/jeeny.jpg" name="Jeeny" title="Marketing Lead" description="Hi I'm Jeeny! I enjoy reading and baking! I joined robotics for the fun experience and community!"/>
	<LeadTile image="/images/leads/juliane.jpg" name="Juliane" title="Art Lead" description="Hi! I like making all kinds of art, but I have the most fun with pottery :) I'm looking forward to having a bunch of fun with friends at comp this season!!"/>
	<LeadTile image="/images/leads/rahul.png" name="Rahul" title="Art Lead" description="Hey! I make the team look nice. I also enjoy the chaos of competitions 😎"/>
</div>
<Footer/>