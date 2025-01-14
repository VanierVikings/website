<script>
	import Header from "$lib/components/Header.svelte";
	import HeaderDropdown from "$lib/components/HeaderDropdown.svelte";
  
	let selectedDropdown;
	const setDropdown = (content) => {
		selectedDropdown = content;
	}
</script>

<Header setDropdown={setDropdown}/>
<HeaderDropdown content={selectedDropdown}/>