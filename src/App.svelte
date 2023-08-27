<script>
	export let name;
</script>

<main>
	<h1>Hello {name.toUpperCase()}!</h1>
	<img src="/svelteIcon.png" alt="svelteIcon"/>
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
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}

		img {
			width: 50vw;
		}
	}
</style>
