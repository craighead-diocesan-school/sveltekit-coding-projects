<slot />

<style>
  @import url('https://fonts.googleapis.com/css2?family=Gabarito:wght@400..900&display=swap');

  :global(html) {
    background-color: #1d4e89;
    font-family: 'Gabarito', sans-serif;
  }

  :global(html) {
    margin: 0;
    padding: 0;
    scrollbar-width: none;
  }

  :global(main) {
    display: flex;
    justify-content: center;
    gap: 1rem;
    padding: 3rem;
  }

  :global(div.left, div.right) {
    width: 50vw;
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }

  :global(div.left) {
    align-items: end;
  }

  :global(div.right) {
    margin-top: 8rem;
    align-items: start;
  }

  :global(a) {
    text-decoration: none;
    color: inherit;
  }

  :global(.my-work) {
    background: #fbd1a2;
    padding: 2rem;
    box-shadow: 0.5rem 0.5rem #123054;
    color: #1d4e89;
  }

  @media screen and (max-width: 600px) {
    :global(main) {
      flex-direction: column;
    }

    :global(div.left, div.right) {
      width: 100%;
      align-items: center;
    }

    :global(div.right) {
      margin-top: 1rem;
    }
  }
</style>
