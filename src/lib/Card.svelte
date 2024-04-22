<script>
  // receive the name and tags as props
  export let name = ''
  export let url = ''
  export let tags = []
</script>

<a href='{url}'>
  <h2>{name}</h2>
  <ul>
    {#each tags as tag}
      <li class={tag}>{tag}</li>
    {/each}
  </ul>
</a>

<style>
  a {
    background: #fbd1a2;
    padding: 2rem;
    box-shadow: 0.5rem 0.5rem #123054;
    color: #1d4e89;
  }

  h2 {
    font-weight: bold;
    font-size: x-large;
    margin: 2rem 0;
    text-align: center;
  }

  ul {
    padding-inline-start: 0;
    margin: 0 0;
  }

  li {
    display: inline;
    margin-right: 1rem;
    padding: 0.5rem;
    border-radius: 0.5rem;
    color: white;
    font-weight: bold;
    font-size: small;
  }

  .input-output {
    background: #e27396;
  }

  .iteration {
    background: #7698b3;
  }

  .selection {
    background: #377771;
  }

  .collections {
    background: #4ce0b3;
  }
</style>
