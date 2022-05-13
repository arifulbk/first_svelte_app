<script>
	export let name;
	let person_name = "Hashim";
	function handleClick()
	{
		person_name = "Abdullah";
	}
</script>

<main>
	<h1>Assalamualykum {name}!</h1>
	<p>Assalamualykum {person_name}!</p>
	<button on:click={handleClick}>Another Name</button>
	<p class="bg-slate-800">This is a great way to start with.</p>
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