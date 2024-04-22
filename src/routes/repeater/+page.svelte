<script>
  import Header from '$lib/Header.svelte'
  import Subheader from '$lib/Subheader.svelte'

  // Write your JavaScript here
  let said = ''
</script>


<main>
  <div class="left">
    <Header />
  </div>
  <div class="right">
    <Subheader text='Repeater'/>

    <div class="my-work">
      <!-- Write your HTML here -->
      <input type="text" bind:value={said}>
      <p>You said {said}!</p>
    </div>

  </div>
</main>