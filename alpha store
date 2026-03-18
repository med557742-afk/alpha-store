alpha-store/
  index.html
  styles.css
  app.js
  images/
    photo-1.jpg
    photo-2.jpg
    photo-3.jpg<!doctype html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Alpha Store — Premium Photo Downloads</title>
  <meta name="description" content="Alpha Store — Beautiful, premium photos for personal and commercial use." />

  <!-- Elegant font (we’ll keep italic by default via CSS) -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,500;0,700;1,500;1,700&display=swap" rel="stylesheet">

  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <div class="bg" aria-hidden="true"></div>

  <header class="header">
    <nav class="nav">
      <a class="brand" href="#">
        <span class="brand__dot"></span>
        Alpha Store
      </a>

      <div class="nav__links">
        <a href="#shop">Shop</a>
        <a href="#licenses">Licenses</a>
        <a href="#faq">FAQ</a>
        <button class="btn btn--ghost" id="openCartBtn" type="button">
          Cart <span class="pill" id="cartCount">0</span>
        </button>
      </div>
    </nav>
  </header>

  <main class="container">
    <section class="hero" aria-labelledby="heroTitle">
      <div class="hero__content">
        <p class="kicker">Premium photo downloads</p>
        <h1 id="heroTitle">Alpha Store</h1>
        <p class="subtitle">
          A curated collection of high-quality photos. Buy personal or commercial licenses—download instantly.
        </p>

        <div class="hero__cta">
          <a class="btn btn--primary" href="#shop">Browse Photos</a>
          <a class="btn btn--secondary" href="#licenses">View Licenses</a>
        </div>

        <div class="trust">
          <div class="trust__item">High-res files</div>
          <div class="trust__item">Instant delivery (after payment)</div>
          <div class="trust__item">Clear licensing</div>
        </div>
      </div>

      <div class="hero__card" role="presentation">
        <div class="hero__cardInner">
          <p class="hero__cardTitle">Featured Collection</p>
          <p class="hero__cardText">Make your website, ads, and content look premium with original visuals.</p>
          <div class="hero__miniGrid">
            <img src="images/photo-1.jpg" alt="Featured photo 1" loading="lazy">
            <img src="images/photo-2.jpg" alt="Featured photo 2" loading="lazy">
            <img src="images/photo-3.jpg" alt="Featured photo 3" loading="lazy">
          </div>
        </div>
      </div>
    </section>

    <section id="shop" class="section" aria-labelledby="shopTitle">
      <div class="section__head">
        <h2 id="shopTitle">Shop Photos</h2>
        <p class="muted">Tip: Replace the sample items with your own photos and prices in <code>app.js</code>.</p>
      </div>

      <div class="grid" id="productGrid" aria-live="polite"></div>
    </section>

    <section id="licenses" class="section" aria-labelledby="licenseTitle">
      <div class="section__head">
        <h2 id="licenseTitle">Licenses</h2>
        <p class="muted">Clear usage terms help you sell confidently.</p>
      </div>

      <div class="cards">
        <article class="card">
          <h3>Personal</h3>
          <p>Use for personal projects, wallpapers, personal social posts.</p>
          <ul>
            <li>No resale or redistribution</li>
            <li>No commercial advertising</li>
          </ul>
        </article>

        <article class="card">
          <h3>Commercial</h3>
          <p>Use for business websites, marketing, client work, social media ads.</p>
          <ul>
            <li>Allowed for business promotion</li>
            <li>No “as-is” resale as stock</li>
          </ul>
        </article>

        <article class="card">
          <h3>Extended</h3>
          <p>For higher-volume campaigns and broader usage needs.</p>
          <ul>
            <li>Higher distribution allowance</li>
            <li>Ideal for agencies & brands</li>
          </ul>
        </article>
      </div>
    </section>

    <section id="faq" class="section" aria-labelledby="faqTitle">
      <div class="section__head">
        <h2 id="faqTitle">FAQ</h2>
      </div>

      <details class="faq">
        <summary>How do downloads work?</summary>
        <p>After payment, you’ll provide a download link automatically (Stripe) or manually (email). I can set up instant delivery for you.</p>
      </details>
      <details class="faq">
        <summary>Do you provide refunds?</summary>
        <p>Typically no refunds on digital downloads once delivered, but you can decide your policy.</p>
      </details>
      <details class="faq">
        <summary>Can customers request edits?</summary>
        <p>Optional: offer retouching as an upsell for extra profit.</p>
      </details>
    </section>

    <footer class="footer">
      <p>© <span id="year"></span> Alpha Store. All rights reserved.</p>
      <p class="muted">Need payments + instant delivery? Tell me: Stripe or PayPal.</p>
    </footer>
  </main>

  <!-- Lightbox -->
  <dialog class="dialog" id="lightbox">
    <button class="dialog__close" id="closeLightboxBtn" aria-label="Close preview">×</button>
    <img id="lightboxImg" alt="Preview" />
    <p class="muted" id="lightboxCaption"></p>
  </dialog>

  <!-- Cart / Checkout -->
  <dialog class="dialog" id="cartDialog">
    <button class="dialog__close" id="closeCartBtn" aria-label="Close cart">×</button>
    <h3>Your Cart</h3>
    <div id="cartItems" class="cart"></div>

    <div class="cart__total">
      <span>Total</span>
      <strong id="cartTotal">$0</strong>
    </div>

    <form id="checkoutForm" class="checkout">
      <label>
        Email (for delivery)
        <input required type="email" name="email" placeholder="you@example.com" />
      </label>

      <label>
        Notes (optional)
        <input type="text" name="notes" placeholder="Any special request?" />
      </label>

      <button class="btn btn--primary" type="submit">Proceed to Payment</button>
      <p class="muted small">
        Payment is currently a demo. I can connect Stripe/PayPal so customers can pay and auto-download.
      </p>
    </form>
  </dialog>

  <script src="app.js"></script>
