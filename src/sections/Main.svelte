<script>
  let todo = {value:1, completed: false}

  function toggle1() {
    todo.completed = !todo.completed
  }
</script>

<main>
  <div>
    <p>{todo.value}: {todo.completed.toString()}</p>
    {#if todo.completed}
      <button type="button" on:click={toggle1}>Mark as undone</button>
    {/if}
    {#if !todo.completed}
      <button type="button" on:click={toggle1}>Mark as done</button>
    {/if}

  </div>
</main>
