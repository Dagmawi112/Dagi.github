<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Online Tech Shop</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <link href="https://fonts.googleapis.com/css2?family=Crimson+Text&family=Roboto&display=swap" rel="stylesheet">
  <style>
    /* Base Styles */
    body {
      margin: 0;
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
      background-color: #f9fafb;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }

    /* Header Styles */
    header {
      background-color: #1a1a1a;
      color: white;
      padding: 2rem 0;
    }

    .container {
      width: 100%;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 1rem;
    }

    h1 {
      font-size: 1.875rem;
      text-align: center;
      font-family: 'Crimson Text', serif;
      margin: 0;
    }

    @media (min-width: 768px) {
      h1 {
        font-size: 2.25rem;
      }
    }

    header p {
      text-align: center;
      margin-top: 0.5rem;
      color: #d1d5db;
      font-family: 'Roboto', sans-serif;
      margin-bottom: 0;
    }

    /* Main Content */
    main {
      padding: 2rem 1rem;
      flex: 1;
    }

    /* Product Grid */
    .product-grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 2rem;
      margin-bottom: 2rem;
    }

    @media (min-width: 768px) {
      .product-grid {
        grid-template-columns: repeat(2, 1fr);
      }
    }

    @media (min-width: 1024px) {
      .product-grid {
        grid-template-columns: repeat(3, 1fr);
      }
    }

    /* Product Card */
    .product-card {
      background-color: white;
      border-radius: 0.5rem;
      box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
      overflow: hidden;
    }

    .product-image {
      position: relative;
      height: 200px;
    }

    .product-image img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .product-details {
      padding: 1.5rem;
    }

    .product-details h2 {
      font-size: 1.25rem;
      margin-bottom: 0.5rem;
      font-family: 'Crimson Text', serif;
    }

    .description {
      color: #4b5563;
      font-size: 0.875rem;
      margin-bottom: 1rem;
      font-family: 'Roboto', sans-serif;
    }

    .product-footer {
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .price {
      font-size: 1.5rem;
      color: #2c5282;
      font-family: 'Roboto', sans-serif;
    }

    .buy-button {
      background-color: #2c5282;
      color: white;
      padding: 0.5rem 1rem;
      border-radius: 0.25rem;
      text-decoration: none;
      font-family: 'Roboto', sans-serif;
      transition: background-color 0.3s;
    }

    .buy-button:hover {
      background-color: #1a365d;
    }

    .mr-2 {
      margin-right: 0.5rem;
    }

    /* Navigation Buttons */
    .nav-buttons {
      display: flex;
      justify-content: center;
      gap: 1rem;
      padding: 1.5rem 0;
      background-color: #f3f4f6;
      margin-top: auto;
    }

    .nav-button {
      padding: 0.75rem 1.5rem;
      border-radius: 0.375rem;
      text-decoration: none;
      font-family: 'Roboto', sans-serif;
      font-weight: 500;
      transition: all 0.3s;
    }

    .home-button {
      background-color: #2c5282;
      color: white;
      border: 2px solid #2c5282;
    }

    .home-button:hover {
      background-color: #1a365d;
      border-color: #1a365d;
    }

    .about-button {
      background-color: transparent;
      color: #2c5282;
      border: 2px solid #2c5282;
    }

    .about-button:hover {
      background-color: #2c5282;
      color: white;
    }
  </style>
</head>
<body>
  <div>
    <header>
      <div class="container">
        <h1>Welcome to Our Curated Tech Collection</h1>
        <p>Discover premium products selected just for you</p>
      </div>
    </header>

    <main class="container">
      <div class="product-grid">
        <!-- Product 1 -->
        <div class="product-card">
          <div class="product-image">
            <img src="/images/headphones.jpg" alt="Premium Wireless Headphones">
          </div>
          <div class="product-details">
            <h2>Premium Wireless Headphones</h2>
            <p class="description">High-quality wireless headphones with noise cancellation and 30-hour battery life</p>
            <div class="product-footer">
              <span class="price">$199.99</span>
              <a href="https://example.com/headphones-affiliate" target="_blank" rel="noopener noreferrer" class="buy-button">
                <i class="fas fa-shopping-cart mr-2"></i>
                Buy Now
              </a>
            </div>
          </div>
        </div>

        <!-- Product 2 -->
        <div class="product-card">
          <div class="product-image">
            <img src="/images/smartwatch.jpg" alt="Smart Fitness Watch">
          </div>
          <div class="product-details">
            <h2>Smart Fitness Watch</h2>
            <p class="description">Track your health and fitness with this advanced smartwatch featuring heart rate monitoring</p>
            <div class="product-footer">
              <span class="price">$149.99</span>
              <a href="https://example.com/smartwatch-affiliate" target="_blank" rel="noopener noreferrer" class="buy-button">
                <i class="fas fa-shopping-cart mr-2"></i>
                Buy Now
              </a>
            </div>
          </div>
        </div>

        <!-- Product 3 -->
        <div class="product-card">
          <div class="product-image">
            <img src="/images/powerbank.jpg" alt="Portable Power Bank">
          </div>
          <div class="product-details">
            <h2>Portable Power Bank</h2>
            <p class="description">20000mAh portable charger with fast charging capability for all your devices</p>
            <div class="product-footer">
              <span class="price">$49.99</span>
              <a href="https://example.com/powerbank-affiliate" target="_blank" rel="noopener noreferrer" class="buy-button">
                <i class="fas fa-shopping-cart mr-2"></i>
                Buy Now
              </a>
            </div>
          </div>
        </div>

        <!-- Product 4 -->
        <div class="product-card">
          <div class="product-image">
            <img src="/images/mouse.jpg" alt="Wireless Gaming Mouse">
          </div>
          <div class="product-details">
            <h2>Wireless Gaming Mouse</h2>
            <p class="description">Professional gaming mouse with RGB lighting and customizable buttons</p>
            <div class="product-footer">
              <span class="price">$79.99</span>
              <a href="https://example.com/mouse-affiliate" target="_blank" rel="noopener noreferrer" class="buy-button">
                <i class="fas fa-shopping-cart mr-2"></i>
                Buy Now
              </a>
            </div>
          </div>
        </div>
      </div>
    </main>

    <!-- Navigation Buttons at Bottom -->
    <div class="nav-buttons">
      <a href="#" class="nav-button home-button">
        <i class="fas fa-home mr-2"></i>Home
      </a>
      <a href="#" class="nav-button about-button">
        <i class="fas fa-info-circle mr-2"></i>About Us
      </a>
    </div>
  </div>
</body>
</html>
