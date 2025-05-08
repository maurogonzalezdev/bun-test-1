<!-- src/lib/components/HeroImage.svelte -->
<div class="hero">
  <div class="hero-content">
    <h1>Welcome to EcomStore</h1>
    <p>Discover amazing products at great prices</p>
    <a href="/products" class="cta-button">Shop Now</a>
  </div>
</div>

<style>
  .hero {
    height: 60vh;
    background-image: url('https://www.heroecommerce.com/wp-content/uploads/2024/03/products-choose.jpg');
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    text-align: center;
  }

  .hero-content {
    background: rgba(0, 0, 0, 0.5);
    padding: 2rem;
    border-radius: 8px;
  }

  h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
  }

  .cta-button {
    display: inline-block;
    padding: 1rem 2rem;
    background: #ff4444;
    color: white;
    text-decoration: none;
    border-radius: 4px;
    margin-top: 1rem;
    transition: background 0.3s;
  }

  .cta-button:hover {
    background: #ff2222;
  }
</style>