</body>
</html>:root{
  --bg0:#070A12;
  --bg1:#0B1020;
  --glass: rgba(255,255,255,.08);
  --glass2: rgba(255,255,255,.12);
  --text: rgba(255,255,255,.92);
  --muted: rgba(255,255,255,.72);
  --line: rgba(255,255,255,.12);
  --accent: #9AE6FF;
  --accent2:#B8A1FF;

  --radius: 16px;
  --shadow: 0 20px 60px rgba(0,0,0,.45);
}

* { box-sizing: border-box; }
html, body { height: 100%; }

body{
  margin: 0;
  color: var(--text);
  background: radial-gradient(1200px 700px at 20% 10%, rgba(154,230,255,.10), transparent 60%),
              radial-gradient(900px 600px at 80% 20%, rgba(184,161,255,.10), transparent 55%),
              linear-gradient(180deg, var(--bg0), var(--bg1));
  font-family: "Playfair Display", serif;

  /* Italic by default (as requested) */
  font-style: italic;
}

.bg{
  position: fixed;
  inset: 0;
  pointer-events: none;
  z-index: -1;

  /* Subtle texture overlay */
  background-image:
    radial-gradient(1000px 600px at 50% 20%, rgba(255,255,255,.06), transparent 60%),
    url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='260' height='260'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='.9' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='260' height='260' filter='url(%23n)' opacity='.22'/%3E%3C/svg%3E");
  mix-blend-mode: overlay;
  opacity: .35;
}

a{ color: inherit; text-decoration: none; }
code{ font-style: normal; } /* Keep code readable */

.container{
  width: min(1100px, calc(100% - 40px));
  margin: 0 auto;
  padding: 24px 0 70px;
}

.header{
  position: sticky;
  top: 0;
  backdrop-filter: blur(14px);
  background: rgba(10, 12, 22, .55);
  border-bottom: 1px solid var(--line);
  z-index: 20;
}

.nav{
  width: min(1100px, calc(100% - 40px));
  margin: 0 auto;
  display:flex;
  align-items:center;
  justify-content: space-between;
  padding: 14px 0;
  gap: 18px;
}

