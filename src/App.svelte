<script>
	let tmp = true;

	let years = 90;

	let age = 33;
</script>

<main>
	{#if tmp}
		<h1>How much time do you have left?</h1>
		<p>Your life visualisation to remind you to live to the fullest. Inspired by Die with Zero by Bill Perkins.</p>
		<div>
			<span>Date of birth</span>
			<input name="birthday"/>
		</div>
		<div>
			<span>You expect to live</span>
			<input name="years" value={years}/>
		</div>
	{:else}
		<h1>You’ve left</h1>
	{/if}

</main>

<style>
	
</style>