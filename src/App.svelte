<script>
	import Header from './sections/Header.svelte'
  import Main from './sections/Main.svelte';
  export let name;
</script>

<Header {name} />
<Main />
