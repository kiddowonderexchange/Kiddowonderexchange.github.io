# Kiddowonderexchange.github.io
/kiddo-wonder-exchange
│── index.html
│── shop.html
│── admin.html
│── manifest.json
│── sw.js

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kiddo Wonder Exchange</title>
<link rel="manifest" href="manifest.json">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
<style>
:root{
--primary:#2563eb; --secondary:#1e40af;
--bg:#f8fafc; --card:#fff; --text:#0f172a; --muted:#64748b; --success:#22c55e;
}
[data-theme="dark"]{
--bg:#020617; --card:#020617; --text:#e5e7eb; --muted:#94a3b8;
}
body{font-family:'Inter',sans-serif;background:var(--bg);color:var(--text);margin:0;}
header{background:linear-gradient(135deg,#2563eb,#1e40af);color:#fff;padding:70px 20px;text-align:center;position:relative;}
nav a{color:white;margin:0 12px;font-weight:600;text-decoration:none;}
.toggle{position:absolute;top:20px;right:20px;padding:8px 14px;border:none;border-radius:20px;font-weight:600;cursor:pointer;}
.section{padding:60px 20px;max-width:1200px;margin:auto}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:20px}
.card{background:var(--card);padding:25px;border-radius:14px;box-shadow:0 10px 30px rgba(0,0,0,.1);}
.card h3{margin-bottom:8px;font-size:1.1rem;}
.whatsapp{background:var(--success);color:white;padding:14px 30px;border-radius:40px;text-decoration:none;font-weight:700;display:inline-block;margin-top:20px;}
input,select,button{width:100%;padding:12px;margin-top:10px;border-radius:6px;border:1px solid #cbd5e1;}
button{background:var(--primary);color:white;font-weight:600;border:none;margin-top:10px;}
footer{background:#020617;color:#cbd5e1;text-align:center;padding:25px;}
</style>
</head>
<body>
<button class="toggle" onclick="toggleTheme()">🌙</button>

<header>
<h1>Kiddo Wonder Exchange</h1>
<p><strong>Your One Stop Shop for Gadgets & Varieties!</strong><br>💥 Quality | 💰 Affordable | ⚡ Reliable</p>
<nav><a href="index.html">Home</a><a href="shop.html">Shop</a><a href="admin.html">Admin</a></nav>
</header>

<section class="section">
<h2>Our Services</h2>
<div class="grid">
<div class="card"><h3>📱 Gadgets & Smart Devices</h3></div>
<div class="card"><h3>💳 Gift Cards → Naira</h3></div>
<div class="card"><h3>₿ Bitcoin & Crypto → Naira</h3></div>
<div class="card"><h3>💼 Buying Digital Funds</h3></div>
<div class="card"><h3>🎵 Music Recording Studio</h3></div>
<div class="card"><h3>👕 Luxurious Wears</h3></div>
<div class="card"><h3>🏠 Interior & Decors</h3></div>
<div class="card"><h3>🛠 Stainless Handrails</h3></div>
<div class="card"><h3>🪟 Window Blinds</h3></div>
<div class="card"><h3>📷 CCTV Camera</h3></div>
<div class="card"><h3>⚡ Electric Fence Wire</h3></div>
</div>
</section>

<section class="section">
<h2>Rate Calculator</h2>
<div class="card">
<select id="type"><option>Gift Card</option><option>Bitcoin</option><option>PayPal</option></select>
<input id="amount" type="number" placeholder="Amount in USD">
<button onclick="calc()">Calculate

