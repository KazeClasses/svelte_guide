<script>
    let name = $state('world');
  </script>
  
  <input bind:value={name} placeholder="Enter your name" />
  {#if name === 'world'}
  <h1>Hello {name}!</h1>
{:else}
  <h1>I don't say hello to anyone else</h1>
{/if}