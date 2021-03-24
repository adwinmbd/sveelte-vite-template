<!-- App.svelte -->
<script>
  /* component logic will go here */
  let count = 0;
  function handleClick() {
    count += 1;
  }
</script>

<div class="App">
  <header class="App-header">
    <img src="/logo.svg" class="App-logo" alt="logo" />
    <p>Hello Svelte + Vite !</p>
    <p>
      <button on:click={handleClick}>
        count is: {count}
      </button>
    </p>
    <p>
      Edit <code>App.svelte</code> and save to test HMR updates.
    </p>
    <p>
      <a
        class="App-link"
        href="https://svelte.dev"
        target="_blank"
        rel="noopener noreferrer"
      >
        Learn Svelte
      </a>
      {' | '}
      <a
        class="App-link"
        href="https://vitejs.dev"
        target="_blank"
        rel="noopener noreferrer"
      >
        Vite Docs
      </a>
    </p>
  </header>
</div>

<style>
  /* css will go here */
  .App {
    text-align: center;
  }
  .App code {
    background: #0002;
    padding: 4px 8px;
    border-radius: 4px;
  }
  .App p {
    margin: 0.4rem;
  }
  .App-header {
    color: #333;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    font-size: calc(10px + 2vmin);
  }
  .App-logo {
    height: 36vmin;
    pointer-events: none;
    margin-bottom: 3rem;
    animation: App-logo-pulse infinite 1.6s ease-in-out alternate;
  }
  @keyframes App-logo-pulse {
    from {
      transform: scale(1);
    }
    to {
      transform: scale(1.06);
    }
  }
  button {
    font-size: calc(10px + 2vmin);
  }
</style>
