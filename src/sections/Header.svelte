<script>
	export let name
</script>

<header>
  <h1>Hello {name.charAt(0).toLocaleUpperCase()+name.slice(1)}!</h1>
  <img src="/svelteIcon.png" alt="Svelte icon">
</header>

<style>
	header {
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
		header {
			max-width: none;
		}

		img {
			width: 50vw;
		}
	}
</style>
