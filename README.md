<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>JOJO Digital — Sri Kumar M | AI-Powered Web & Design Studio</title>
<meta name="description" content="JOJO Digital — AI-powered web design, development, and creative services for local businesses in Hosur, Tamil Nadu.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@600;700;800&family=Plus+Jakarta+Sans:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root{
    --navy-900:#0d1b2b;
    --navy-800:#132b45;
    --navy-700:#1e3a5f;
    --navy-600:#2a4d78;
    --gold:#d4af37;
    --gold-soft:#e8cd7a;
    --ink:#eef2f7;
    --ink-dim:#a8b6c9;
    --glass:rgba(255,255,255,0.05);
    --glass-border:rgba(212,175,55,0.18);
    --radius:18px;
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    background:
      radial-gradient(1200px 700px at 85% -10%, rgba(212,175,55,0.10), transparent 60%),
      radial-gradient(900px 600px at 5% 20%, rgba(42,77,120,0.35), transparent 55%),
      var(--navy-900);
    color:var(--ink);
    font-family:'Plus Jakarta Sans', sans-serif;
    line-height:1.6;
    overflow-x:hidden;
  }
  a{color:inherit;text-decoration:none;}
  .wrap{max-width:1120px;margin:0 auto;padding:0 24px;}
  h1,h2,h3{font-family:'Syne',sans-serif;letter-spacing:-0.01em;}

  /* NAV */
  nav{
    position:fixed;top:0;left:0;right:0;z-index:50;
    backdrop-filter:blur(14px);
    background:rgba(13,27,43,0.65);
    border-bottom:1px solid var(--glass-border);
  }
  nav .wrap{display:flex;align-items:center;justify-content:space-between;height:72px;}
  .brand{display:flex;align-items:center;gap:10px;font-family:'Syne',sans-serif;font-weight:700;font-size:1.15rem;}
  .brand .dot{width:9px;height:9px;border-radius:50%;background:var(--gold);box-shadow:0 0 12px var(--gold);}
  nav .links{display:flex;gap:32px;font-size:0.92rem;color:var(--ink-dim);}
  nav .links a:hover{color:var(--gold-soft);}
  .nav-cta{
    padding:10px 20px;border-radius:100px;
    background:linear-gradient(135deg,var(--gold),var(--gold-soft));
    color:var(--navy-900);font-weight:600;font-size:0.88rem;
  }
  @media(max-width:760px){ nav .links{display:none;} }

  /* HERO */
  header.hero{padding:170px 0 90px;position:relative;}
  .eyebrow{
    display:inline-flex;align-items:center;gap:8px;
    font-family:'JetBrains Mono',monospace;font-size:0.78rem;
    color:var(--gold-soft);letter-spacing:0.08em;text-transform:uppercase;
    border:1px solid var(--glass-border);padding:6px 14px;border-radius:100px;
    background:var(--glass);margin-bottom:24px;
  }
  .hero-grid{display:grid;grid-template-columns:1.15fr 0.85fr;gap:56px;align-items:center;}
  @media(max-width:860px){.hero-grid{grid-template-columns:1fr;}}
  h1.title{font-size:3.4rem;font-weight:800;line-height:1.08;margin-bottom:22px;}
  h1.title .accent{color:var(--gold);}
  .sub{font-size:1.08rem;color:var(--ink-dim);max-width:480px;margin-bottom:34px;}
  .hero-actions{display:flex;gap:16px;flex-wrap:wrap;}
  .btn-primary{
    padding:14px 28px;border-radius:100px;font-weight:600;font-size:0.95rem;
    background:linear-gradient(135deg,var(--gold),var(--gold-soft));color:var(--navy-900);
    box-shadow:0 8px 24px rgba(212,175,55,0.25);
  }
  .btn-ghost{
    padding:14px 28px;border-radius:100px;font-weight:600;font-size:0.95rem;
    border:1px solid var(--glass-border);color:var(--ink);
  }

  /* Terminal signature element */
  .terminal{
    background:var(--navy-800);border:1px solid var(--glass-border);
    border-radius:var(--radius);overflow:hidden;
    box-shadow:0 30px 60px -20px rgba(0,0,0,0.6);
  }
  .terminal-bar{
    display:flex;align-items:center;gap:8px;padding:12px 16px;
    background:rgba(0,0,0,0.2);border-bottom:1px solid var(--glass-border);
  }
  .terminal-bar span{width:10px;height:10px;border-radius:50%;}
  .terminal-bar span:nth-child(1){background:#ff5f56;}
  .terminal-bar span:nth-child(2){background:#ffbd2e;}
  .terminal-bar span:nth-child(3){background:#27c93f;}
  .terminal-body{padding:22px;font-family:'JetBrains Mono',monospace;font-size:0.84rem;color:var(--ink-dim);min-height:230px;}
  .terminal-body .line{margin-bottom:10px;}
  .terminal-body .prompt{color:var(--gold-soft);}
  .terminal-body .ok{color:#6ee7b7;}
  .cursor{display:inline-block;width:7px;height:14px;background:var(--gold-soft);animation:blink 1s step-end infinite;vertical-align:middle;}
  @keyframes blink{50%{opacity:0;}}

  /* SECTION shared */
  section{padding:110px 0;position:relative;}
  .section-head{margin-bottom:56px;max-width:620px;}
  .section-head .eyebrow{margin-bottom:16px;}
  .section-head h2{font-size:2.2rem;font-weight:700;margin-bottom:14px;}
  .section-head p{color:var(--ink-dim);font-size:1.02rem;}

  /* ABOUT */
  .about-grid{display:grid;grid-template-columns:1fr 1fr;gap:48px;align-items:start;}
  @media(max-width:860px){.about-grid{grid-template-columns:1fr;}}
  .about-card{
    background:var(--glass);border:1px solid var(--glass-border);border-radius:var(--radius);
    padding:32px;
  }
  .about-card h3{font-size:1.1rem;margin-bottom:10px;color:var(--gold-soft);}
  .about-card p{color:var(--ink-dim);font-size:0.96rem;}
  .tag-row{display:flex;flex-wrap:wrap;gap:10px;margin-top:22px;}
  .tag{
    font-family:'JetBrains Mono',monospace;font-size:0.76rem;color:var(--ink-dim);
    border:1px solid var(--glass-border);border-radius:100px;padding:6px 12px;
  }

  /* SERVICES */
  .services-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:24px;}
  @media(max-width:860px){.services-grid{grid-template-columns:1fr;}}
  .service-card{
    background:var(--glass);border:1px solid var(--glass-border);border-radius:var(--radius);
    padding:30px;transition:transform 0.25s ease, border-color 0.25s ease;
  }
  .service-card:hover{transform:translateY(-6px);border-color:var(--gold);}
  .service-card.featured{border-color:var(--gold);position:relative;}
  .service-card .badge{
    position:absolute;top:-12px;right:24px;background:var(--gold);color:var(--navy-900);
    font-size:0.7rem;font-weight:700;padding:4px 12px;border-radius:100px;
    font-family:'JetBrains Mono',monospace;letter-spacing:0.04em;
  }
  .service-card .price{font-family:'Syne',sans-serif;font-size:2rem;font-weight:800;color:var(--gold-soft);margin:12px 0 4px;}
  .service-card .price span{font-size:0.9rem;font-weight:500;color:var(--ink-dim);}
  .service-card h3{font-size:1.15rem;margin-bottom:6px;}
  .service-card ul{list-style:none;margin-top:18px;color:var(--ink-dim);font-size:0.9rem;}
  .service-card li{padding:7px 0;border-top:1px solid var(--glass-border);}
  .service-card li:first-child{border-top:none;}

  /* WORK */
  .work-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:24px;}
  @media(max-width:860px){.work-grid{grid-template-columns:1fr;}}
  .work-card{
    border-radius:var(--radius);overflow:hidden;border:1px solid var(--glass-border);
    background:var(--navy-800);
  }
  .work-thumb{
    height:150px;display:flex;align-items:center;justify-content:center;
    font-family:'Syne',sans-serif;font-weight:700;font-size:1.3rem;color:var(--navy-900);
  }
  .work-card:nth-child(1) .work-thumb{background:linear-gradient(135deg,#8b0000,#1a1a1a);color:#fff;}
  .work-card:nth-child(2) .work-thumb{background:linear-gradient(135deg,#1e3a5f,#3a6ea5);color:#fff;}
  .work-card:nth-child(3) .work-thumb{background:linear-gradient(135deg,#0f4c4c,#1c7a7a);color:#fff;}
  .work-info{padding:20px;}
  .work-info h3{font-size:1.02rem;margin-bottom:6px;}
  .work-info p{color:var(--ink-dim);font-size:0.86rem;}

  /* CONTACT */
  .contact-card{
    background:linear-gradient(135deg, rgba(212,175,55,0.08), rgba(30,58,95,0.3));
    border:1px solid var(--glass-border);border-radius:24px;
    padding:56px;text-align:center;
  }
  .contact-card h2{font-size:2rem;margin-bottom:14px;}
  .contact-card p{color:var(--ink-dim);margin-bottom:32px;max-width:480px;margin-left:auto;margin-right:auto;}
  .contact-links{display:flex;justify-content:center;gap:16px;flex-wrap:wrap;}
  .contact-links a{
    display:flex;align-items:center;gap:8px;
    padding:12px 22px;border-radius:100px;border:1px solid var(--glass-border);
    font-size:0.9rem;font-weight:600;color:var(--ink);
  }
  .contact-links a.primary{
    background:linear-gradient(135deg,var(--gold),var(--gold-soft));color:var(--navy-900);border:none;
  }
  .contact-links a:hover{border-color:var(--gold);}

  footer{padding:36px 0;border-top:1px solid var(--glass-border);text-align:center;color:var(--ink-dim);font-size:0.85rem;}

  @media (prefers-reduced-motion: reduce){
    html{scroll-behavior:auto;}
    .cursor{animation:none;opacity:1;}
  }
</style>
</head>
<body>

<nav>
  <div class="wrap">
    <div class="brand"><span class="dot"></span> JOJO Digital</div>
    <div class="links">
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#work">Work</a>
      <a href="#contact">Contact</a>
    </div>
    <a class="nav-cta" href="https://wa.me/918248128329?text=Hi%2C%20I%27m%20interested%20in%20your%20work%20and%20would%20like%20to%20work%20with%20you." target="_blank">WhatsApp Us</a>
  </div>
</nav>

<header class="hero">
  <div class="wrap hero-grid">
    <div>
      <div class="eyebrow">● Hosur, Tamil Nadu — Agentic AI Studio</div>
      <h1 class="title">Websites your business<br> can actually <span class="accent">show up with.</span></h1>
      <p class="sub">JOJO Digital builds AI-powered websites, brand assets, and video content for local businesses — designed, coded, and shipped by one person, fast.</p>
      <div class="hero-actions">
        <a class="btn-primary" href="#services">See pricing</a>
        <a class="btn-ghost" href="#work">View live demos</a>
      </div>
    </div>
    <div class="terminal">
      <div class="terminal-bar"><span></span><span></span><span></span></div>
      <div class="terminal-body" id="termBody"></div>
    </div>
  </div>
</header>

<section id="about">
  <div class="wrap">
    <div class="section-head">
      <div class="eyebrow">About</div>
      <h2>One founder. One stack. Real results.</h2>
      <p>JOJO Digital is run by Sri Kumar M — a BCA student, NSS Programme Officer, and self-taught AI/web developer building practical digital tools for businesses that don't have the time or budget for a big agency.</p>
    </div>
    <div class="about-grid">
      <div class="about-card">
        <h3>Who I am</h3>
        <p>2nd year BCA student at M.G.R. College, Hosur (Periyar University), and NSS Programme Officer on campus. I picked up web design, AI development, and prompt engineering by building — not just studying — and I run JOJO Digital as a one-person studio serving local businesses around Hosur.</p>
        <div class="tag-row">
          <span class="tag">HTML / CSS / JS</span>
          <span class="tag">AI-Assisted Dev</span>
          <span class="tag">GitHub Pages</span>
          <span class="tag">Canva Design</span>
        </div>
      </div>
      <div class="about-card">
        <h3>How I work</h3>
        <p>Instead of pitching with a proposal PDF, I build a working demo site first — real design, real code, deployed and live — then show it to the business directly. You see exactly what you're paying for before you commit.</p>
        <div class="tag-row">
          <span class="tag">Tamil</span>
          <span class="tag">English</span>
          <span class="tag">Hindi</span>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="services">
  <div class="wrap">
    <div class="section-head">
      <div class="eyebrow">Services & Pricing</div>
      <h2>Three ways to get online.</h2>
      <p>Straightforward tiers, no hidden costs — pick what matches where your business is right now.</p>
    </div>
    <div class="services-grid">
      <div class="service-card">
        <h3>Starter Page</h3>
        <div class="price">₹2,000</div>
        <p style="color:var(--ink-dim);font-size:0.88rem;">A single, polished landing page to get your business online fast.</p>
        <ul>
          <li>1-page responsive site</li>
          <li>WhatsApp contact button</li>
          <li>Basic SEO setup</li>
          <li>Delivered in 2–3 days</li>
        </ul>
      </div>
      <div class="service-card featured">
        <span class="badge">MOST BOOKED</span>
        <h3>Business Site</h3>
        <div class="price">₹5,000</div>
        <p style="color:var(--ink-dim);font-size:0.88rem;">A complete multi-section site built around how your business actually sells.</p>
        <ul>
          <li>Multi-section custom design</li>
          <li>Photo gallery / service menu</li>
          <li>Google Maps + contact form</li>
          <li>Mobile-first, fast loading</li>
        </ul>
      </div>
      <div class="service-card">
        <h3>Full Digital Setup</h3>
        <div class="price">₹10,000</div>
        <p style="color:var(--ink-dim);font-size:0.88rem;">Website plus the brand assets and content to launch properly.</p>
        <ul>
          <li>Everything in Business Site</li>
          <li>Logo + brand assets (Canva)</li>
          <li>Launch reels / video edit</li>
          <li>1 month of support</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section id="work">
  <div class="wrap">
    <div class="section-head">
      <div class="eyebrow">Recent Work</div>
      <h2>Demos built to prove it works.</h2>
      <p>Every project below started as a spec demo, built first and pitched second.</p>
    </div>
    <div class="work-grid">
      <div class="work-card">
        <div class="work-thumb">Hammer Fitness</div>
        <div class="work-info">
          <h3>Hammer Fitness</h3>
          <p>Dark athletic red/black theme gym landing page.</p>
        </div>
      </div>
      <div class="work-card">
        <div class="work-thumb">DDC Polur</div>
        <div class="work-info">
          <h3>DDC Polur</h3>
          <p>Glassmorphism site with 3D flip cards & bilingual content.</p>
        </div>
      </div>
      <div class="work-card">
        <div class="work-thumb">Ketone Gym</div>
        <div class="work-info">
          <h3>Ketone Fitness Gym</h3>
          <p>Live client demo, deployed on GitHub Pages.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="contact">
  <div class="wrap">
    <div class="contact-card">
      <h2>Want a demo built for your business?</h2>
      <p>Message me directly — I'll usually reply the same day, and if you want, I can build a free demo of your site before you decide anything.</p>
      <div class="contact-links">
        <a class="primary" href="https://wa.me/918248128329?text=Hi%2C%20I%27m%20interested%20in%20your%20work%20and%20would%20like%20to%20work%20with%20you." target="_blank">WhatsApp</a>
        <a href="mailto:srikumarm8248@gmail.com?subject=Interested%20in%20working%20with%20you&body=Hi%20Sri%20Kumar%2C%0A%0AI%27m%20interested%20in%20your%20work%20and%20would%20like%20to%20work%20with%20you.%0A%0A">Email</a>
        <a href="https://github.com/srikumarm8248-droid" target="_blank">GitHub</a>
        <a href="https://linkedin.com/in/srikumarm161" target="_blank">LinkedIn</a>
        <a href="https://fiverr.com/srikumarm161" target="_blank">Fiverr</a>
      </div>
    </div>
  </div>
</section>

<footer>
  <div class="wrap">© 2026 JOJO Digital — Sri Kumar M, Hosur, Tamil Nadu.</div>
</footer>

<script>
  const lines = [
    { t: "prompt", text: "$ jojo build --client \"local-business\"" },
    { t: "plain", text: "→ analyzing business type..." },
    { t: "plain", text: "→ generating layout + copy..." },
    { t: "plain", text: "→ deploying to github pages..." },
    { t: "ok", text: "✓ demo live in 46s — ready to pitch" }
  ];
  const body = document.getElementById('termBody');
  let li = 0, ci = 0;

  function typeLine(){
    if(li >= lines.length){ return; }
    const current = lines[li];
    if(ci === 0){
      const div = document.createElement('div');
      div.className = 'line';
      div.innerHTML = '<span class="'+ (current.t==='prompt' ? 'prompt' : current.t==='ok' ? 'ok' : '') +'"></span>';
      body.appendChild(div);
    }
    const div = body.lastChild;
    const span = div.querySelector('span');
    ci++;
    span.textContent = current.text.slice(0, ci);
    if(ci <= current.text.length){
      setTimeout(typeLine, current.t==='prompt' ? 38 : 18);
    } else {
      ci = 0; li++;
      if(li < lines.length) setTimeout(typeLine, 260);
      else {
        const cursor = document.createElement('span');
        cursor.className = 'cursor';
        div.appendChild(cursor);
      }
    }
  }
  typeLine();
</script>

</body>
</html>
