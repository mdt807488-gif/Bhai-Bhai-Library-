<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>ভাই ভাই লাইব্রেরী | অনলাইন শপ</title>

<style>
:root{
  --green:#075b32;
  --dark:#032f1b;
  --orange:#f57224;
  --light:#f4f6f5;
  --white:#fff;
}

*{margin:0;padding:0;box-sizing:border-box}

body{
  font-family:Arial,"Noto Sans Bengali",sans-serif;
  background:var(--light);
  color:#222;
}

a{text-decoration:none;color:inherit}
button{cursor:pointer;font-family:inherit}

/* TOP BAR */
.topbar{
  background:var(--dark);
  color:#fff;
  padding:10px 15px;
}

.topbar-content{
  max-width:1200px;
  margin:auto;
  display:flex;
  justify-content:center;
  flex-wrap:wrap;
  gap:18px;
  font-size:15px;
}

/* HEADER */
header{
  background:#fff;
  padding:18px 15px;
  box-shadow:0 2px 10px rgba(0,0,0,.08);
}

.header-content{
  max-width:1200px;
  margin:auto;
  display:flex;
  align-items:center;
  gap:20px;
}

.logo-area{
  display:flex;
  align-items:center;
  gap:12px;
  min-width:300px;
}

.logo{
  width:65px;
  height:65px;
  border:2px solid var(--orange);
  border-radius:50%;
  display:flex;
  justify-content:center;
  align-items:center;
  color:var(--green);
  font-size:22px;
  font-weight:bold;
  position:relative;
}

.logo:after{
  content:"📖";
  position:absolute;
  bottom:-12px;
  font-size:25px;
}

.logo-text h1{
  color:var(--green);
  font-size:25px;
}

.logo-text p{
  color:#777;
  font-size:12px;
  margin-top:5px;
}

.search{
  flex:1;
  display:flex;
  border:1px solid #ddd;
  border-radius:8px;
  overflow:hidden;
  height:52px;
}

.search input{
  flex:1;
  border:0;
  padding:0 15px;
  font-size:16px;
  outline:none;
}

.search button{
  border:0;
  background:var(--orange);
  color:#fff;
  padding:0 25px;
  font-size:16px;
  font-weight:bold;
}

.cart{
  position:relative;
  border:0;
  background:transparent;
  font-size:16px;
}

.cart span{
  position:absolute;
  top:-10px;
  right:-12px;
  background:var(--orange);
  color:#fff;
  width:23px;
  height:23px;
  border-radius:50%;
  font-size:12px;
  display:grid;
  place-items:center;
}

/* NAV */
nav{
  background:#fff;
  border-top:1px solid #eee;
}

.nav-content{
  max-width:1200px;
  margin:auto;
  display:flex;
  justify-content:center;
  flex-wrap:wrap;
  gap:30px;
  padding:15px;
}

.nav-content a{
  font-weight:bold;
}

.nav-content a:hover{
  color:var(--orange);
}

/* MAIN */
main{
  max-width:1200px;
  margin:auto;
  padding:20px 15px;
}

