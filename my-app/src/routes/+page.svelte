<script>
	import Counter from './Counter.svelte';
	import spacestation_fallback from '$lib/images/spacestation.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>
		<span class="welcome">
			<picture>
				
				<img src={spacestation_fallback} alt="spacestation"      width="500" 
				height="500" />
			</picture>
		</span>

		
	</h1>

	<h2>
		welcome aboard <strong>CAPTAIN</strong>
	</h2>
	<div class=counters>
		<Counter material="STEEL"/>
		<Counter material="MONEY"/>
		<Counter material="FOOD"/>
	</div>

</section>

<style>
	.counters{
		display: flex;
    	justify-content: space-around;
	}
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 20%;
		padding: 0 0 20 0;
	}


</style>
