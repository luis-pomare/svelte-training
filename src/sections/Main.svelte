<script>
  let todoOne = {value:1, completed: false}
  let todoTwo = {value:2, completed: false}

  function toggle1() {
    todoOne.completed = !todoOne.completed
  }
  function toggle2() {
    todoTwo.completed = !todoTwo.completed
  }
  $: console.log(todoOne.value)
  $: console.log(todoTwo.value)
</script>

<main>
  <div>
    <p>{todoOne.value}: {todoOne.completed.toString()}</p>
    <button type="button" on:click={toggle1}></button>
  </div>
  <div>
    <p>{todoTwo.value}: {todoTwo.completed.toString()}</p>
    <button type="button" on:click={toggle2}></button>
  </div>
</main>
