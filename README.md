<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Irfan Jute Bag</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #f2f2f2;
    }
    header {
      background: #2d572c;
      color: white;
      text-align: center;
      padding: 15px;
    }
    header h1 {
      margin: 0;
      font-size: 24px;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 15px;
      padding: 15px;
    }
    .product {
      background: white;
      border-radius: 8px;
      padding: 10px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .product img {
      width: 100%;
      max-height: 150px;
      object-fit: cover;
      border-radius: 8px;
    }
    .product h3 {
      margin: 10px 0 5px;
      font-size: 18px;
      color: #333;
    }
    .product p {
      margin: 5px 0;
      color: #555;
    }
    .contact {
      background: white;
      margin: 20px;
      padding: 15px;
      border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .contact h2 {
      text-align: center;
      color: #2d572c;
    }
    .contact input, .contact textarea {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    .contact button {
      background: #2d572c;
      color: white;
      border: none;
      padding: 12px;
      width: 100%;
      border-radius: 5px;
      cursor: pointer;
      font-size: 16px;
    }
    .contact button:hover {
      background: #244822;
    }
    footer {
      text-align: center;
      padding: 15px;
      background: #2d572c;
      color: white;
      margin-top: 20px;
    }
    footer a {
      color: white;
      text-decoration: none;
    }
  </style>
</head>
<body>

  <header>
    <h1>👜 Irfan Jute Bag</h1>
    <p>Eco-friendly | Stylish | Affordable</p>
  </header>

  <!-- Product Section -->
  <section class="products">
    <div class="product">
      <img src="https://i.imgur.com/NEB6wDK.jpg" alt="Classic Jute Bag">
      <h3>Classic Jute Bag</h3>
      <p>₹250</p>
    </div>
    <div class="product">
      <img src="https://i.imgur.com/v0drh72.jpg" alt="Shopping Jute Bag">
      <h3>Shopping Jute Bag</h3>
      <p>₹300</p>
    </div>
    <div class="product">
      <img src="https://i.imgur.com/9PbFb0r.jpg" alt="Designer Jute Bag">
      <h3>Designer Jute Bag</h3>
      <p>₹350</p>
    </div>
    <div class="product">
      <img src="https://i.imgur.com/hYoS1Xr.jpg" alt="Eco Tote Jute Bag">
      <h3>Eco Tote Jute Bag</h3>
      <p>₹280</p>
    </div>
    <div class="product">
      <img src="https://i.imgur.com/JbQkF9z.jpg" alt="Premium Office Jute Bag">
      <h3>Premium Office Jute Bag</h3>
      <p>₹400</p>
    </div>
  </section>

  <!-- Order Form -->
  <section class="contact">
    <h2>Order Now</h2>
    <form onsubmit="sendToWhatsApp(event)">
      <input type="text" id="name" placeholder="Full Name" required>
      <input type="tel" id="phone" placeholder="Phone Number" required>
      <input type="tel" id="alt" placeholder="Alternate Number">
      <textarea id="address" placeholder="Full Address" rows="3" required></textarea>
      <button type="submit">Submit Order</button>
    </form>
    <p style="text-align:center; color:#333; margin-top:10px;">
      💳 Payment Options: <b>UPI, Net Banking & Card Payment</b>
    </p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2025 Irfan Jute Bag | Owner: AJAGAR ALI</p>
    <p>📞 WhatsApp: <a href="https://wa.me/918334976089" target="_blank">8334976089</a></p>
    <p>📧 Email: <a href="mailto:irfangaming12580@gmail.com">irfangaming12580@gmail.com</a></p>
  </footer>

  <!-- WhatsApp Order Script -->
  <script>
    function sendToWhatsApp(event) {
      event.preventDefault();
      let name = document.getElementById("name").value;
      let phone = document.getElementById("phone").value;
      let alt = document.getElementById("alt").value;
      let address = document.getElementById("address").value;

      let message = `🛍️ New Order%0A👤 Name: ${name}%0A📞 Phone: ${phone}%0A📞 Alt: ${alt}%0A🏠 Address: ${address}%0A💰 Payment: UPI / Net Banking / Card`;
      window.open(`https://wa.me/918334976089?text=${message}`, "_blank");
    }
  </script>

</body>
</html>
