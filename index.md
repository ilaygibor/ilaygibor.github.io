---
layout: default
title: Ilay Gibor — Engineering Portfolio
---

<!-- One-file, no-build landing page. Paste into /index.md on GitHub Pages. -->
<style>
  :root{
    --bg:#0a0b10; --surface:#10121a; --card:#121523; --ink:#e9ecf4; --muted:#aab2cc; --brand:#6aa9ff; --brand2:#9fffe2; --border:#1d2234; --glow:#7ab8ff66;
  }
  html{scroll-behavior:smooth}
  body{margin:0;font:16px/1.6 Inter, ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial; color:var(--ink); background:radial-gradient(1200px 600px at 10% -10%, #122043 0%, transparent 60%), radial-gradient(1200px 600px at 100% 0%, #1a1e2e 0%, transparent 60%), var(--bg)}
  a{color:inherit;text-decoration:none}
  .wrap{max-width:1150px;margin:0 auto;padding:24px}
  .nav{position:sticky;top:0;backdrop-filter:saturate(160%) blur(10px);background:rgba(10,11,16,.6);border-bottom:1px solid var(--border);z-index:50}
  .nav .inner{display:flex;align-items:center;justify-content:space-between}
  .logo{display:flex;align-items:center;gap:10px;font-weight:800;letter-spacing:.2px}
  .logoDot{width:8px;height:8px;border-radius:50%;background:linear-gradient(135deg,var(--brand),var(--brand2));box-shadow:0 0 18px var(--glow)}
  .tabs a{color:var(--muted);margin-left:18px;font-weight:500}
  .tabs a:hover{color:var(--ink)}
  .hero{padding:84px 24px 56px; position:relative; overflow:hidden}
  .ribbon{position:absolute; inset: -20% -20% auto auto; height:280px; width:820px; transform:rotate(15deg); background:linear-gradient(90deg, transparent, #ffffff05, transparent); filter:blur(4px)}
  .h-title{font-size:56px; line-height:1.05; margin:.2em 0 .15em; letter-spacing:.3px}
  .h-sub{font-size:18px; color:var(--muted); max-width:720px}
  .btnrow{display:flex;flex-wrap:wrap;gap:12px;margin-top:20px}
  .btn{display:inline-flex;align-items:center;gap:10px;padding:12px 16px;border-radius:12px;font-weight:650;border:1px solid var(--border);background:linear-gradient(180deg, rgba(255,255,255,.03), rgba(255,255,255,.00));box-shadow:inset 0 1px 0 rgba(255,255,255,.06)}
  .btn.primary{background:linear-gradient(135deg,var(--brand),#6ee7ff); color:#07101a;border:none}
  .btn:hover{transform:translateY(-1px); box-shadow:0 14px 34px rgba(0,0,0,.25), 0 0 0 2px #ffffff08}
  .section{padding:48px 24px}
  .section h2{font-size:30px;margin:0 0 10px}
  .section p.lead{color:var(--muted);max-width:820px}
  .grid{display:grid;gap:18px}
  .grid-2{grid-template-columns:1fr}
  @media(min-width:860px){.grid-2{grid-template-columns:1fr 1fr}}
  .cards{display:grid;gap:18px}
  .cards-3x2{grid-template-columns:1fr;}
  @media(min-width:760px){.cards-3x2{grid-template-columns:1fr 1fr}}
  @media(min-width:1040px){.cards-3x2{grid-template-columns:1fr 1fr 1fr}}
  .cards-4x3{grid-template-columns:1fr 1fr}
  @media(min-width:900px){.cards-4x3{grid-template-columns:repeat(4,1fr)}}
  .card{background:linear-gradient(180deg, rgba(255,255,255,.02), rgba(255,255,255,.00));border:1px solid var(--border);border-radius:18px;padding:16px; position:relative; overflow:hidden; transition:.25s}
  .card:hover{transform:translateY(-3px); box-shadow:0 20px 50px rgba(0,0,0,.35)}
  .card::after{content:""; position:absolute; inset:-40%; background:radial-gradient(500px 200px at var(--mx,50%) var(--my,50%), #7aa8ff15, transparent 60%); transition:.15s}
  .thumb{aspect-ratio: 16/10; border-radius:12px; background:linear-gradient(135deg,#1c2740,#0e1324); border:1px dashed #2a3350; display:flex;align-items:center;justify-content:center; color:#94a3b8; font-weight:700}
  .thumb svg{opacity:.8}
  .c-title{font-weight:700;margin:10px 0 6px}
  .c-text{color:var(--muted); font-size:14px}
  .pill{display:inline-flex;align-items:center;gap:8px;border:1px solid var(--border);padding:6px 10px;border-radius:999px;color:var(--muted);font-size:12px}
  .footer{border-top:1px solid var(--border);padding:28px 24px;color:var(--muted)}
  .center{display:flex;align-items:center;justify-content:center}
  .hero-stack{margin-top:22px; display:flex; flex-direction:column; gap:12px}
</style>

<!-- NAV -->
<div class="nav">
  <div class="wrap inner">
    <a class="logo" href="#top"><span class="logoDot"></span> Ilay Gibor</a>
    <div class="tabs">
      <a href="#projects">Research</a>
      <a href="#projects">Robotics</a>
      <a href="#impact">Competitions</a>
      <a href="#impact">Recognition</a>
      <a href="#contact">Contact</a>
      <a href="https://github.com/IlayGibor">GitHub</a>
    </div>
  </div>
</div>

<!-- HERO -->
<section id="top" class="wrap hero">
  <div class="ribbon"></div>
  <h1 class="h-title">Ilay Gibor.</h1>
  <div class="h-sub">Welcome to my engineering portfolio where I showcase my work and skills.</div>

  <div class="hero-stack">
    <p class="h-sub">I’m a high‑school engineer focused on robotics, machine learning, and bioengineering. I build reproducible systems, lead technical teams, and ship projects end‑to‑end—from research ideas to working code and competition‑ready builds.</p>
    <div class="btnrow">
      <a class="btn primary" href="#projects">View my work</a>
      <a class="btn" href="#skills">Skills & expertise</a>
      <a class="btn" href="#impact">Impact & recognition</a>
    </div>
  </div>
</section>

<!-- PROJECTS -->
<section id="projects" class="section wrap">
  <h2>Projects</h2>
  <p class="lead">A selection of hands‑on builds and research implementations. Click any card to open its dedicated page.</p>

  <div class="cards cards-3x2" id="projCards">
    <!-- Six project placeholder cards -->
    <!-- Repeatable card pattern -->
    <a class="card" href="#" onmousemove="this.style.setProperty('--mx', event.offsetX+'px'); this.style.setProperty('--my', event.offsetY+'px');">
      <div class="thumb">Project 1 • Image</div>
      <div class="c-title">Project 1</div>
      <div class="c-text">Short one‑liner describing what the project does and why it matters.</div>
    </a>
    <a class="card" href="#">
      <div class="thumb">Project 2 • Image</div>
      <div class="c-title">Project 2</div>
      <div class="c-text">Short one‑liner describing what the project does and why it matters.</div>
    </a>
    <a class="card" href="#">
      <div class="thumb">Project 3 • Image</div>
      <div class="c-title">Project 3</div>
      <div class="c-text">Short one‑liner describing what the project does and why it matters.</div>
    </a>
    <a class="card" href="#">
      <div class="thumb">Project 4 • Image</div>
      <div class="c-title">Project 4</div>
      <div class="c-text">Short one‑liner describing what the project does and why it matters.</div>
    </a>
    <a class="card" href="#">
      <div class="thumb">Project 5 • Image</div>
      <div class="c-title">Project 5</div>
      <div class="c-text">Short one‑liner describing what the project does and why it matters.</div>
    </a>
    <a class="card" href="#">
      <div class="thumb">Project 6 • Image</div>
      <div class="c-title">Project 6</div>
      <div class="c-text">Short one‑liner describing what the project does and why it matters.</div>
    </a>
  </div>
</section>

<!-- SKILLS -->
<section id="skills" class="section wrap">
  <h2>Skills</h2>
  <p class="lead">Core tools and domains I use across robotics, ML, and systems work.</p>
  <div class="cards cards-4x3">
    <!-- 12 skill squares with icon placeholders -->
    
    <!-- Row 1 -->
    <div class="card center"><div>
      <div class="thumb" style="aspect-ratio:1/1; margin-bottom:10px">👾</div>
      <div class="c-title center" style="justify-content:center">Skill 1</div>
    </div></div>
    <div class="card center"><div>
      <div class="thumb" style="aspect-ratio:1/1; margin-bottom:10px">🧠</div>
      <div class="c-title center" style="justify-content:center">Skill 2</div>
    </div></div>
    <div class="card center"><div>
      <div class="thumb" style="aspect-ratio:1/1; margin-bottom:10px">⚙️</div>
      <div class="c-title center" style="justify-content:center">Skill 3</div>
    </div></div>
    <div class="card center"><div>
      <div class="thumb" style="aspect-ratio:1/1; margin-bottom:10px">📐</div>
      <div class="c-title center" style="justify-content:center">Skill 4</div>
    </div></div>

    <!-- Row 2 -->
    <div class="card center"><div>
      <div class="thumb" style="aspect-ratio:1/1; margin-bottom:10px">🛰️</div>
      <div class="c-title center" style="justify-content:center">Skill 5</div>
    </div></div>
    <div class="card center"><div>
      <div class="thumb" style="aspect-ratio:1/1; margin-bottom:10px">🤖</div>
      <div class="c-title center" style="justify-content:center">Skill 6</div>
    </div></div>
    <div class="card center"><div>
      <div class="thumb" style="aspect-ratio:1/1; margin-bottom:10px">🧪</div>
      <div class="c-title center" style="justify-content:center">Skill 7</div>
    </div></div>
    <div class="card center"><div>
      <div class="thumb" style="aspect-ratio:1/1; margin-bottom:10px">🖥️</div>
      <div class="c-title center" style="justify-content:center">Skill 8</div>
    </div></div>

    <!-- Row 3 -->
    <div class="card center"><div>
      <div class="thumb" style="aspect-ratio:1/1; margin-bottom:10px">🧩</div>
      <div class="c-title center" style="justify-content:center">Skill 9</div>
    </div></div>
    <div class="card center"><div>
      <div class="thumb" style="aspect-ratio:1/1; margin-bottom:10px">🕹️</div>
      <div class="c-title center" style="justify-content:center">Skill 10</div>
    </div></div>
    <div class="card center"><div>
      <div class="thumb" style="aspect-ratio:1/1; margin-bottom:10px">📊</div>
      <div class="c-title center" style="justify-content:center">Skill 11</div>
    </div></div>
    <div class="card center"><div>
      <div class="thumb" style="aspect-ratio:1/1; margin-bottom:10px">🔧</div>
      <div class="c-title center" style="justify-content:center">Skill 12</div>
    </div></div>
  </div>
</section>

<!-- IMPACT / RECOGNITION -->
<section id="impact" class="section wrap">
  <h2>Impact & Recognition</h2>
  <p class="lead">Press, awards, recommendations, and posts that highlight outcomes from my work.</p>
  <div class="cards cards-3x2">
    <!-- 6 visual placeholders (expand to 8 later) -->
    <a class="card" href="#">
      <div class="thumb">Recognition 1</div>
      <div class="c-title">Recognition 1</div>
      <div class="c-text">Link to recommendation letter, press, or post.</div>
    </a>
    <a class="card" href="#">
      <div class="thumb">Recognition 2</div>
      <div class="c-title">Recognition 2</div>
      <div class="c-text">Link to recommendation letter, press, or post.</div>
    </a>
    <a class="card" href="#">
      <div class="thumb">Recognition 3</div>
      <div class="c-title">Recognition 3</div>
      <div class="c-text">Link to recommendation letter, press, or post.</div>
    </a>
    <a class="card" href="#">
      <div class="thumb">Recognition 4</div>
      <div class="c-title">Recognition 4</div>
      <div class="c-text">Link to recommendation letter, press, or post.</div>
    </a>
    <a class="card" href="#">
      <div class="thumb">Recognition 5</div>
      <div class="c-title">Recognition 5</div>
      <div class="c-text">Link to recommendation letter, press, or post.</div>
    </a>
    <a class="card" href="#">
      <div class="thumb">Recognition 6</div>
      <div class="c-title">Recognition 6</div>
      <div class="c-text">Link to recommendation letter, press, or post.</div>
    </a>
  </div>
</section>

<!-- CONTACT -->
<section id="contact" class="section wrap">
  <h2>Let’s connect</h2>
  <p class="lead"><strong>Email:</strong> your.email@example.com<br>
  <strong>GitHub:</strong> <a href="https://github.com/IlayGibor">github.com/IlayGibor</a></p>
  <div class="btnrow">
    <a class="btn primary" href="mailto:your.email@example.com">Email Me</a>
    <a class="btn" href="https://github.com/IlayGibor">GitHub Profile</a>
  </div>
</section>

<!-- FOOTER -->
<footer class="footer">
  <div class="wrap">
    <div>© <span id="y"></span> Ilay Gibor. All rights reserved.</div>
    <div>Built with static HTML/CSS. Zero dependencies.</div>
  </div>
</footer>
<script>
  document.getElementById('y').textContent=new Date().getFullYear();
  // glow follows cursor on cards
  for(const card of document.querySelectorAll('.card')){
    card.addEventListener('mousemove', e=>{
      const rect = e.currentTarget.getBoundingClientRect();
      card.style.setProperty('--mx', (e.clientX - rect.left)+'px');
      card.style.setProperty('--my', (e.clientY - rect.top)+'px');
    });
  }
</script>
