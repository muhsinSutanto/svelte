<script>
		export let name;
		export let age;
		
		$: uppercase = name.toUpperCase()
		


	function incrementAge() {
		age += 1;
	}

	function changeName() {
		name= 'Max'
	}


</script>

<style>
	h1 {
		color: purple;
	}
</style>

<h1>Hello {uppercase} and I'm {age}!</h1>
<button on:click={incrementAge}>click</button>
<button on:click={changeName}>change name</button>
