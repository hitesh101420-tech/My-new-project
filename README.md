# My-new-project
<!DOCTYPE html><html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Local Graphic Designer</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/emailjs-com@3/dist/email.min.js"></script>
<style>
body {font-family: 'Poppins', sans-serif; margin:0;}
header {background:#000; color:#fff; padding:15px; text-align:center;}
.hero {height:90vh; background:url('https://i.ibb.co/7JbRY779/Screenshot-20260427-034020.jpg') center/cover no-repeat; display:flex; flex-direction:column; justify-content:center; align-items:center; color:white; text-shadow:2px 2px 5px black;}
.hero h1 {font-size:3rem;}
.btn {padding:10px 20px; background:#ff6600; color:#fff; border:none; cursor:pointer;}
.products {padding:20px; overflow-x:auto; display:flex; gap:20px;}
.card {min-width:250px; border:1px solid #ddd; padding:15px;}
.cart-icon {position:fixed; top:20px; right:20px; background:black; color:white; padding:10px; border-radius:50%; cursor:pointer;}
.cart {position:fixed; right:-300px; top:0; width:300px; height:100%; background:#fff; transition:0.3s; padding:20px;}
.cart.open {right:0;}
.whatsapp {position:fixed; bottom:20px; right:20px; background:green; color:white; padding:15px; border-radius:50%; text-decoration:none;}
</style>
</head>
<body><header>
<h2>The Local Graphic Designer</h2>
<p>Fresh Finds, Best Prices</p>
</header><div class="hero">
<h1>Creative Designs That Speak</h1>
<button class="btn" onclick="scrollToProducts()">Book Now</button>
</div><div class="cart-icon" onclick="toggleCart()">🛒 <span id="count">0</span></div><div class="cart" id="cart">
<h3>Your Cart</h3>
<ul id="cart-items"></ul>
<input type="text" id="name" placeholder="Your Name"><br><br>
<input type="text" id="phone" placeholder="Phone Number"><br><br>
<button onclick="sendEmail()">Book Time</button>
</div><section id="products" class="products">
<div class="card">
<h4>Logo Design</h4>
<p>₹499</p>
<button onclick="addToCart('Logo Design')">Add</button>
</div>
<div class="card">
<h4>Poster Design</h4>
<p>₹299</p>
<button onclick="addToCart('Poster Design')">Add</button>
</div>
<div class="card">
<h4>Social Media Post</h4>
<p>₹199</p>
<button onclick="addToCart('Social Media Post')">Add</button>
</div>
</section
