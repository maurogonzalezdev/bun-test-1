<!-- src/lib/components/Header.svelte -->
<script>
  import HeroImage from './HeroImage.svelte';
</script>

<header>
  <nav>
    <div class="logo">
      <a href="/">EcomStore</a>
    </div>
    <ul>
      <li><a href="/">Home</a></li>
      <li><a href="/products">Products</a></li>
      <li><a href="/cart">Cart</a></li>
    </ul>
  </nav>
  <HeroImage />
</header>

<style>
  header {
    width: 100%;
  }

  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 2rem;
    background: #fff;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }

  .logo a {
    font-size: 1.5rem;
    font-weight: bold;
    text-decoration: none;
    color: #333;
  }

  ul {
    display: flex;
    gap: 2rem;
    list-style: none;
  }

  a {
    text-decoration: none;
    color: #333;
  }
</style>
