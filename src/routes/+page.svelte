<!-- src/routes/+page.svelte -->
<script>
  import { products } from '$lib/data/products';
  import ProductCard from '$lib/components/ProductCard.svelte';
</script>

<section class="featured-products">
  <h2>Featured Products</h2>
  <div class="product-grid">
    {#each products.slice(0, 4) as product}
      <ProductCard {product} />
    {/each}
  </div>
</section>

<style>
  .featured-products {
    padding: 4rem 0;
  }

  h2 {
    text-align: center;
    margin-bottom: 2rem;
  }

  .product-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
  }
</style>
