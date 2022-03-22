<script>
	import SearchGame from "./SearchGame.svelte";
	import Mainpage from "./Mainpage.svelte";
	import Ingame from "./Page.svelte";
	export let name;
	let window = 1
</script>
<style >
	
	:global(body){
        background-image: url('./background.png');
		background-repeat: no-repeat;
		background-attachment: fixed;
		background-size: 100% 100%;
	}
	.centerred{
		position: absolute;
		left: 30%;
		top: 10%;
		transform: translate(-50%, -50%);
	}
</style>
<main>
	{#if window==0}
	<Mainpage bind:window = {window}/>
		{:else if window == 1}
		<div class = "centerred">
			<SearchGame bind:leave = {window}/>
		</div>
		{:else}
		<Ingame></Ingame>
	{/if}
</main>
