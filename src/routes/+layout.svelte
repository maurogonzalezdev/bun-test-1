<!-- src/routes/+layout.svelte -->
<script>
  import Header from '$lib/components/Header.svelte';
</script>

<Header />
<main>
  <slot />
</main>

<style>
  main {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 1rem;
  }
</style>
