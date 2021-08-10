<script>
    export let expectedAge;
    export let tmp;

    function handleChange() {
		console.log(this.value)
	}
	function handleSubmit() {
		tmp = false;
	}
</script>

<h1>How much time do you have left?</h1>
<p>Your life visualisation to remind you to live to the fullest. Inspired by Die with Zero by Bill Perkins.</p>
<form on:submit={handleSubmit}>
    <label>
        Date of birth
        <input type="text" on:keyup={handleChange}/>
    </label>
    <label>
        You expect to live
        <input type="number" bind:value={expectedAge}/>
    </label>
    <button>Next</button>
</form>