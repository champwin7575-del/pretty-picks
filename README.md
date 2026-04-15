# pretty-picks
My shopping website
<!DOCTYPE html>
<html>
<head>
<title>Pretty Picks</title>

<style>
body {
  margin: 0;
  font-family: Arial;
  background: #fff0f5;
}

/* NAVBAR */
.navbar {
  background: #ff3f6c;
  color: white;
  padding: 15px;
  text-align: center;
  font-size: 22px;
  font-weight: bold;
}

/* HERO */
.hero {
  background: linear-gradient(to right, #ff99cc, #ffe6f0);
  text-align: center;
  padding: 40px;
  color: white;
  font-size: 28px;
}

/* GRID */
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 20px;
  padding: 20px;
}

/* CARD */
.card {
  background: white;
  border-radius: 15px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  padding: 10px;
  text-align: center;
}

.card img {
  width: 100%;
  border-radius: 10px;
}

.price {
  color: #ff3f6c;
  font-weight: bold;
}

/* BUTTON */
button {
  background: #ff3f6c;
  color: white;
  border: none;
  padding: 10px;
  border-radius: 20px;
  cursor: pointer;
}

button:hover {
  background: black;
}

/* FOOTER */
.footer {
  background: #ff3f6c;
  color: white;
  padding: 20px;
  text-align: center;
  font-size: 14px;
}
</style>

<script>
function order(product, price) {
  let phone = "91XXXXXXXXXX"; // ⚠️ apna number daal
  let msg = `Hi, I want to buy ${product} for ₹${price}`;
  let url = `https://wa.me/${phone}?text=${encodeURIComponent(msg)}`;
  window.open(url, "_blank");
}
</script>

</head>

<body>

<div class="navbar">
Pretty Picks 💖
</div>

<div class="hero">
Glow Like Never Before ✨
</div>

<div class="grid">

<div class="card">
<img src="https://source.unsplash.com/300x300/?makeup">
<p>Makeup Kit</p>
<p class="price">₹999</p>
<button onclick="order('Makeup Kit',999)">Buy on WhatsApp</button>
</div>

<div class="card">
<img src="https://source.unsplash.com/300x300/?perfume">
<p>Perfume</p>
<p class="price">₹799</p>
<button onclick="order('Perfume',799)">Buy on WhatsApp</button>
</div>

<div class="card">
<img src="https://source.unsplash.com/300x300/?earrings">
<p>Earrings</p>
<p class="price">₹299</p>
<button onclick="order('Earrings',299)">Buy on WhatsApp</button>
</div>

<div class="card">
<img src="https://source.unsplash.com/300x300/?handbag">
<p>Purse</p>
<p class="price">₹1199</p>
<button onclick="order('Purse',1199)">Buy on WhatsApp</button>
</div>

</div>

<div class="footer">
<p>Cash on Delivery Available 💵</p>

<p><b>Return & Replacement Policy 💖</b></p>
<p>
• Products are non-returnable<br>
• Only 1-time replacement allowed (damage/wrong item)<br>
• Unboxing video required<br>
• Request within 24 hours
</p>

</div>

</body>
</html>
