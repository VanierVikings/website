<script>
	import Carousel from "../lib/components/Carousel.svelte";
	import Header from "../lib/components/Header.svelte";

	const imageList = ["/images/carousel/consurgo.webp","/images/carousel/consurgo.webp","/images/carousel/consurgo.webp"];
</script>

<Header/>
<Carousel images={imageList}/>

