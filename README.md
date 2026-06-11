<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Satori SMM Panel</title>
  <meta name="description" content="Fast, simple, and professional social media services panel." />
  <style>
    :root{
      --bg:#0b1020;
      --card:#11182d;
      --card2:#16213b;
      --text:#eef2ff;
      --muted:#aab3d1;
      --line:rgba(255,255,255,.08);
      --accent:#7c3aed;
      --accent2:#22c55e;
      --shadow:0 20px 60px rgba(0,0,0,.35);
      --radius:22px;
    }
    *{box-sizing:border-box}
    html,body{margin:0;padding:0;background:
      radial-gradient(circle at top left, rgba(124,58,237,.35), transparent 35%),
      radial-gradient(circle at top right, rgba(34,197,94,.18), transparent 30%),
      linear-gradient(180deg, #070b16 0%, #0b1020 100%);
      color:var(--text);font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif}
    a{text-decoration:none;color:inherit}
    .wrap{max-width:1150px;margin:0 auto;padding:24px}
    .nav{display:flex;justify-content:space-between;align-items:center;padding:14px 0}
    .brand{display:flex;align-items:center;gap:12px;font-weight:800;font-size:20px}
    .logo{width:42px;height:42px;border-radius:14px;background:linear-gradient(135deg,var(--accent),#4f46e5);display:grid;place-items:center;box-shadow:var(--shadow)}
    .logo span{font-size:20px}
    .navlinks{display:flex;gap:18px;color:var(--muted);font-size:14px}
    .hero{display:grid;grid-template-columns:1.2fr .8fr;gap:22px;align-items:stretch;padding:34px 0 14px}
    .panel{background:rgba(17,24,45,.82);backdrop-filter:blur(12px);border:1px solid var(--line);border-radius:var(--radius);box-shadow:var(--shadow)}
    .hero-left{padding:34px}
    .tag{display:inline-flex;gap:8px;align-items:center;background:rgba(124,58,237,.14);border:1px solid rgba(124,58,237,.3);color:#ddd6fe;padding:8px 14px;border-radius:999px;font-size:13px;margin-bottom:18px}
    h1{margin:0;font-size:clamp(36px,6vw,62px);line-height:1.02}
    .grad{background:linear-gradient(90deg,#fff,#c4b5fd,#86efac);-webkit-background-clip:text;background-clip:text;color:transparent}
    .sub{color:var(--muted);font-size:17px;line-height:1.7;max-width:620px;margin:18px 0 26px}
    .actions{display:flex;gap:12px;flex-wrap:wrap}
    .btn{padding:14px 20px;border-radius:14px;font-weight:700;border:1px solid transparent;display:inline-flex;align-items:center;gap:10px}
    .btn.primary{background:linear-gradient(135deg,var(--accent),#4f46e5);box-shadow:0 12px 30px rgba(124,58,237,.28)}
    .btn.secondary{background:rgba(255,255,255,.04);border-color:var(--line);color:var(--text)}
    .hero-right{padding:24px;display:flex;flex-direction:column;justify-content:space-between}
    .statgrid{display:grid;grid-template-columns:repeat(2,1fr);gap:12px}
    .stat{background:rgba(255,255,255,.04);border:1px solid var(--line);border-radius:18px;padding:18px}
    .stat strong{display:block;font-size:26px;margin-bottom:6px}
    .stat span{color:var(--muted);font-size:13px}
    .mini{margin-top:16px;background:linear-gradient(180deg,rgba(34,197,94,.16),rgba(34,197,94,.06));border:1px solid rgba(34,197,94,.25);border-radius:18px;padding:18px}
    .mini h3{margin:0 0 8px}
    .mini p{margin:0;color:var(--muted);line-height:1.6;font-size:14px}
    .section{padding:18px 0}
    .section h2{margin:0 0 16px;font-size:28px}
    .cards{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
    .card{padding:20px;border-radius:20px;background:rgba(255,255,255,.04);border:1px solid var(--line)}
    .card .icon{width:48px;height:48px;border-radius:16px;background:rgba(124,58,237,.16);display:grid;place-items:center;margin-bottom:14px;font-size:22px}
    .card h3{margin:0 0 8px}
    .card p{margin:0;color:var(--muted);line-height:1.6;font-size:14px}
    .pricing{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
    .price{padding:24px;border-radius:22px;background:rgba(255,255,255,.04);border:1px solid var(--line)}
    .price.featured{background:linear-gradient(180deg,rgba(124,58,237,.18),rgba(255,255,255,.04));border-color:rgba(124,58,237,.35);transform:translateY(-8px)}
    .price h3{margin:0 0 8px}
    .amt{font-size:38px;font-weight:800;margin:14px 0}
    ul{margin:0;padding-left:18px;color:var(--muted);line-height:1.8}
    .footer{padding:22px 0 10px;color:var(--muted);font-size:14px;text-align:center}
    @media (max-width:900px){
      .hero,.cards,.pricing{grid-template-columns:1fr}
      .navlinks{display:none}
      .hero-left{padding:24px}
      .price.featured{transform:none}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header class="nav">
      <div class="brand">
        <div class="logo"><span>◎</span></div>
        <div>Satori Panel</div>
      </div>
      <nav class="navlinks">
        <a href="#features">Features</a>
        <a href="#services">Services</a>
        <a href="#pricing">Packages</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <main class="hero">
      <section class="panel hero-left">
        <div class="tag">Fast • Clean • Professional</div>
        <h1><span class="grad">Grow faster</span> with a modern SMM panel homepage.</h1>
        <p class="sub">
          Built for a clean, premium look with service blocks, pricing cards, and a strong call to action.
          Perfect for a free GitHub Pages landing page.
        </p>
        <div class="actions">
          <a class="btn primary" href="#pricing">View Packages</a>
          <a class="btn secondary" href="#contact">Contact Us</a>
        </div>
      </section>

      <aside class="panel hero-right">
        <div class="statgrid">
          <div class="stat"><strong>24/7</strong><span>Support style layout</span></div>
          <div class="stat"><strong>99%</strong><span>Simple UX design</span></div>
          <div class="stat"><strong>150+</strong><span>Service cards ready</span></div>
          <div class="stat"><strong>Fast</strong><span>Mobile friendly</span></div>
        </div>
        <div class="mini">
          <h3>Dashboard Preview</h3>
          <p>
            Add your own login, order, and API system later. This homepage is ready for GitHub Pages now.
          </p>
        </div>
      </aside>
    </main>

    <section class="section" id="features">
      <h2>Why choose Satori?</h2>
      <div class="cards">
        <div class="card">
          <div class="icon">⚡</div>
          <h3>Fast Landing Page</h3>
          <p>Loads quickly and looks professional on mobile and desktop.</p>
        </div>
        <div class="card">
          <div class="icon">🎨</div>
          <h3>Premium Design</h3>
          <p>Dark theme, glass effect, soft shadows, and modern gradient accents.</p>
        </div>
        <div class="card">
          <div class="icon">📱</div>
          <h3>Mobile Ready</h3>
          <p>Easy to use on phones, tablets, and computer screens.</p>
        </div>
      </div>
    </section>

    <section class="section" id="services">
      <h2>Popular Services</h2>
      <div class="cards">
        <div class="card"><h3>Instagram Followers</h3><p>Boost your social proof with a simple service block.</p></div>
        <div class="card"><h3>Facebook Likes</h3><p>Clean display for any social service category.</p></div>
        <div class="card"><h3>TikTok Views</h3><p>Easy to replace with your own services later.</p></div>
      </div>
    </section>

    <section class="section" id="pricing">
      <h2>Packages</h2>
      <div class="pricing">
        <div class="price">
          <h3>Starter</h3>
          <div class="amt">₱0</div>
          <ul>
            <li>Homepage only</li>
            <li>GitHub Pages hosted</li>
            <li>Simple design</li>
          </ul>
        </div>
        <div class="price featured">
          <h3>Pro</h3>
          <div class="amt">₱99</div>
          <ul>
            <li>More sections</li>
            <li>Better branding</li>
            <li>Custom content</li>
          </ul>
        </div>
        <div class="price">
          <h3>Business</h3>
          <div class="amt">₱199</div>
          <ul>
            <li>Full panel look</li>
            <li>Strong CTA buttons</li>
            <li>Ready for expansion</li>
          </ul>
        </div>
      </div>
    </section>

    <section class="section" id="contact">
      <div class="panel" style="padding:24px;text-align:center">
        <h2 style="margin:0 0 10px">Ready to build your panel?</h2>
        <p style="margin:0;color:var(--muted)">This is the free homepage version. You can edit text, colors, and links anytime.</p>
      </div>
    </section>

    <div class="footer">© 2026 Satori Panel. All rights reserved.</div>
  </div>
</body>
</html>
