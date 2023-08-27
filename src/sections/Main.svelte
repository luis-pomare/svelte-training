<script>
  let todos = [
    {value:'1',
      completed: false
    },
    {value:'2',
      completed: false
    },
  ]
  function toggle1() {
    todos[0].completed = !todos[0].completed
  }
  function toggle2() {
    todos[1].completed = !todos[1].completed
  }
</script>

<style>
  /* your styles go here */
</style>

<main>
  <div>
    <p>{todos[0].value}: {todos[0].completed.toString()}</p>
    <button type="button" on:click={toggle1}></button>
  </div>
  <div>
    <p>{todos[1].value}: {todos[1].completed.toString()}</p>
    <button type="button" on:click={toggle2}></button>
  </div>
</main>
