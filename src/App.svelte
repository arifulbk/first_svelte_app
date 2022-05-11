<script>
	export let name;
	let person_name = "Hashim";
	function handleClick()
	{
		person_name = "Abdullah";
	}
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Assalamualykum {person_name}!</p>
	<button on:click={handleClick}>Enter your age</button>
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