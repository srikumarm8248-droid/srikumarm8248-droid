<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SK STARK — Sri Kumar M</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@600;700;800&family=Plus+Jakarta+Sans:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --bg: #070d17;
    --panel: #10203a;
    --panel-edge: #1E3A5F;
    --gold: #D4AF37;
    --gold-bright: #F4D97A;
    --ink: #E8EDF4;
    --muted: #64789a;
    --line: rgba(212,175,55,0.18);
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    background:var(--bg);
    color:var(--ink);
    font-family:'Plus Jakarta Sans', sans-serif;
    overflow-x:hidden;
    position:relative;
  }
  ::selection{background:var(--gold);color:var(--bg);}

  /* ambient grid texture */
  body::before{
    content:'';
    position:fixed; inset:0;
    background-image:
      linear-gradient(var(--line) 1px, transparent 1px),
      linear-gradient(90deg, var(--line) 1px, transparent 1px);
    background-size:64px 64px;
    opacity:0.35;
    pointer-events:none;
    z-index:1;
    mask-image:radial-gradient(ellipse 80% 60% at 50% 20%, black 40%, transparent 90%);
  }

  h1,h2,h3{font-family:'Syne', sans-serif;}
  .mono{font-family:'JetBrains Mono', monospace;}

  /* ---------- HUD chrome ---------- */
  .corner{
    position:fixed; width:26px; height:26px; z-index:50;
    border-color:var(--gold); opacity:0.65; pointer-events:none;
  }
  .corner.tl{top:18px; left:18px; border-top:2px solid; border-left:2px solid;}
  .corner.tr{top:18px; right:18px; border-top:2px solid; border-right:2px solid;}
  .corner.bl{bottom:18px; left:18px; border-bottom:2px solid; border-left:2px solid;}
  .corner.br{bottom:18px; right:18px; border-bottom:2px solid; border-right:2px solid;}

  .hud-label{
    position:fixed; z-index:50; font-family:'JetBrains Mono', monospace;
    font-size:11px; letter-spacing:0.15em; color:var(--muted); pointer-events:none;
  }
  .hud-top{top:22px; left:56px;}
  .hud-top-right{top:22px; right:56px; text-align:right;}
  #clock{color:var(--gold);}

  .scanline{
    position:fixed; left:0; right:0; height:2px; z-index:40;
    background:linear-gradient(90deg, transparent, var(--gold-bright), transparent);
    opacity:0.5; pointer-events:none;
    animation:sweep 7s linear infinite;
  }
  @keyframes sweep{
    0%{ top:-2px; opacity:0;}
    5%{opacity:0.6;}
    95%{opacity:0.6;}
    100%{ top:100vh; opacity:0;}
  }

  /* progress rail */
  #rail{
    position:fixed; right:28px; top:50%; transform:translateY(-50%);
    z-index:60; display:flex; flex-direction:column; gap:18px;
  }
  #rail button{
    width:9px; height:9px; border-radius:50%;
    background:transparent; border:1.5px solid var(--muted);
    cursor:pointer; padding:0; transition:all .3s ease;
  }
  #rail button.active{background:var(--gold); border-color:var(--gold); box-shadow:0 0 10px var(--gold);}

  /* ---------- HERO ---------- */
  #hero{
    position:relative; height:100vh; display:flex; align-items:center; justify-content:center;
    z-index:5;
  }
  #core-canvas{position:absolute; inset:0; z-index:1;}
  .hero-inner{position:relative; z-index:3; text-align:center; padding:0 24px;}
  .eyebrow{
    font-family:'JetBrains Mono', monospace; font-size:12px; letter-spacing:0.35em;
    color:var(--gold); text-transform:uppercase; margin-bottom:18px; opacity:0;
    animation:fadeUp .9s ease forwards .3s;
  }
  .hero-inner h1{
    font-size:clamp(3rem, 9vw, 7.5rem); font-weight:800; letter-spacing:-0.02em;
    line-height:0.95; color:var(--ink); opacity:0;
    animation:fadeUp 1s ease forwards .5s;
  }
  .hero-inner h1 span{color:var(--gold);}
  .hero-sub{
    margin-top:22px; font-size:clamp(1rem,2vw,1.25rem); color:var(--muted);
    max-width:560px; margin-left:auto; margin-right:auto; opacity:0;
    animation:fadeUp 1s ease forwards .75s;
  }
  .hero-tags{
    margin-top:30px; display:flex; gap:10px; justify-content:center; flex-wrap:wrap;
    opacity:0; animation:fadeUp 1s ease forwards 1s;
  }
  .tag{
    font-family:'JetBrains Mono', monospace; font-size:12px; padding:7px 14px;
    border:1px solid var(--line); border-radius:100px; color:var(--gold-bright);
    background:rgba(212,175,55,0.05);
  }
  @keyframes fadeUp{ from{opacity:0; transform:translateY(18px);} to{opacity:1; transform:translateY(0);} }

  .scroll-cue{
    position:absolute; bottom:38px; left:50%; transform:translateX(-50%);
    font-family:'JetBrains Mono', monospace; font-size:10px; letter-spacing:0.3em;
    color:var(--muted); z-index:3; display:flex; flex-direction:column; align-items:center; gap:8px;
  }
  .scroll-cue::after{
    content:''; width:1px; height:34px; background:linear-gradient(var(--gold), transparent);
    animation:pulse 1.8s ease infinite;
  }
  @keyframes pulse{ 0%,100%{opacity:0.2;} 50%{opacity:1;} }

  /* ---------- Sections ---------- */
  section{position:relative; z-index:5; padding:130px 24px; max-width:1080px; margin:0 auto;}
  .section-head{margin-bottom:56px;}
  .section-head .idx{font-family:'JetBrains Mono', monospace; font-size:12px; color:var(--gold); letter-spacing:0.25em;}
  .section-head h2{font-size:clamp(1.9rem,4vw,3rem); margin-top:10px; font-weight:700;}
  .reveal{opacity:0; transform:translateY(28px); transition:opacity .8s ease, transform .8s ease;}
  .reveal.in{opacity:1; transform:translateY(0);}

  /* about */
  #about .grid{display:grid; grid-template-columns:1.3fr 1fr; gap:48px;}
  #about p{color:#c3cee0; line-height:1.75; font-size:1.05rem; margin-bottom:16px;}
  .stat-panel{
    border:1px solid var(--line); background:rgba(30,58,95,0.25); backdrop-filter:blur(6px);
    border-radius:14px; padding:22px;
  }
  .stat-row{display:flex; justify-content:space-between; padding:11px 0; border-bottom:1px dashed var(--line); font-size:0.92rem;}
  .stat-row:last-child{border-bottom:none;}
  .stat-row .k{color:var(--muted); font-family:'JetBrains Mono', monospace; font-size:0.78rem; letter-spacing:0.05em;}
  .stat-row .v{color:var(--ink); font-weight:600;}

  /* now / focus */
  .focus-grid{display:grid; grid-template-columns:repeat(auto-fit, minmax(230px,1fr)); gap:18px;}
  .focus-card{
    border:1px solid var(--line); border-radius:14px; padding:24px;
    background:linear-gradient(160deg, rgba(30,58,95,0.35), rgba(7,13,23,0.4));
    position:relative; overflow:hidden; transition:transform .35s ease, border-color .35s ease;
  }
  .focus-card:hover{transform:translateY(-6px); border-color:var(--gold);}
  .focus-card .tag-mini{font-family:'JetBrains Mono', monospace; font-size:10px; color:var(--gold); letter-spacing:0.2em;}
  .focus-card h3{font-size:1.05rem; margin:10px 0 8px; font-weight:700;}
  .focus-card p{font-size:0.88rem; color:var(--muted); line-height:1.55;}

  /* projects */
  .proj{
    display:grid; grid-template-columns:60px 1fr; gap:22px; padding:26px 0;
    border-bottom:1px solid var(--line); align-items:start;
  }
  .proj:last-child{border-bottom:none;}
  .proj .sysno{font-family:'JetBrains Mono', monospace; color:var(--gold); font-size:0.85rem; padding-top:4px;}
  .proj h3{font-size:1.35rem; margin-bottom:8px;}
  .proj p{color:#c3cee0; font-size:0.95rem; line-height:1.6; margin-bottom:12px; max-width:640px;}
  .stack{display:flex; flex-wrap:wrap; gap:8px;}
  .stack span{
    font-family:'JetBrains Mono', monospace; font-size:11px; color:var(--muted);
    border:1px solid var(--line); padding:4px 10px; border-radius:6px;
  }

  /* competencies */
  .bar-item{margin-bottom:20px;}
  .bar-label{display:flex; justify-content:space-between; font-size:0.88rem; margin-bottom:8px;}
  .bar-label .name{font-weight:600;}
  .bar-label .val{font-family:'JetBrains Mono', monospace; color:var(--gold);}
  .bar-track{height:6px; border-radius:6px; background:rgba(255,255,255,0.06); overflow:hidden;}
  .bar-fill{height:100%; border-radius:6px; width:0%; background:linear-gradient(90deg, var(--panel-edge), var(--gold)); transition:width 1.4s cubic-bezier(.16,1,.3,1);}

  /* contact */
  #contact{text-align:center;}
  #contact h2{font-size:clamp(2.2rem,5vw,3.6rem);}
  #contact p.lead{color:var(--muted); max-width:480px; margin:18px auto 40px;}
  .contact-row{display:flex; gap:14px; justify-content:center; flex-wrap:wrap;}
  .btn{
    font-family:'JetBrains Mono', monospace; font-size:0.85rem; letter-spacing:0.05em;
    padding:13px 22px; border-radius:10px; text-decoration:none; display:inline-flex; align-items:center; gap:8px;
    border:1px solid var(--line); color:var(--ink); transition:all .3s ease;
  }
  .btn:hover{border-color:var(--gold); color:var(--gold-bright); box-shadow:0 0 22px rgba(212,175,55,0.18); transform:translateY(-2px);}
  .btn.primary{background:var(--gold); color:var(--bg); border-color:var(--gold); font-weight:700;}
  .btn.primary:hover{color:var(--bg); box-shadow:0 0 26px rgba(212,175,55,0.45);}

  footer{
    text-align:center; padding:40px 24px 60px; font-family:'JetBrains Mono', monospace;
    font-size:11px; color:var(--muted); letter-spacing:0.1em; position:relative; z-index:5;
  }

  @media (max-width:820px){
    #about .grid{grid-template-columns:1fr;}
    .proj{grid-template-columns:1fr;}
    #rail{display:none;}
  }
  @media (prefers-reduced-motion: reduce){
    *{animation-duration:0.01ms !important; animation-iteration-count:1 !important; transition-duration:0.01ms !important;}
  }
</style>
</head>
<body>

<div class="corner tl"></div>
<div class="corner tr"></div>
<div class="corner bl"></div>
<div class="corner br"></div>
<div class="hud-label hud-top">SYSTEM // SK-STARK<br>STATUS: <span id="clock">ONLINE</span></div>
<div class="hud-label hud-top-right">HOSUR, TAMIL NADU<br><span class="mono" id="localtime">--:--:--</span></div>
<div class="scanline"></div>

<nav id="rail">
  <button data-target="hero" class="active" aria-label="Hero"></button>
  <button data-target="about" aria-label="About"></button>
  <button data-target="focus" aria-label="Now"></button>
  <button data-target="projects" aria-label="Projects"></button>
  <button data-target="skills" aria-label="Competencies"></button>
  <button data-target="contact" aria-label="Contact"></button>
</nav>

<!-- HERO -->
<section id="hero" style="padding:0;">
  <canvas id="core-canvas"></canvas>
  <div class="hero-inner">
    <div class="eyebrow">// initializing profile</div>
    <h1>SK <span>STARK</span></h1>
    <p class="hero-sub">Sri Kumar M — agentic AI builder, freelance web developer, and NSS Programme Officer running a one-person control system out of Hosur, Tamil Nadu.</p>
    <div class="hero-tags">
      <span class="tag">AI &amp; Automation</span>
      <span class="tag">Web &amp; App Builder</span>
      <span class="tag">BCA · Periyar University</span>
      <span class="tag">NSS Programme Officer</span>
    </div>
  </div>
  <div class="scroll-cue">SCROLL</div>
</section>

<!-- ABOUT -->
<section id="about">
  <div class="section-head reveal">
    <div class="idx">01 // ABOUT</div>
    <h2>Building my own control room</h2>
  </div>
  <div class="grid">
    <div class="reveal">
      <p>I'm a BCA 2nd year student at M.G.R. College, Hosur, affiliated with Periyar University, Salem — and I run my freelance brand alongside it, taking on web design, AI development, Canva work, and automation for local businesses.</p>
      <p>My flagship build right now is <strong style="color:var(--gold-bright)">STARK CONTROL</strong> — a mobile-controlled laptop management system made of eight standalone apps (Connect, Remote, Files, Terminal, Cam, Status, NFC, Vault), built on Flask, React Native Expo, and ngrok tunneling.</p>
      <p>Outside code, I'm the NSS Programme Officer for my college — designing the systems that find and score student volunteers — and I keep a quieter creative practice in pencil drawing and pencil carving.</p>
    </div>
    <div class="reveal stat-panel">
      <div class="stat-row"><span class="k">LOCATION</span><span class="v">Hosur, Tamil Nadu</span></div>
      <div class="stat-row"><span class="k">EDUCATION</span><span class="v">BCA — 2nd Year</span></div>
      <div class="stat-row"><span class="k">INSTITUTION</span><span class="v">M.G.R. College</span></div>
      <div class="stat-row"><span class="k">AFFILIATION</span><span class="v">Periyar University</span></div>
      <div class="stat-row"><span class="k">NSS ROLE</span><span class="v">Programme Officer</span></div>
      <div class="stat-row"><span class="k">LANGUAGES</span><span class="v">Tamil · English · Hindi</span></div>
      <div class="stat-row"><span class="k">CERT (HP LIFE)</span><span class="v">AI · Cybersecurity · Data Science</span></div>
    </div>
  </div>
</section>

<!-- FOCUS -->
<section id="focus">
  <div class="section-head reveal">
    <div class="idx">02 // CURRENT FOCUS</div>
    <h2>What's running right now</h2>
  </div>
  <div class="focus-grid">
    <div class="focus-card reveal">
      <div class="tag-mini">BUILD</div>
      <h3>STARK CONTROL</h3>
      <p>8-app mobile control suite for managing a laptop remotely — the main system in active development.</p>
    </div>
    <div class="focus-card reveal">
      <div class="tag-mini">FREELANCE</div>
      <h3>Fiverr gigs</h3>
      <p>Landing page &amp; vibe-coded website gig, plus Canva design and resume design gigs coming online.</p>
    </div>
    <div class="focus-card reveal">
      <div class="tag-mini">CAMPUS</div>
      <h3>NSS digital pipeline</h3>
      <p>Volunteer assessment form, scoring framework, and a digital enrollment system with QR payments.</p>
    </div>
    <div class="focus-card reveal">
      <div class="tag-mini">PERSONAL</div>
      <h3>JoJo — baby AI</h3>
      <p>A local Ollama + Llama3 assistant that starts from zero knowledge and grows with use over time.</p>
    </div>
  </div>
</section>

<!-- PROJECTS -->
<section id="projects">
  <div class="section-head reveal">
    <div class="idx">03 // PROJECTS</div>
    <h2>Shipped &amp; in progress</h2>
  </div>

  <div class="proj reveal">
    <div class="sysno">01</div>
    <div>
      <h3>STARK CONTROL</h3>
      <p>Control your laptop from your phone — connection, remote desktop, file access, terminal, camera, live status, NFC triggers, and a secure vault, as eight independent apps talking to one Flask backend.</p>
      <div class="stack"><span>Python · Flask</span><span>React Native Expo</span><span>ngrok</span></div>
    </div>
  </div>

  <div class="proj reveal">
    <div class="sysno">02</div>
    <div>
      <h3>Client demo sites</h3>
      <p>Ketone Fitness Gym and Hammer Fitness (live on GitHub Pages), plus DDC Polur, a premium diagnostic-centre concept site with Tamil-language content and Schema.org SEO — all single-file builds in the Navy + Gold system.</p>
      <div class="stack"><span>HTML/CSS glassmorphism</span><span>Syne + Plus Jakarta Sans</span><span>Schema.org</span></div>
    </div>
  </div>

  <div class="proj reveal">
    <div class="sysno">03</div>
    <div>
      <h3>NSS Digital ID System</h3>
      <p>Zero-cost volunteer enrollment platform — assessment form, CSV export, and QR-based payment tracking for the campus NSS unit.</p>
      <div class="stack"><span>GitHub Pages</span><span>Google Apps Script</span></div>
    </div>
  </div>

  <div class="proj reveal">
    <div class="sysno">04</div>
    <div>
      <h3>JoJo AI</h3>
      <p>A personal AI that begins with no knowledge and learns as it's used — my long-running experiment in growing a model instead of shipping one fully formed.</p>
      <div class="stack"><span>Ollama</span><span>Llama 3</span></div>
    </div>
  </div>
</section>

<!-- SKILLS -->
<section id="skills">
  <div class="section-head reveal">
    <div class="idx">04 // COMPETENCIES</div>
    <h2>Where the hours go</h2>
  </div>
  <div class="reveal" id="bars">
    <div class="bar-item">
      <div class="bar-label"><span class="name">AI &amp; Automation</span><span class="val">88%</span></div>
      <div class="bar-track"><div class="bar-fill" data-w="88"></div></div>
    </div>
    <div class="bar-item">
      <div class="bar-label"><span class="name">Web &amp; App Development</span><span class="val">90%</span></div>
      <div class="bar-track"><div class="bar-fill" data-w="90"></div></div>
    </div>
    <div class="bar-item">
      <div class="bar-label"><span class="name">Design (Canva / Figma / UI)</span><span class="val">80%</span></div>
      <div class="bar-track"><div class="bar-fill" data-w="80"></div></div>
    </div>
    <div class="bar-item">
      <div class="bar-label"><span class="name">Leadership &amp; NSS Ops</span><span class="val">85%</span></div>
      <div class="bar-track"><div class="bar-fill" data-w="85"></div></div>
    </div>
    <div class="bar-item">
      <div class="bar-label"><span class="name">Freelance &amp; Client Sales</span><span class="val">75%</span></div>
      <div class="bar-track"><div class="bar-fill" data-w="75"></div></div>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <div class="reveal">
    <div class="idx" style="justify-content:center; display:flex;">05 // CONTACT</div>
    <h2>Let's build something</h2>
    <p class="lead">Open to freelance web &amp; AI projects, collaborations, and anything that needs a control system built around it.</p>
    <div class="contact-row">
      <a class="btn primary" href="https://wa.me/918248128329?text=Hi%20SK%20Stark%2C%20I%27m%20interested%20in%20working%20with%20you" target="_blank">WhatsApp</a>
      <a class="btn" href="mailto:srikumarm8248@gmail.com">Email</a>
      <a class="btn" href="https://fiverr.com/srikumarm161" target="_blank">Fiverr</a>
      <a class="btn" href="https://linkedin.com/in/srikumarm161" target="_blank">LinkedIn</a>
      <a class="btn" href="https://github.com/srikumarm8248-droid" target="_blank">GitHub</a>
    </div>
  </div>
</section>

<footer>SK STARK © 2026 — BUILT FROM HOSUR, TAMIL NADU // ALL SYSTEMS NOMINAL</footer>

<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
<script>
  /* ---------- Live clock ---------- */
  function tick(){
    const d = new Date();
    document.getElementById('localtime').textContent = d.toLocaleTimeString('en-GB', {hour12:false});
  }
  tick(); setInterval(tick, 1000);

  /* ---------- Scroll reveal ---------- */
  const revealEls = document.querySelectorAll('.reveal');
  const io = new IntersectionObserver((entries)=>{
    entries.forEach(e=>{
      if(e.isIntersecting){
        e.target.classList.add('in');
        if(e.target.id === 'bars'){
          e.target.querySelectorAll('.bar-fill').forEach(b=>{
            b.style.width = b.dataset.w + '%';
          });
        }
      }
    });
  }, {threshold:0.2});
  revealEls.forEach(el=>io.observe(el));

  /* ---------- Rail nav sync ---------- */
  const sections = ['hero','about','focus','projects','skills','contact'];
  const railBtns = document.querySelectorAll('#rail button');
  railBtns.forEach(btn=>{
    btn.addEventListener('click', ()=>{
      document.getElementById(btn.dataset.target).scrollIntoView({behavior:'smooth'});
    });
  });
  const secObserver = new IntersectionObserver((entries)=>{
    entries.forEach(e=>{
      if(e.isIntersecting){
        railBtns.forEach(b=>b.classList.toggle('active', b.dataset.target === e.target.id));
      }
    });
  }, {threshold:0.5});
  sections.forEach(id=>{
    const el = document.getElementById(id);
    if(el) secObserver.observe(el);
  });

  /* ---------- Three.js reactor core ---------- */
  (function(){
    const canvas = document.getElementById('core-canvas');
    const renderer = new THREE.WebGLRenderer({canvas, alpha:true, antialias:true});
    renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2));
    renderer.setSize(window.innerWidth, window.innerHeight);

    const scene = new THREE.Scene();
    const camera = new THREE.PerspectiveCamera(55, window.innerWidth/window.innerHeight, 0.1, 100);
    camera.position.set(0,0,7.5);

    const group = new THREE.Group();
    scene.add(group);

    // outer wireframe icosahedron
    const outerGeo = new THREE.IcosahedronGeometry(2.4, 1);
    const outerMat = new THREE.MeshBasicMaterial({color:0xD4AF37, wireframe:true, transparent:true, opacity:0.55});
    const outer = new THREE.Mesh(outerGeo, outerMat);
    group.add(outer);

    // inner glow core
    const innerGeo = new THREE.IcosahedronGeometry(1.1, 2);
    const innerMat = new THREE.MeshBasicMaterial({color:0xF4D97A, wireframe:true, transparent:true, opacity:0.85});
    const inner = new THREE.Mesh(innerGeo, innerMat);
    group.add(inner);

    // orbit rings
    const ringGeo1 = new THREE.TorusGeometry(3.1, 0.006, 8, 100);
    const ringMat = new THREE.MeshBasicMaterial({color:0x1E3A5F, transparent:true, opacity:0.9});
    const ring1 = new THREE.Mesh(ringGeo1, ringMat);
    ring1.rotation.x = Math.PI/2.4;
    group.add(ring1);
    const ring2 = new THREE.Mesh(ringGeo1.clone(), ringMat.clone());
    ring2.rotation.x = Math.PI/1.6;
    ring2.rotation.y = Math.PI/3;
    ring2.material.color.set(0xD4AF37);
    ring2.material.opacity = 0.35;
    group.add(ring2);

    // particle field
    const particleCount = 260;
    const positions = new Float32Array(particleCount*3);
    for(let i=0;i<particleCount;i++){
      const r = 4 + Math.random()*4;
      const theta = Math.random()*Math.PI*2;
      const phi = Math.acos((Math.random()*2)-1);
      positions[i*3] = r*Math.sin(phi)*Math.cos(theta);
      positions[i*3+1] = r*Math.sin(phi)*Math.sin(theta);
      positions[i*3+2] = r*Math.cos(phi);
    }
    const pGeo = new THREE.BufferGeometry();
    pGeo.setAttribute('position', new THREE.BufferAttribute(positions,3));
    const pMat = new THREE.PointsMaterial({color:0xD4AF37, size:0.03, transparent:true, opacity:0.5});
    const particles = new THREE.Points(pGeo, pMat);
    scene.add(particles);

    let targetX = 0, targetY = 0;
    window.addEventListener('mousemove', (e)=>{
      targetX = (e.clientX/window.innerWidth - 0.5) * 0.6;
      targetY = (e.clientY/window.innerHeight - 0.5) * 0.6;
    });

    function animate(){
      requestAnimationFrame(animate);
      outer.rotation.y += 0.0022;
      outer.rotation.x += 0.0009;
      inner.rotation.y -= 0.0035;
      inner.rotation.x += 0.0016;
      ring1.rotation.z += 0.0016;
      ring2.rotation.z -= 0.001;
      particles.rotation.y += 0.0003;

      group.rotation.y += (targetX - group.rotation.y) * 0.02;
      group.rotation.x += (-targetY - group.rotation.x) * 0.02;

      renderer.render(scene, camera);
    }
    animate();

    // fade core out on scroll past hero
    window.addEventListener('scroll', ()=>{
      const vh = window.innerHeight;
      const fade = Math.max(0, 1 - (window.scrollY / (vh*0.9)));
      canvas.style.opacity = fade;
    });

    window.addEventListener('resize', ()=>{
      camera.aspect = window.innerWidth/window.innerHeight;
      camera.updateProjectionMatrix();
      renderer.setSize(window.innerWidth, window.innerHeight);
    });
  })();
</script>
</body>
</html>