/* HERO */
.hero{
  min-height:350px;
  background:linear-gradient(135deg,#032f1b,#08703d);
  border-radius:15px;
  color:#fff;
  padding:45px;
  position:relative;
  overflow:hidden;
}

.hero h2{
  font-size:48px;
  color:#ffd166;
  max-width:650px;
}

.hero p{
  font-size:19px;
  line-height:1.7;
  max-width:600px;
  margin:18px 0;
}

.hero button{
  border:0;
  background:var(--orange);
  color:#fff;
  padding:14px 25px;
  border-radius:7px;
  font-size:16px;
  font-weight:bold;
}

.hero .art{
  position:absolute;
  right:7%;
  bottom:20px;
  font-size:130px;
  opacity:.8;
}

/* FEATURES */
.features{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:15px;
  margin:20px 0;
}

.feature{
  background:#fff;
  padding:20px;
  text-align:center;
  border-radius:10px;
  box-shadow:0 2px 10px rgba(0,0,0,.07);
}

.feature i{
  display:block;
  font-size:35px;
  margin-bottom:8px;
}

.feature h3{
  color:var(--green);
  font-size:16px;
}

.feature p{
  color:#777;
  font-size:12px;
  margin-top:5px;
}

/* SECTION */
.section{
  background:#fff;
  margin-top:20px;
  padding:22px;
  border-radius:12px;
  box-shadow:0 2px 10px rgba(0,0,0,.07);
}

.section-head{
  display:flex;
  justify-content:space-between;
  align-items:center;
  margin-bottom:20px;
}

.section h2{
  color:#333;
}

.see-all{
  color:var(--green);
  font-weight:bold;
}

/* CATEGORY */
.categories{
  display:grid;
  grid-template-columns:repeat(6,1fr);
  gap:12px;
}

.category{
  border:1px solid #eee;
  padding:18px 10px;
  border-radius:8px;
  text-align:center;
  cursor:pointer;
}

.category:hover{
  border-color:var(--green);
  background:#f3fff8;
}

.category .emoji{
  font-size:40px;
}

.category h4{
  margin-top:8px;
  font-size:14px;
}

/* PRODUCTS */
.products{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:15px;
}

.product{
  border:1px solid #eee;
  border-radius:10px;
  overflow:hidden;
  position:relative;
}

.badge{
  position:absolute;
  top:8px;
  left:8px;
  background:#e53935;
  color:#fff;
  padding:5px 8px;
  border-radius:5px;
  font-size:11px;
}

.product-img{
  height:170px;
  background:#f4f6f5;
  display:grid;
  place-items:center;
  font-size:75px;
}

.product-info{
  padding:14px;
}

.product-info h3{
  font-size:15px;
  min-height:42px;
}

.price{
  color:var(--orange);
  font-size:20px;
  font-weight:bold;
  margin-top:8px;
}

.old{
  color:#999;
  text-decoration:line-through;
  font-size:12px;
  margin-left:5px;
}

.product button{
  width:100%;
  margin-top:10px;
  border:0;
  background:var(--green);
  color:#fff;
  padding:10px;
  border-radius:6px;
  font-weight:bold;
}

/* FOOTER */
footer{
  background:var(--dark);
  color:#fff;
  margin-top:40px;
  padding:40px 15px 20px;
}

.footer-content{
  max-width:1200px;
  margin:auto;
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:30px;
}

footer h3{
  margin-bottom:15px;
}

footer p, footer a{
  color:#d4e0d8;
  line-height:1.8;
  font-size:14px;
}

.copyright{
  max-width:1200px;
  margin:30px auto 0;
  padding-top:15px;
  border-top:1px solid #ffffff22;
  text-align:center;
}

/* CART DRAWER */
.overlay{
  display:none;
  position:fixed;
  inset:0;
  background:rgba(0,0,0,.5);
  z-index:99;
}

.overlay.show{display:block}

.cart-box{
  position:fixed;
  right:-450px;
  top:0;
  width:400px;
  max-width:100%;
  height:100%;
  background:#fff;
  z-index:100;
  transition:.3s;
  display:flex;
  flex-direction:column;
}

.cart-box.show{right:0}

.cart-header{
  background:var(--green);
  color:#fff;
  padding:18px;
  display:flex;
  justify-content:space-between;
}

.close{
  background:none;
  border:0;
  color:#fff;
  font-size:25px;
}

.cart-items{
  flex:1;
  padding:15px;
  overflow:auto;
}

.cart-item{
  border-bottom:1px solid #eee;
  padding:12px 0;
}

.cart-item strong{
  display:block;
}

.cart-item button{
  margin-top:8px;
  border:0;
  padding:5px 9px;
  background:#eee;
}

.cart-footer{
  padding:18px;
  border-top:1px solid #ddd;
}

.total{
  font-size:20px;
  font-weight:bold;
  display:flex;
  justify-content:space-between;
  margin-bottom:15px;
}

.order-btn{
  width:100%;
  background:#25d366;
  color:#fff;
  border:0;
  padding:15px;
  border-radius:7px;
  font-size:16px;
  font-weight:bold;
}

.empty{
  text-align:center;
  color:#888;
  margin-top:60px;
}

/* MOBILE */
@media(max-width:800px){
  .header-content{
    flex-wrap:wrap;
  }

  .logo-area{
    min-width:0;
  }

  .search{
    order:3;
    flex-basis:100%;
  }

  .hero h2{
    font-size:35px;
  }

  .hero .art{
    opacity:.2;
  }

  .features{
    grid-template-columns:repeat(2,1fr);
  }

  .categories{
    grid-template-columns:repeat(3,1fr);
  }

  .products{
    grid-template-columns:repeat(2,1fr);
  }

  .footer-content{
    grid-template-columns:1fr;
  }
}

@media(max-width:500px){
  .hero{
    padding:30px 20px;
  }

  .hero h2{
    font-size:29px;
  }

  .hero p{
    font-size:15px;
  }

  .logo{
    width:55px;
    height:55px;
  }

  .logo-text h1{
    font-size:20px;
  }

  .features{
    gap:8px;
  }

  .feature{
    padding:12px 5px;
  }

  .feature p{
    display:none;
  }
}
</style>
</head>

<body>

<div class="topbar">
  <div class="topbar-content">
    <a href="tel:01955015589">📞 01955015589</a>
    <a href="javascript:void(0)" onclick="openWhatsApp()">💬 WhatsApp</a>
    <a href="#products">🎧 অর্ডার করুন</a>
    <a href="#about">আমাদের সম্পর্কে</a>
    <a href="#contact">যোগাযোগ</a>
  </div>
</div>

<header>
  <div class="header-content">

    <a href="#" class="logo-area">
      <div class="logo">BBL</div>
      <div class="logo-text">
        <h1>ভাই ভাই লাইব্রেরী</h1>
        <p>বই, খাতা, কলম ও শিক্ষা সামগ্রীর বিশ্বস্ত ঠিকানা</p>
      </div>
    </a>

    <div class="search">
      <input type="text" id="searchInput"
      placeholder="আপনার পছন্দের পণ্য খুঁজুন..."
      onkeyup="searchProducts()">
      <button onclick="searchProducts()">🔍 খুঁজুন</button>
    </div>

    <button class="cart" onclick="toggleCart()">🛒 কার্ট
      <span id="cartCount">0</span>
    </button>

  </div>
</header>

<nav>
  <div class="nav-content">
    <a href="#">🏠 হোম</a>
    <a href="#categories">ক্যাটাগরি</a>
    <a href="#products">জনপ্রিয় পণ্য</a>
    <a href="#offers">🔥 বিশেষ অফার</a>
    <a href="#contact">যোগাযোগ</a>
  </div>
</nav>

<main>

<section class="hero">
  <div class="art">📚🎒</div>

  <h2>আপনার শিক্ষা সামগ্রীর বিশ্বস্ত অনলাইন শপ</h2>
  <p>
    স্কুল, কলেজ ও মাদ্রাসার বই, খাতা, কলম, জ্যামিতি বক্স,
    ব্যাগসহ সকল শিক্ষা সামগ্রী পাইকারি ও খুচরা মূল্যে।
  </p>

  <button onclick="document.getElementById('products').scrollIntoView()">
    এখনই পণ্য দেখুন
  </button>
</section>

<section class="features">
  <div class="feature">
    <i>🚚</i>
    <h3>দ্রুত ডেলিভারি</h3>
    <p>সহজ ও দ্রুত অর্ডার</p>
  </div>

  <div class="feature">
    <i>💰</i>
    <h3>সাশ্রয়ী মূল্য</h3>
    <p>পাইকারি ও খুচরা বিক্রি</p>
  </div>

  <div class="feature">
    <i>📚</i>
    <h3>সব ধরনের বই</h3>
    <p>স্কুল, কলেজ ও মাদ্রাসা</p>
  </div>

  <div class="feature">
    <i>💬</i>
    <h3>WhatsApp অর্ডার</h3>
    <p>সহজে অর্ডার করুন</p>
  </div>
</section>

<section class="section" id="categories">
  <div class="section-head">
    <h2>জনপ্রিয় ক্যাটাগরি</h2>
  </div>

  <div class="categories">
    <div class="category"><div class="emoji">📖</div><h4>স্কুল বই</h4></div>
    <div class="category"><div class="emoji">📚</div><h4>কলেজ বই</h4></div>
    <div class="category"><div class="emoji">🕌</div><h4>মাদ্রাসা বই</h4></div>
    <div class="category"><div class="emoji">✏️</div><h4>স্টেশনারি</h4></div>
    <div class="category"><div class="emoji">🎒</div><h4>ব্যাগ</h4></div>
    <div class="category"><div class="emoji">🎁</div><h4>বিশেষ অফার</h4></div>
  </div>
</section>

<section class="section" id="offers">
  <div class="section-head">
    <h2>🔥 বিশেষ অফার</h2>
    <span class="see-all">সব অফার দেখুন</span>
  </div>

  <div class="products">

    <div class="product" data-name="পেপার সোপ">
      <span class="badge">অফার</span>
      <div class="product-img">🧼</div>
      <div class="product-info">
        <h3>পেপার সোপ</h3>
        <div class="price">৩০ টাকা <span class="old">৪০ টাকা</span></div>
        <button onclick="addToCart('পেপার সোপ',30)">🛒 কার্টে যোগ করুন</button>
      </div>
    </div>

    <div class="product" data-name="ম্যাজিক স্লেট">
      <span class="badge">অফার</span>
      <div class="product-img">🖍️</div>
      <div class="product-info">
        <h3>ম্যাজিক স্লেট</h3>
        <div class="price">১৭৯ টাকা <span class="old">২২০ টাকা</span></div>
        <button onclick="addToCart('ম্যাজিক স্লেট',179)">🛒 কার্টে যোগ করুন</button>
      </div>
    </div>

    <div class="product" data-name="এক্সাম ফাইল প্যাক">
      <span class="badge">জনপ্রিয়</span>
      <div class="product-img">📁</div>
      <div class="product-info">
        <h3>এক্সাম ফাইল প্যাক</h3>
        <div class="price">৩৯০ টাকা</div>
        <button onclick="addToCart('এক্সাম ফাইল প্যাক',390)">🛒 কার্টে যোগ করুন</button>
      </div>
    </div>

    <div class="product" data-name="জ্যামিতি বক্স">
      <div class="product-img">📐</div>
      <div class="product-info">
        <h3>জ্যামিতি বক্স</h3>
        <div class="price">অর্ডার করুন</div>
        <button onclick="addToCart('জ্যামিতি বক্স',0)">🛒 কার্টে যোগ করুন</button>
      </div>
    </div>

  </div>
</section>

<section class="section" id="products">
  <div class="section-head">
    <h2>জনপ্রিয় পণ্য</h2>
    <span class="see-all">সব পণ্য</span>
  </div>

  <div class="products">

    <div class="product" data-name="স্কুল খাতা">
      <div class="product-img">📒</div>
      <div class="product-info">
        <h3>স্কুল খাতা</h3>
        <div class="price">অর্ডার করুন</div>
        <button onclick="addToCart('স্কুল খাতা',0)">🛒 কার্টে যোগ করুন</button>
      </div>
    </div>

    <div class="product" data-name="ম্যাটাডোর কলম">
      <div class="product-img">🖊️</div>
      <div class="product-info">
        <h3>ম্যাটাডোর কলম</h3>
        <div class="price">অর্ডার করুন</div>
        <button onclick="addToCart('ম্যাটাডোর কলম',0)">🛒 কার্টে যোগ করুন</button>
      </div>
    </div>

    <div class="product" data-name="স্কুল ব্যাগ">
      <div class="product-img">🎒</div>
      <div class="product-info">
        <h3>স্কুল ব্যাগ</h3>
        <div class="price">অর্ডার করুন</div>
        <button onclick="addToCart('স্কুল ব্যাগ',0)">🛒 কার্টে যোগ করুন</button>
      </div>
    </div>

    <div class="product" data-name="পাঠ্যবই">
      <div class="product-img">📚</div>
      <div class="product-info">
        <h3>পাঠ্যবই ও গাইড</h3>
        <div class="price">অর্ডার করুন</div>
        <button onclick="addToCart('পাঠ্যবই ও গাইড',0)">🛒 কার্টে যোগ করুন</button>
      </div>
    </div>

  </div>
</section>

</main>

<footer>
  <div class="footer-content">

    <div id="about">
      <h3>ভাই ভাই লাইব্রেরী</h3>
      <p>
        বই, খাতা, কলম ও সকল শিক্ষা সামগ্রীর বিশ্বস্ত ঠিকানা।
        পাইকারি ও খুচরা বিক্রি করা হয়।
      </p>
    </div>

    <div>
      <h3>দ্রুত লিংক</h3>
      <a href="#categories">ক্যাটাগরি</a><br>
      <a href="#products">জনপ্রিয় পণ্য</a><br>
      <a href="#offers">বিশেষ অফার</a>
    </div>

    <div id="contact">
      <h3>যোগাযোগ</h3>
      <p>📍 গোসিংগা রোড, আমরাইদ বাজার, কাপাসিয়া, গাজীপুর</p>
      <p>📞 01955015589</p>
      <p>💬 WhatsApp: 01955015589</p>
    </div>

  </div>

  <div class="copyright">
    © ২০২৬ ভাই ভাই লাইব্রেরী — সর্বস্বত্ব সংরক্ষিত।
  </div>
</footer>

<div class="overlay" id="overlay" onclick="toggleCart()"></div>

<div class="cart-box" id="cartBox">
  <div class="cart-header">
    <h2>🛒 আপনার কার্ট</h2>
    <button class="close" onclick="toggleCart()">×</button>
  </div>

  <div class="cart-items" id="cartItems">
    <div class="empty">আপনার কার্ট খালি।</div>
  </div>

  <div class="cart-footer">
    <div class="total">
      <span>মোট:</span>
      <span id="totalPrice">০ টাকা</span>
    </div>

    <button class="order-btn" onclick="checkoutWhatsApp()">
      💬 WhatsApp-এ অর্ডার করুন
    </button>
  </div>
</div>

<script>
let cart = [];

function openWhatsApp(){
  window.open(
    "https://wa.me/8801955015589?text=" +
    encodeURIComponent("আসসালামু আলাইকুম, আমি ভাই ভাই লাইব্রেরী থেকে অর্ডার করতে চাই।"),
    "_blank"
  );
}

function toggleCart(){
  document.getElementById("cartBox").classList.toggle("show");
  document.getElementById("overlay").classList.toggle("show");
}

function addToCart(name,price){
  const found = cart.find(item => item.name === name);

  if(found){
    found.qty++;
  }else{
    cart.push({name:name,price:price,qty:1});
  }

  updateCart();
}

function removeItem(index){
  cart.splice(index,1);
  updateCart();
}

function changeQty(index,change){
  cart[index].qty += change;

  if(cart[index].qty <= 0){
    cart.splice(index,1);
  }

  updateCart();
}

function updateCart(){
  const items = document.getElementById("cartItems");
  const count = document.getElementById("cartCount");
  const total = document.getElementById("totalPrice");

  let totalQty = 0;
  let totalPrice = 0;

  if(cart.length === 0){
    items.innerHTML = '<div class="empty">আপনার কার্ট খালি।</div>';
  }else{
    items.innerHTML = "";

    cart.forEach((item,index)=>{
      totalQty += item.qty;
      totalPrice += item.price * item.qty;

      items.innerHTML += `
        <div class="cart-item">
          <strong>${item.name}</strong>
          <p>${item.price > 0 ? item.price + " টাকা" : "মূল্য জানতে যোগাযোগ করুন"}</p>

          <button onclick="changeQty(${index},-1)">−</button>
          <strong style="display:inline;margin:0 10px">${item.qty}</strong>
          <button onclick="changeQty(${index},1)">+</button>
          <br>
          <button onclick="removeItem(${index})">🗑️ মুছে দিন</button>
        </div>
      `;
    });
  }

  count.innerText = totalQty;
  total.innerText = totalPrice + " টাকা";
}

function checkoutWhatsApp(){
  if(cart.length === 0){
    alert("আপনার কার্ট খালি।");
    return;
  }

  let message = "🛒 নতুন অর্ডার - ভাই ভাই লাইব্রেরী\n\n";

  cart.forEach((item,index)=>{
    message += `${index+1}. ${item.name} × ${item.qty}\n`;
  });

  let total = cart.reduce((sum,item)=>sum+(item.price*item.qty),0);

  message += "\nমোট মূল্য: " + total + " টাকা";
  message += "\n\nদয়া করে আমার অর্ডারটি নিশ্চিত করুন।";

  window.open(
    "https://wa.me/8801955015589?text=" +
    encodeURIComponent(message),
    "_blank"
  );
}

function searchProducts(){
  const value = document.getElementById("searchInput").value.toLowerCase();
  const products = document.querySelectorAll(".product");

  products.forEach(product=>{
    const name = product.getAttribute("data-name").toLowerCase();

    if(name.includes(value)){
      product.style.display = "block";
    }else{
      product.style.display = "none";
    }
  });
}
</script>

</body>
</html>
