<script>
	let FirstName = "Vincent";
	let LastName = "Kim";
	
	// Defined 'beltColour' to visualize several colors by 
	// controlling this variable.
	let beltColour = "black";
	$: fullName = `${firstName} ${lastName}`;
	$: {console.log(beltColour); console.log(fullName);}

	let imgSrc = "images.png";
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>