<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Meida Enterprise – Industrial & Household Chemicals</title>
<meta name="description" content="Meida Enterprise: High-quality industrial and household chemicals in Bangladesh. Bulk supply for factories." />
<style>
  body{margin:0;font-family:"Segoe UI",sans-serif;background:#f8fafc;color:#1e293b;line-height:1.6;}
  header{background:linear-gradient(135deg,#1e3a8a,#0f172a);color:#fff;text-align:center;padding:60px 20px;}
  h1{margin:0;font-size:2.5rem}
  nav{background:#fff;border-bottom:1px solid #cbd5e1;display:flex;justify-content:center;gap:30px;padding:10px 0;position:sticky;top:0}
  nav a{color:#334155;text-decoration:none;font-weight:500}
  nav a:hover{color:#1d4ed8}
  section{max-width:900px;margin:auto;padding:50px 20px}
  h2{text-align:center;font-size:1.8rem;margin-bottom:20px;color:#0f172a}
  .alert{background:#fef3c7;color:#78350f;border-left:4px solid #facc15;padding:10px 15px;border-radius:6px;margin-top:15px}
  ul{list-style:none;padding:0}
  ul li{margin:8px 0}
  .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:15px}
  .grid div{background:#fff;border:1px solid #cbd5e1;padding:15px;border-radius:8px;text-align:center;box-shadow:0 1px 2px rgba(0,0,0,.05)}
  footer{background:#0f172a;color:#94a3b8;text-align:center;padding:25px;margin-top:40px}
  @media(max-width:600px){h1{font-size:1.8rem}}
</style>
</head>
<body>
  <header>
    <h1>Meida Enterprise</h1>
    <p>ইন্ডাস্ট্রিয়াল ও হাউজহোল্ড কেমিক্যাল সরবরাহকারী</p>
  </header>

  <nav>
    <a href="#about">About</a>
    <a href="#products">Products</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="about">
    <h2>আমাদের সম্পর্কে (About Us)</h2>
    <p>
      “হ্যালো! আমরা Meida Enterprise – বহু বছর ধরে আমরা গুণগতমানসম্পন্ন ইন্ডাস্ট্রিয়াল ও হাউজহোল্ড কেমিক্যাল অফলাইনে বিক্রি করে আসছি, আর এখন আমরা আমাদের ব্যবসা অনলাইনে শুরু করেছি!”
    </p>
    <p>
      “Hello! We are Meida Enterprise – for many years we have been selling quality industrial and household chemicals offline, and now we have started our business online!”
    </p>
    <div class="alert">
      ⚠️ দয়া করে লক্ষ্য করুন — আমাদের তালিকাভুক্ত পণ্যের বাইরে অন্য কোনও পণ্য আমাদের কাছে নেই।
    </div>
  </section>

  <section id="features">
    <ul>
      <li>✅ সকল পণ্য চায়না থেকে আমদানিকৃত</li>
      <li>✅ গার্মেন্টস ও ফ্যাক্টরির জন্য বাল্ক সরবরাহ</li>
      <li>✅ দ্রুত ডেলিভারি ও নির্ভরযোগ্য মান</li>
    </ul>
  </section>

  <section id="products">
    <h2>আমাদের পণ্যসমূহ (Products)</h2>
    <div class="grid">
      <div>সফটনার / Softener</div>
      <div>লিকুইড ডিটারজেন্ট / Liquid Detergent</div>
      <div>কালার কারেক্টর এজেন্ট / Color Corrector Agent</div>
      <div>ব্লিচ লিকুইড / Bleach Liquid</div>
      <div>অয়েল রিমুভিং এজেন্ট / Oil Removing Agent</div>
      <div>কালার ফিক্সিং এজেন্ট / Color Fixing Agent</div>
      <div>সলিউবল কাটিং অয়েল / Soluble Cutting Oil</div>
      <div>কাটিং কম্পাউন্ড / Cutting Compound</div>
      <div>সিলিকন ইমলশন / Silicone Emulsion</div>
      <div>ডিসইনফেকটেন্ট লিকুইড / Disinfectant Liquid</div>
      <div>স্যানিটাইজার লিকুইড / Sanitizer Liquid</div>
      <div>অ্যান্টি রাস্ট অয়েল / Anti‑Rust Oil</div>
      <div>ওয়াটার বেসড রিলিজ এজেন্ট / Water‑Based Release Agent</div>
      <div>অয়েল বেসড রিলিজ এজেন্ট / Oil‑Based Release Agent</div>
    </div>
  </section>

  <section id="contact">
    <h2>যোগাযোগ করুন (Contact Us)</h2>
    <p style="text-align:center;font-size:1.2rem">
      📞 ০১৭৮৪ ৭৬৮১৮৩ <br>
      📍 নতুন বাজার, ঢাকা (Notun Bazar, Dhaka)
    </p>
  </section>

  <footer>
    © <span id="year"></span> Meida Enterprise. All rights reserved.
  </footer>

<script>
  document.getElementById("year").textContent=new Date().getFullYear();
  document.querySelectorAll('a[href^="#"]').forEach(l=>{
    l.addEventListener("click",e=>{
      e.preventDefault();
      document.querySelector(l.getAttribute("href")).scrollIntoView({behavior:"smooth"});
    });
  });
</script>
</body>
</html>
