<script>
  let { text } = $props();
  let count = $state(0);

  function increment() {
    count += 1;
  }
</script>

<style>
  /* Scoped styles: only affects this component */
  button {
    color: #ff3e00;
    font-size: 1.2em;
    font-weight: bold;
  }
</style>

<button onclick={increment}>{text} + {count}</button>
