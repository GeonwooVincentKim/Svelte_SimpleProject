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
	<h1>Hello {fullName}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>
