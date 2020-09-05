<script>
	let FirstName = "Vincent";
	let LastName = "Kim";
	
	// Defined 'beltColour' to visualize several colors by 
	// controlling this variable.
	let beltColour = "black";
	$: fullName = `${FirstName} ${LastName}`;
	$: {console.log(beltColour); console.log(fullName);}

	let imgSrc = "images.png";
	let imgSrc2 = "images2.png";
</script>

<main>
	<h1>Hello {fullName}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>

	<!-- Output full-name here. -->
	<p style="color: {beltColour}">{fullName} - has {beltColour} belt</p>

	<!-- Two way bounding, 'handleInput' and 'beltColour'. -->	
	<input type="text" bind:value={FirstName}>
	<input type="text" bind:value={LastName}>
	<input type="text" bind:value={beltColour}>

	<!-- svelte-ignore a11y-missing-attribute -->
	<img src={imgSrc}>
	<img src={imgSrc2}>
</main>