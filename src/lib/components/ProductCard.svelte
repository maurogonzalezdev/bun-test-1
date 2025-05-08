<!-- src/lib/components/ProductCard.svelte -->
<script>
  export let product;
</script>

<div class="product-card">
  <img src={product.image} alt={product.name} />
  <div class="product-info">
    <h3>{product.name}</h3>
    <p class="price">${product.price}</p>
    <a href={`/products/${product.slug}`} class="view-button">View Details</a>
  </div>
</div>

<style>
  .product-card {
    border: 1px solid #eee;
    border-radius: 8px;
    overflow: hidden;
    transition: transform 0.3s;
  }

  .product-card:hover {
    transform: translateY(-5px);
  }

  img {
    width: 100%;
    height: 200px;
    object-fit: cover;
  }

  .product-info {
    padding: 1rem;
  }

  .price {
    color: #ff4444;
    font-weight: bold;
    margin: 0.5rem 0;
  }

  .view-button {
    display: block;
    text-align: center;
    padding: 0.5rem;
    background: #333;
    color: white;
    text-decoration: none;
    border-radius: 4px;
  }
</style>