.brand{
  display:flex;
  align-items:center;
  gap: 10px;
  font-weight: 700;
  letter-spacing: .3px;
}

.brand__dot{
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: linear-gradient(135deg, var(--accent), var(--accent2));
  box-shadow: 0 0 24px rgba(154,230,255,.35);
}

.nav__links{
  display:flex;
  align-items:center;
  gap: 14px;
  color: var(--muted);
}

.nav__links a:hover{ color: var(--text); }

.pill{
  display:inline-flex;
  align-items:center;
  justify-content:center;
  min-width: 24px;
  padding: 3px 8px;
  border: 1px solid var(--line);
  border-radius: 999px;
  margin-left: 8px;
  font-style: normal; /* counts look better normal */
}

.hero{
  display:grid;
  grid-template-columns: 1.2fr .8fr;
  gap: 18px;
  padding: 34px 0 14px;
}

@media (max-width: 900px){
  .hero{ grid-template-columns: 1fr; }
}

.kicker{
  color: var(--muted);
  letter-spacing: .2em;
  text-transform: uppercase;
  font-size: 12px;
  margin: 0 0 10px;
  font-style: normal; /* kicker often more readable */
}

h1{
  margin: 0;
  font-size: clamp(40px, 6vw, 62px);
  line-height: 1.05;
}

.subtitle{
  color: var(--muted);
  font-size: 18px;
  line-height: 1.5;
  margin: 14px 0 22px;
  max-width: 58ch;
}

.hero__cta{
  display:flex;
  flex-wrap: wrap;
  gap: 12px;
  margin-bottom: 18px;
}

.btn{
  border: 1px solid var(--line);
  border-radius: 999px;
  padding: 10px 14px;
  background: rgba(255,255,255,.06);
  color: var(--text);
  cursor: pointer;
  box-shadow: 0 8px 30px rgba(0,0,0,.20);
  transition: transform .12s ease, background .12s ease, border-color .12s ease;
  font-family: inherit;
  font-style: normal; /* buttons better normal for clarity */
}

.btn:hover{
  transform: translateY(-1px);
  border-color: rgba(255,255,255,.22);
  background: rgba(255,255,255,.08);
}

.btn--primary{
  background: linear-gradient(135deg, rgba(154,230,255,.20), rgba(184,161,255,.18));
  border-color: rgba(154,230,255,.25);
}

.btn--secondary{
  background: rgba(255,255,255,.06);
}

.btn--ghost{
  background: transparent;
}

.trust{
  display:flex;
  flex-wrap: wrap;
  gap: 10px;
  color: var(--muted);
}

.trust__item{
  padding: 8px 10px;
  border: 1px solid var(--line);
  background: rgba(255,255,255,.05);
  border-radius: 999px;
  font-size: 13px;
  font-style: normal;
}

.hero__card{
  border: 1px solid var(--line);
  border-radius: var(--radius);
  background: rgba(255,255,255,.06);
  box-shadow: var(--shadow);
  overflow: hidden;
}

.hero__cardInner{
  padding: 16px;
}

.hero__cardTitle{
  margin: 0 0 6px;
  font-weight: 700;
  font-style: normal;
}

.hero__cardText{
  margin: 0 0 12px;
  color: var(--muted);
  line-height: 1.5;
}

.hero__miniGrid{
  display:grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
}

.hero__miniGrid img{
  width: 100%;
  aspect-ratio: 1 / 1;
  object-fit: cover;
  border-radius: 12px;
  border: 1px solid rgba(255,255,255,.10);
}

.section{
  padding: 34px 0 0;
}

.section__head{
  display:flex;
  align-items: flex-end;
  justify-content: space-between;
  gap: 14px;
  margin-bottom: 14px;
}

.section__head h2{
  margin: 0;
  font-size: 28px;
}

.muted{ color: var(--muted); }
.small{ font-size: 13px; }

.grid{
  display:grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 14px;
}

@media (max-width: 900px){
  .grid{ grid-template-columns: repeat(2, 1fr); }
}
@media (max-width: 620px){
  .grid{ grid-template-columns: 1fr
