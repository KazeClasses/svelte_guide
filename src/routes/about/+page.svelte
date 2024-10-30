<script>
    let name = $state('world');

    let count = $state(0);

    function onclick() {
    count += 1;
    }
</script>
  
<input bind:value={name} placeholder="Enter your name" />
{#if name === 'world'}
  <h1>Hello {name}!</h1>
{:else}
  <h1>I don't say hello to anyone else</h1>
{/if}

<button {onclick}>
    Clicked {count} {count === 1 ? 'time' : 'times'}
</button>