# Store.karlqq
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Afterglow Vinyl Store</title>
  <style>
    body {
      font-family: "Helvetica Neue", Arial, sans-serif;
      background-color: #0a0a0a;
      color: #f5f5f5;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      margin: 0;
    }

    .product-card {
      background: #111;
      border: 1px solid #333;
      border-radius: 12px;
      padding: 30px;
      text-align: center;
      width: 320px;
      box-shadow: 0 0 15px rgba(255, 0, 100, 0.2);
    }

    .product-card img {
      width: 100%;
      border-radius: 10px;
      margin-bottom: 15px;
    }

    h1 {
      font-size: 1.8em;
      margin-bottom: 10px;
    }

    p.price {
      font-size: 1.3em;
      color: #ff66b3;
      margin-bottom: 20px;
    }

    button {
      background-color: #ff3399;
      border: none;
      color: #fff;
      padding: 12px 25px;
      border-radius: 6px;
      cursor: pointer;
      font-size: 1em;
      transition: background 0.2s ease-in-out;
    }

    button:hover {
      background-color: #ff66b3;
    }

    .message {
      margin-top: 15px;
      color: #00ff99;
      display: none;
    }
  </style>
</head>
<body>
  <div class="product-card">
    <img src="afterglow-vinyl.jpg" alt="Afterglow Vinyl Cover">
    <h1>Afterglow 7” Vinyl</h1>
    <p>Limited edition pink splatter design</p>
    <p class="price">€13.99</p>
    <button onclick="addToCart()">Add to Cart</button>
    <p class="message" id="cart-message">✅ Added to cart!</p>
  </div>

  <script>
    function addToCart() {
      const msg = document.getElementById("cart-message");
      msg.style.display = "block";
      setTimeout(() => {
        msg.style.display = "none";
      }, 2000);
    }
  </script>
</body>
</html>
