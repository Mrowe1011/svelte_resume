<script>
  import logo from './assets/svelte.png'
  import Navbar from './lib/Navbar.svelte'
  import Counter from './lib/GetIP.svelte'
</script>

<main>
  <Navbar />
</main>


<style>
  :global(html) {
    background-color:black;
    color: white;
    font-family: 'Rubik', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }
</style>