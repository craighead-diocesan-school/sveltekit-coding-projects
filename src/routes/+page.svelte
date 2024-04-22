<script>
  import Header from '$lib/Header.svelte'
  import Subheader from '$lib/Subheader.svelte'
  import Card from '$lib/Card.svelte'

  const projectsLeft = [
    {
      name: '🔁 Repeater 🔁',
      url: 'repeater',
      tags: ['input-output'],
    },
    {
      name: '🫡 Count the Values 🫡',
      url: 'count-the-values',
      tags: ['input-output', 'iteration', 'collections'],
    },
    {
      name: '🕵️‍♀️ Same or Different 🕵️‍♀️',
      url: 'same-or-different',
      tags: ['input-output', 'selection'],
    },
    {
      name: '👯 Count Occurrences 👯',
      url: 'count-occurrences',
      tags: ['input-output', 'iteration', 'selection', 'collections'],
    },
  ]

  const projectsRight = [
    {
      name: '🏎️ MadLibs 🏎️',
      url: 'madlibs',
      tags: ['input-output'],
    },
    {
      name: '🧮 Average 🧮',
      url: 'average',
      tags: ['input-output', 'iteration', 'collections'],
    },
    {
      name: '🔍 Number Search 🔍',
      url: 'number-search',
      tags: ['input-output', 'iteration', 'collections'],
    },
    {
      name: '📈 Sorted Check 📈',
      url: 'sorted-check',
      tags: ['input-output', 'iteration', 'selection', 'collections'],
    },
  ]
</script>

<main>
  <!-- left side of the page -->
  <div class="left">
    <Header />

    <!-- iterate through the projectsLeft array and output each one as a linked Card -->
    {#each projectsLeft as project}
      <Card name={project.name} url={project.url} tags={project.tags} />
    {/each}
  </div>
  
  <!-- right side of the page -->
  <div class="right">
    <Subheader text="Small projects to help you re-learn how to code" />

    <!-- iterate through the projectsRight array and output each one as a linked Card -->
    {#each projectsRight as project}
      <Card name={project.name} url={project.url} tags={project.tags} />
    {/each}
  </div>
</main>
