<script>
	import Form from './Form.svelte';
	import Viz from './Viz.svelte';


	let tmp = true;

	let expectedAge = 90;	

	
</script>

<main>
	{#if tmp}
		<Form expectedAge={expectedAge} tmp={tmp}/>
	{:else}
		<Viz/>
	{/if}

</main>

<style>
	
</style>