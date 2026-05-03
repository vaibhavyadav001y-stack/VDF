<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Vaibhav Dairy Farm | Order Milk Online</title>

<meta name="description" content="Order fresh milk daily with subscription. Pay via UPI and get home delivery.">

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
:root{--green:#2e7d32;--dark:#1b5e20;--light:#f5f5f5;--accent:#43a047}
body{margin:0;font-family:Poppins;background:var(--light)}
header,footer{text-align:center;background:var(--green);color:#fff;padding:15px}
nav{background:var(--dark);display:flex;justify-content:center;gap:20px;padding:10px}
nav a{color:#fff;text-decoration:none}
.hero{text-align:center;padding:80px 20px;background:url('https://images.unsplash.com/photo-1605000797499-95a51c5269ae') center/cover;color:#fff}
.btn{background:var(--accent);padding:12px 20px;color:#fff;border:none;border-radius:8px;text-decoration:none;cursor:pointer}
.section{text-align:center;padding:40px 20px}
.products,.plans{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:20px}
.card{background:#fff;padding:20px;border-radius:10px;box-shadow:0 3px 8px rgba(0,0,0,.1)}
input,select{width:100%;padding:10px;margin:8px 0}
.whatsapp{position:fixed;bottom:20px;right:20px;background:#25D366;color:#fff;padding:15px;border-radius:50px;text-decoration:none}
</style>
</head>

<body>

<header>
<h1>Vaibhav Dairy Farm 🐄</h1>
<p>Fresh Milk Subscription | Direct From Farm</p>
</header>

<nav>
<a href="#">Home</a>
<a href="#products">Products</a>
<a href="#plans">Subscription</a>
<a href="#order">Order</a>
</nav>

<section class="hero">
<h2>Daily Fresh Milk at Your Doorstep</h2>
<p>Subscribe Today & Never Miss Milk</p>
<a href="#order" class="btn">Start Order</a>
</section>

<section id="products" class="section">
<h2>Products</h2>
<div class="products">
<div class="card"><h3>Milk</h3><p>₹50/Litre</p></div>
<div class="card"><h3>Ghee</h3><p>₹900/Kg</p></div>
</div>
</section>

<section id="plans" class="section">
<h2>Milk Subscription Plans</h2>
<div class="plans">
<div class="card"><h3>Daily Plan</h3><p>1L/day</p></div>
<div class="card"><h3>Family Plan</h3><p>2L/day</p></div>
<div class="card"><h3>Custom Plan</h3><p>As per need</p></div>
</div>
</section>

<section id="order" class="section">
<h2>Order Now</h2>
<input type="text" id="name" placeholder="Your Name">
<input type="text" id="phone" placeholder="Phone">
<select id="product">
<option>Milk</option>
<option>Ghee</option>
</select>
<input type="text" id="qty" placeholder="Quantity (e.g. 2L)">
<input type="text" id="address" placeholder="Address">
<button class="btn" onclick="sendWhatsApp()">Order on WhatsApp</button>
</section>

<section class="section">
<h2>Pay via UPI</h2>
<p>Scan & Pay (add your QR here)</p>
<p>UPI ID: yourupi@bank</p>
</section>

<a href="https://wa.me/91XXXXXXXXXX" class="whatsapp">Chat</a>

<footer>
<p>© 2026 Vaibhav Dairy Farm | Earn From Dairy 🚀</p>
</footer>

<script>
function sendWhatsApp(){
let name=document.getElementById('name').value;
let phone=document.getElementById('phone').value;
let product=document.getElementById('product').value;
let qty=document.getElementById('qty').value;
let address=document.getElementById('address').value;

let message=`Order Details:%0AName: ${name}%0APhone: ${phone}%0AProduct: ${product}%0AQuantity: ${qty}%0AAddress: ${address}`;

window.open(`https://wa.me/91XXXXXXXXXX?text=${message}`,'_blank');
}
</script>

</body>
</html>
