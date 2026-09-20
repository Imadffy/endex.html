<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>z4yd parfums — عطور فاخرة</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Reem+Kufi:wght@400..700&family=Tajawal:wght@300;400;500;700&display=swap" rel="stylesheet">
<style>
  :root{
    --bg: #12102A;
    --bg-card: #1C1940;
    --bg-card-hover: #241F52;
    --gold: #C9A227;
    --gold-soft: #E3C568;
    --amber: #2E2A5C;
    --cream: #F1EEE6;
    --muted: #9C97B8;
    --line: #2C2757;
    --radius: 2px;
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    background:var(--bg);
    color:var(--cream);
    font-family:'Tajawal',sans-serif;
    font-weight:400;
    line-height:1.7;
    overflow-x:hidden;
  }
  h1,h2,h3,.display{
    font-family:'Reem Kufi',sans-serif;
    font-weight:600;
    letter-spacing:.5px;
  }
  a{color:inherit;text-decoration:none;}
  img{display:block;max-width:100%;}
  .wrap{
    width:100%;
    max-width:1180px;
    margin:0 auto;
    padding:0 28px;
  }

  /* subtle noise/texture backdrop */
  body::before{
    content:"";
    position:fixed;
    inset:0;
    background:
      radial-gradient(ellipse 900px 500px at 85% -5%, rgba(198,149,44,.10), transparent 60%),
      radial-gradient(ellipse 700px 500px at -10% 40%, rgba(72,60,140,.18), transparent 60%);
    pointer-events:none;
    z-index:0;
  }

  /* ===== Header ===== */
  header{
    position:sticky;
    top:0;
    z-index:50;
    background:rgba(19,15,11,.88);
    backdrop-filter:blur(10px);
    border-bottom:1px solid var(--line);
  }
  header .wrap{
    display:flex;
    align-items:center;
    justify-content:space-between;
    height:78px;
  }
  .brand{
    display:flex;
    align-items:baseline;
    gap:10px;
  }
  .brand-mark{
    font-family:'Reem Kufi',sans-serif;
    font-size:24px;
    color:var(--cream);
  }
  .brand-mark span{color:var(--gold);}
  .brand-sub{
    font-size:11px;
    color:var(--muted);
    letter-spacing:2px;
  }
  nav{display:flex;gap:34px;font-size:15px;}
  nav a{color:var(--muted);transition:color .25s;position:relative;}
  nav a:hover{color:var(--cream);}
  .header-cta{
    display:flex;
    align-items:center;
    gap:8px;
    background:transparent;
    border:1px solid var(--gold);
    color:var(--gold-soft);
    padding:9px 20px;
    border-radius:var(--radius);
    font-size:14px;
    transition:all .25s;
    white-space:nowrap;
  }
  .header-cta:hover{background:var(--gold);color:#171310;}
  .menu-toggle{display:none;}

  /* ===== Hero ===== */
  .hero{
    position:relative;
    z-index:1;
    padding:90px 0 70px;
    display:grid;
    grid-template-columns:1.1fr .9fr;
    gap:40px;
    align-items:center;
  }
  .hero-eyebrow{
    color:var(--gold);
    font-size:14px;
    margin-bottom:18px;
  }
  .hero h1{
    font-size:56px;
    line-height:1.25;
    color:var(--cream);
    max-width:560px;
  }
  .hero p{
    margin-top:22px;
    max-width:460px;
    color:var(--muted);
    font-size:16px;
  }
  .hero-actions{
    margin-top:38px;
    display:flex;
    gap:16px;
    flex-wrap:wrap;
  }
  .btn-primary{
    background:var(--gold);
    color:#171310;
    padding:15px 30px;
    border-radius:var(--radius);
    font-size:15px;
    font-weight:700;
    display:inline-flex;
    align-items:center;
    gap:10px;
    transition:transform .25s, box-shadow .25s;
  }
  .btn-primary:hover{transform:translateY(-2px);box-shadow:0 10px 30px -10px rgba(198,149,44,.6);}
  .btn-ghost{
    border:1px solid var(--line);
    color:var(--cream);
    padding:15px 30px;
    border-radius:var(--radius);
    font-size:15px;
    transition:border-color .25s;
  }
  .btn-ghost:hover{border-color:var(--gold);}

  .hero-art{
    position:relative;
    display:flex;
    justify-content:center;
    align-items:center;
  }
  .hero-art svg{width:100%;max-width:340px;}

  /* ===== Marquee strip ===== */
  .marquee{
    border-top:1px solid var(--line);
    border-bottom:1px solid var(--line);
    overflow:hidden;
    background:var(--bg-card);
    position:relative;
    z-index:1;
  }
  .marquee-track{
    display:flex;
    gap:60px;
    white-space:nowrap;
    padding:16px 0;
    animation:scroll 28s linear infinite;
    width:max-content;
  }
  .marquee-track span{
    font-family:'Reem Kufi',sans-serif;
    font-size:14px;
    color:var(--muted);
    letter-spacing:1px;
  }
  @keyframes scroll{
    from{transform:translateX(0);}
    to{transform:translateX(-50%);}
  }
  @media (prefers-reduced-motion: reduce){
    .marquee-track{animation:none;}
  }

  /* ===== Gallery ===== */
  .section{
    position:relative;
    z-index:1;
    padding:100px 0 40px;
  }
  .section-head{
    display:flex;
    justify-content:space-between;
    align-items:flex-end;
    margin-bottom:46px;
    flex-wrap:wrap;
    gap:16px;
  }
  .section-head h2{
    font-size:36px;
    color:var(--cream);
  }
  .section-head p{
    color:var(--muted);
    max-width:380px;
    font-size:15px;
  }

  .grid{
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(260px, 1fr));
    gap:26px;
  }
  .card{
    background:var(--bg-card);
    border:1px solid var(--line);
    border-radius:var(--radius);
    padding:30px 26px 26px;
    display:flex;
    flex-direction:column;
    transition:border-color .3s, background .3s;
  }
  .card:hover{border-color:var(--gold);background:var(--bg-card-hover);}
  .card-art{
    height:190px;
    display:flex;
    align-items:center;
    justify-content:center;
    margin-bottom:22px;
    background:linear-gradient(160deg, #F1EEE6, #DCD8EC);
    border-radius:6px;
    padding:14px;
  }
  .card-art img{
    max-height:100%;
    max-width:100%;
    object-fit:contain;
    mix-blend-mode:multiply;
  }
  .card-art svg{height:170px;}
  .card-cat{
    font-size:12px;
    color:var(--gold);
    margin-bottom:8px;
    letter-spacing:1px;
  }
  .card h3{
    font-size:21px;
    color:var(--cream);
    margin-bottom:8px;
  }
  .card-notes{
    color:var(--muted);
    font-size:13.5px;
    margin-bottom:20px;
  }
  .size-row{
    display:flex;
    gap:10px;
    margin-bottom:18px;
  }
  .size-chip{
    flex:1;
    background:var(--bg);
    border:1px solid var(--line);
    border-radius:var(--radius);
    padding:8px 10px;
    display:flex;
    flex-direction:column;
    align-items:center;
    gap:2px;
  }
  .size-chip-label{
    font-size:12px;
    color:var(--muted);
  }
  .size-chip-price{
    font-family:'Reem Kufi',sans-serif;
    font-size:15px;
    color:var(--gold-soft);
  }
  .card-footer{
    margin-top:auto;
    display:flex;
    align-items:center;
    justify-content:space-between;
    border-top:1px solid var(--line);
    padding-top:18px;
  }
  .price{
    font-family:'Reem Kufi',sans-serif;
    font-size:19px;
    color:var(--gold-soft);
  }
  .price sup{font-size:12px;color:var(--muted);margin-right:4px;}
  .order-btn{
    display:flex;
    align-items:center;
    gap:8px;
    background:#1F2B22;
    color:#8FE0A6;
    border:1px solid #2C4A34;
    padding:9px 16px;
    border-radius:var(--radius);
    font-size:13px;
    transition:all .25s;
  }
  .order-btn:hover{background:#2C4A34;}
  .order-btn svg{width:15px;height:15px;fill:currentColor;}

  /* ===== About strip ===== */
  .about{
    position:relative;
    z-index:1;
    padding:100px 0;
    border-top:1px solid var(--line);
    display:grid;
    grid-template-columns:.9fr 1.1fr;
    gap:60px;
    align-items:center;
  }
  .about-figure{
    aspect-ratio:4/5;
    background:
      linear-gradient(160deg, #211C46, #100D24 70%);
    border:1px solid var(--line);
    border-radius:var(--radius);
    display:flex;
    align-items:center;
    justify-content:center;
  }
  .about-figure svg{width:60%;}
  .about h2{
    font-size:32px;
    margin-bottom:22px;
    color:var(--cream);
  }
  .about p{
    color:var(--muted);
    margin-bottom:16px;
    max-width:520px;
    font-size:15.5px;
  }
  .stats{
    display:flex;
    gap:44px;
    margin-top:34px;
  }
  .stat b{
    display:block;
    font-family:'Reem Kufi',sans-serif;
    font-size:28px;
    color:var(--gold);
  }
  .stat span{font-size:13px;color:var(--muted);}

  /* ===== Contact / CTA ===== */
  .cta{
    position:relative;
    z-index:1;
    margin:60px 0 0;
    padding:80px 0;
    text-align:center;
    border-top:1px solid var(--line);
    background:radial-gradient(ellipse 700px 300px at 50% 0%, rgba(198,149,44,.08), transparent 70%);
  }
  .cta h2{
    font-size:34px;
    color:var(--cream);
    margin-bottom:16px;
  }
  .cta p{
    color:var(--muted);
    max-width:440px;
    margin:0 auto 34px;
    font-size:15px;
  }

  /* ===== Footer ===== */
  footer{
    position:relative;
    z-index:1;
    border-top:1px solid var(--line);
    padding:44px 0 30px;
  }
  footer .wrap{
    display:flex;
    justify-content:space-between;
    align-items:center;
    flex-wrap:wrap;
    gap:18px;
  }
  .foot-links{display:flex;gap:26px;font-size:14px;color:var(--muted);}
  .foot-links a:hover{color:var(--gold-soft);}
  .foot-copy{font-size:13px;color:#6B5F4C;}

  /* ===== Floating WhatsApp ===== */
  .float-wa{
    position:fixed;
    left:24px;
    bottom:24px;
    z-index:100;
    width:58px;
    height:58px;
    border-radius:50%;
    background:#25D366;
    display:flex;
    align-items:center;
    justify-content:center;
    box-shadow:0 10px 30px -8px rgba(37,211,102,.6);
    transition:transform .25s;
  }
  .float-wa:hover{transform:scale(1.08);}
  .float-wa svg{width:28px;height:28px;fill:#0d1a12;}

  /* ===== Responsive ===== */
  @media (max-width: 900px){
    .hero{grid-template-columns:1fr;padding-top:50px;}
    .hero h1{font-size:40px;}
    .hero-art{order:-1;}
    .grid{grid-template-columns:repeat(2,1fr);}
    .about{grid-template-columns:1fr;}
    nav{display:none;}
  }
  @media (max-width: 560px){
    .grid{grid-template-columns:1fr;}
    .hero h1{font-size:32px;}
    .section-head{flex-direction:column;align-items:flex-start;}
    .stats{gap:26px;}
  }
</style>
</head>
<body>

<header>
  <div class="wrap">
    <div class="brand">
      <span class="brand-mark">z4yd <span>parfums</span></span>
    </div>
    <nav>
      <a href="#gallery">المجموعة</a>
      <a href="#about">قصتنا</a>
      <a href="#contact">تواصل معنا</a>
    </nav>
    <a class="header-cta" id="headerWa" href="#" target="_blank" rel="noopener">
      اطلب عبر واتساب
    </a>
  </div>
</header>

<section class="hero wrap">
  <div>
    <div class="hero-eyebrow">عطور أصيلة — تركيبات فاخرة</div>
    <h1>عطرك يبقى في الذاكرة قبل أن تُرى</h1>
    <p>z4yd parfums تقدم مجموعة مختارة من العطور الفاخرة، بروائح تدوم طويلاً وتركيبات مستوحاة من التقاليد العريقة لصناعة العطور. اكتشف عطرك المفضل واطلبه بسهولة عبر واتساب.</p>
    <div class="hero-actions">
      <a href="#gallery" class="btn-primary">
        تصفح المجموعة
      </a>
      <a href="#about" class="btn-ghost">قصة العلامة</a>
    </div>
  </div>
  <div class="hero-art">
    <svg viewBox="0 0 200 320" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <linearGradient id="bottleMain" x1="0" y1="0" x2="1" y2="1">
          <stop offset="0%" stop-color="#E3C568"/>
          <stop offset="100%" stop-color="#2E2A5C"/>
        </linearGradient>
      </defs>
      <rect x="70" y="20" width="60" height="34" rx="4" fill="#C9A227"/>
      <rect x="85" y="4" width="30" height="20" rx="3" fill="#E3C568"/>
      <path d="M55 60 h90 a10 10 0 0 1 10 10 v210 a20 20 0 0 1 -20 20 h-70 a20 20 0 0 1 -20 -20 v-210 a10 10 0 0 1 10 -10 z" fill="url(#bottleMain)" opacity="0.9"/>
      <rect x="60" y="150" width="80" height="70" fill="#12102A" opacity="0.25"/>
      <text x="100" y="190" text-anchor="middle" font-family="Reem Kufi" font-size="16" fill="#12102A" opacity="0.7">z4yd</text>
    </svg>
  </div>
</section>

<div class="marquee">
  <div class="marquee-track">
    <span>عطور فاخرة</span><span>◆</span><span>ثبات يدوم طويلاً</span><span>◆</span><span>التوصيل 35 د.م.</span><span>◆</span><span>طلب مباشر عبر واتساب</span><span>◆</span>
    <span>عطور فاخرة</span><span>◆</span><span>ثبات يدوم طويلاً</span><span>◆</span><span>التوصيل 35 د.م.</span><span>◆</span><span>طلب مباشر عبر واتساب</span><span>◆</span>
  </div>
</div>

<section class="section wrap" id="gallery">
  <div class="section-head">
    <h2>مجموعتنا</h2>
    <p>كل عطر مصمم بعناية ليعكس شخصية مختلفة — من الروائح الشرقية الدافئة إلى النفحات الزهرية المنعشة.</p>
  </div>
  <div class="grid" id="productGrid"></div>
</section>

<section class="about wrap" id="about">
  <div class="about-figure">
    <svg viewBox="0 0 120 150" xmlns="http://www.w3.org/2000/svg">
      <circle cx="60" cy="75" r="45" fill="none" stroke="#C9A227" stroke-width="1"/>
      <rect x="40" y="35" width="40" height="55" rx="6" fill="#2E2A5C" opacity="0.85"/>
      <rect x="50" y="20" width="20" height="18" rx="3" fill="#C9A227"/>
    </svg>
  </div>
  <div>
    <h2>عن z4yd parfums</h2>
    <p>وُلدت z4yd parfums من شغف حقيقي بفن العطور، وسعي دائم لتقديم روائح تحمل طابعاً مميزاً وتدوم من الصباح حتى المساء. نختار مكوناتنا بعناية، ونجمع بين الأصالة والحداثة في كل قارورة.</p>
    <p>نؤمن أن العطر ليس مجرد رائحة، بل توقيع شخصي يرافقك أينما ذهبت.</p>
    <div class="stats">
      <div class="stat"><b>+15</b><span>عطر متوفر</span></div>
      <div class="stat"><b>100%</b><span>مكونات مختارة</span></div>
      <div class="stat"><b>24س</b><span>الرد على الطلبات</span></div>
    </div>
  </div>
</section>

<section class="cta" id="contact">
  <div class="wrap">
    <h2>جاهز تختار عطرك؟</h2>
    <p>تواصل معنا مباشرة عبر واتساب لطلب أي عطر من المجموعة، أو للاستفسار عن التوفر والأسعار.</p>
    <a class="btn-primary" id="ctaWa" href="#" target="_blank" rel="noopener">
      تواصل معنا عبر واتساب
    </a>
  </div>
</section>

<footer>
  <div class="wrap">
    <span class="brand-mark" style="font-size:18px;">z4yd <span>parfums</span></span>
    <div class="foot-links">
      <a href="#gallery">المجموعة</a>
      <a href="#about">قصتنا</a>
      <a href="#contact">تواصل معنا</a>
    </div>
    <span class="foot-copy">© 2026 z4yd parfums. جميع الحقوق محفوظة.</span>
  </div>
</footer>

<a class="float-wa" id="floatWa" href="#" target="_blank" rel="noopener" aria-label="تواصل عبر واتساب">
  <svg viewBox="0 0 32 32"><path d="M16.001 3C9.107 3 3.5 8.607 3.5 15.5c0 2.457.72 4.744 1.96 6.67L3 29l7.02-2.42a12.44 12.44 0 0 0 5.98 1.52C22.895 28.1 28.5 22.493 28.5 15.6 28.5 8.706 22.895 3 16.001 3zm0 22.7a10.16 10.16 0 0 1-5.19-1.42l-.372-.22-4.166 1.437 1.36-4.06-.242-.396a10.14 10.14 0 0 1-1.59-5.44c0-5.61 4.56-10.17 10.2-10.17 5.638 0 10.2 4.56 10.2 10.17 0 5.61-4.562 10.17-10.2 10.17zm5.59-7.63c-.306-.153-1.81-.893-2.09-.995-.28-.102-.484-.153-.688.153-.204.306-.79.995-.97 1.2-.178.204-.356.23-.662.077-.306-.153-1.293-.477-2.463-1.52-.91-.812-1.524-1.815-1.703-2.12-.178-.306-.02-.472.134-.624.137-.137.306-.357.46-.535.153-.178.204-.306.306-.51.102-.204.05-.383-.026-.535-.077-.153-.688-1.657-.943-2.27-.248-.596-.5-.515-.688-.524l-.586-.01c-.204 0-.535.077-.815.383-.28.306-1.07 1.046-1.07 2.55s1.096 2.958 1.25 3.163c.153.204 2.157 3.293 5.227 4.617.73.315 1.3.503 1.744.644.733.233 1.4.2 1.928.121.588-.088 1.81-.74 2.065-1.454.255-.714.255-1.326.178-1.454-.076-.128-.28-.204-.586-.357z"/></svg>
</a>

<script>
  // ===== EDIT THIS: your WhatsApp number in international format, no + or spaces =====
  const WHATSAPP_NUMBER = "212656363971";
  // ===== EDIT THIS: delivery fee shown on the site and in the WhatsApp message =====
  const DELIVERY_FEE = "35";

  // ===== EDIT THIS: your products list =====
  const products = [
    {
      name: "Le Beau Le Parfum",
      brand: "Jean Paul Gaultier",
      category: "شرقي / خشبي",
      notes: "جوز الهند، الفانيليا، خشب الأرز",
      sizes: [{ label: "5ml", price: "50" }, { label: "10ml", price: "100" }],
      image: "image1.jpg"
    },
    {
      name: "Le Beau EDT",
      brand: "Jean Paul Gaultier",
      category: "منعش / خشبي",
      notes: "جوز الهند، البرغموت، خشب الصندل",
      sizes: [{ label: "5ml", price: "50" }, { label: "10ml", price: "100" }],
      image: "image2.jpg"
    },
    {
      name: "Born In Roma Coral Fantasy Uomo",
      brand: "Valentino",
      category: "شرقي / حار",
      notes: "فلفل وردي، خشب الأرز، مسك",
      sizes: [{ label: "5ml", price: "60" }, { label: "10ml", price: "120" }],
      image: "image3.jpg"
    },
    {
      name: "Stronger With You Intensely",
      brand: "Emporio Armani",
      category: "شرقي / حلو",
      notes: "كاكاو، فانيليا، خزامى",
      sizes: [{ label: "5ml", price: "50" }, { label: "10ml", price: "100" }],
      image: "image4.jpg"
    }
  ];

  function waLink(productName){
    const msg = encodeURIComponent(`السلام عليكم، بغيت نطلب عطر "${productName}" من z4yd parfums.`);
    return `https://wa.me/${WHATSAPP_NUMBER}?text=${msg}`;
  }

  function bottleSVG(c1, c2){
    return `
    <svg viewBox="0 0 200 320" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <linearGradient id="g${c1.replace('#','')}" x1="0" y1="0" x2="1" y2="1">
          <stop offset="0%" stop-color="${c1}"/>
          <stop offset="100%" stop-color="${c2}"/>
        </linearGradient>
      </defs>
      <rect x="75" y="18" width="50" height="30" rx="4" fill="${c2}"/>
      <rect x="88" y="4" width="24" height="18" rx="3" fill="${c1}"/>
      <path d="M60 55 h80 a9 9 0 0 1 9 9 v190 a18 18 0 0 1 -18 18 h-62 a18 18 0 0 1 -18 -18 v-190 a9 9 0 0 1 9 -9 z" fill="url(#g${c1.replace('#','')})" opacity="0.92"/>
      <rect x="65" y="140" width="70" height="60" fill="#12102A" opacity="0.22"/>
    </svg>`;
  }

  const grid = document.getElementById('productGrid');
  products.forEach(p => {
    const card = document.createElement('div');
    card.className = 'card';

    let sizesHtml = '';
    if (p.sizes && p.sizes.length) {
      sizesHtml = `<div class="size-row">` + p.sizes.map(s =>
        `<div class="size-chip"><span class="size-chip-label">${s.label}</span><span class="size-chip-price">${s.price} د.م.</span></div>`
      ).join('') + `</div>`;
    } else if (p.price && p.price !== "0") {
      sizesHtml = `<div class="price">${p.price} <sup>د.م.</sup></div>`;
    } else {
      sizesHtml = `<div class="price" style="font-size:14px;color:var(--muted);">السعر عند الطلب</div>`;
    }

    const fullName = p.brand ? p.brand + ' ' + p.name : p.name;
    const orderMsg = p.sizes && p.sizes.length
      ? `${fullName} — المقاسات: ${p.sizes.map(s => s.label + ' (' + s.price + ' د.م.)').join(' / ')} (+ ${DELIVERY_FEE} د.م. توصيل)`
      : fullName;

    card.innerHTML = `
      <div class="card-art">${p.image ? `<img src="${p.image}" alt="${p.name}" style="max-height:100%;object-fit:contain;">` : bottleSVG(p.color1, p.color2)}</div>
      <div class="card-cat">${p.brand ? p.brand + ' — ' : ''}${p.category}</div>
      <h3>${p.name}</h3>
      <div class="card-notes">${p.notes}</div>
      ${sizesHtml}
      <div class="card-footer" style="flex-direction:column;align-items:stretch;gap:10px;">
        <a class="order-btn" target="_blank" rel="noopener" href="${waLink(orderMsg)}" style="width:100%;justify-content:center;">
          <svg viewBox="0 0 32 32"><path d="M16.001 3C9.107 3 3.5 8.607 3.5 15.5c0 2.457.72 4.744 1.96 6.67L3 29l7.02-2.42a12.44 12.44 0 0 0 5.98 1.52C22.895 28.1 28.5 22.493 28.5 15.6 28.5 8.706 22.895 3 16.001 3z"/></svg>
          اطلب عبر واتساب
        </a>
        <div style="text-align:center;font-size:12.5px;color:var(--muted);">+ ${DELIVERY_FEE} د.م. رسوم التوصيل</div>
      </div>
    `;
    grid.appendChild(card);
  });

  const generalLink = waLink('استفسار عام');
  document.getElementById('headerWa').href = generalLink;
  document.getElementById('ctaWa').href = generalLink;
  document.getElementById('floatWa').href = generalLink;
</script>

</body>
</html>

