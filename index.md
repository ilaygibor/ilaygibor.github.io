---
layout: default
title: Ilay Gibor — Engineering Portfolio
---

<!-- Paste this file as /index.md in your GitHub Pages repo. It works without any build tools. -->
<style>
  :root{
    --bg:#0b0c10; --card:#111217; --ink:#e6e6f0; --muted:#a9aec1; --brand:#6ea8fe; --accent:#8bffc3; --border:#1d2030;
  }
  html{scroll-behavior:smooth}
  body{margin:0;font:16px/1.6 system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji","Segoe UI Emoji";color:var(--ink);background:radial-gradient(1200px 600px at 20% -10%, #12203a 0%, transparent 60%), radial-gradient(1200px 600px at 100% 10%, #1a1d2b 0%, transparent 55%), var(--bg)}
  a{color:inherit;text-decoration:none}
  .wrap{max-width:1100px;margin:0 auto;padding:24px}
  .nav{position:sticky;top:0;backdrop-filter:saturate(160%) blur(10px);background:rgba(11,12,16,.6);border-bottom:1px solid var(--border);z-index:10}
  .nav .inner{display:flex;align-items:center;justify-content:space-between}
  .nav a.logo{font-weight:700;letter-spacing:.2px}
  .nav .links a{color:var(--muted);margin-left:18px}
  .nav .links a:hover{color:var(--ink)}
  .hero{padding:72px 24px 40px}
  .grid{display:grid;gap:18px}
  @media (min-width:900px){.grid-2{grid-template-columns:1.2fr 1fr}}
  h1{font-size:40px;line-height:1.15;margin:.2em 0}
  h2{font-size:28px;margin:0 0 8px}
  h3{font-size:18px;margin:0 0 8px}
  p{margin:0 0 10px;color:var(--muted)}
  .eyebrow{font-size:12px;letter-spacing:.18em;text-transform:uppercase;color:#9aa4bf}
  .badge{display:inline-block;border:1px solid var(--border);padding:4px 8px;border-radius:999px;font-size:12px;color:var(--muted);margin:8px 8px 0 0}
  .cta{display:inline-flex;align-items:center;gap:8px;background:linear-gradient(135deg,var(--brand),#6ee7ff);color:#081018;border:none;padding:10px 14px;border-radius:10px;font-weight:600}
  .cta.secondary{background:transparent;border:1px solid var(--border);color:var(--ink)}
  .card{background:linear-gradient(180deg, rgba(255,255,255,.02), rgba(255,255,255,.00));border:1px solid var(--border);border-radius:16px;padding:18px}
  .card:hover{box-shadow:0 10px 30px rgba(0,0,0,.25);transform:translateY(-2px);transition:.25s}
  .subtle{font-size:14px;color:var(--muted)}
  .quote{border-left:3px solid var(--border);padding:12px 16px;border-radius:8px;background:rgba(255,255,255,.03)}
  .pillrow{display:flex;flex-wrap:wrap;gap:8px}
  .footer{border-top:1px solid var(--border);padding:28px 24px;color:var(--muted)}
  .fade{opacity:0;transform:translateY(8px);animation:rise .7s .15s forwards}
  @keyframes rise{to{opacity:1;transform:none}}
  .btnrow{display:flex;flex-wrap:wrap;gap:10px;margin-top:14px}
  .cards{display:grid;gap:18px}
  @media(min-width:800px){.cards{grid-template-columns:1fr 1fr}}
  .title{background:linear-gradient(90deg,#dbe8ff 0%, #9fd7ff 60%, #b2ffe1 100%);-webkit-background-clip:text;background-clip:text;color:transparent}
  .kicker{display:inline-flex;align-items:center;gap:8px;border:1px solid var(--border);padding:6px 10px;border-radius:999px;color:var(--muted)}
  .kicker .dot{width:6px;height:6px;border-radius:50%;background:var(--accent)}
</style>

<!-- NAV -->
<div class="nav">
  <div class="wrap inner">
    <a class="logo" href="#top">Ilay Gibor</a>
    <div class="links">
      <a href="#research">Research</a>
      <a href="#engineering">Engineering</a>
      <a href="#contact">Contact</a>
      <a href="https://github.com/IlayGibor">GitHub</a>
    </div>
  </div>
</div>

<!-- HERO -->
<section id="top" class="wrap hero grid grid-2">
  <div>
    <div class="kicker fade">Engineering Portfolio <span class="dot"></span> Robotics • ML • Bioengineering</div>
    <h1 class="title fade">Ilay Gibor — Engineering Portfolio</h1>
    <p class="fade">Welcome! I’m Ilay, a high-school engineer working at the intersection of <strong>robotics</strong>, <strong>machine learning</strong>, and <strong>bioengineering</strong>.<br>This site collects my research and engineering projects with links to the complete code and documentation.</p>
    <div class="pillrow fade">
      <span class="badge">Robotics</span>
      <span class="badge">Machine Learning</span>
      <span class="badge">Bioengineering</span>
      <span class="badge">Open‑source</span>
    </div>
    <div class="btnrow fade">
      <a class="cta" href="#research">Explore Projects →</a>
      <a class="cta secondary" href="https://github.com/IlayGibor">GitHub Profile</a>
    </div>
  </div>
  <div class="fade">
    <div class="card">
      <h3 style="margin:0 0 6px">Focus Areas</h3>
      <p class="subtle">Collagen segmentation • Data robustness • Vision pipelines • PID tuning • Autonomous & Tele‑op • Full‑stack prototypes</p>
    </div>
    <div class="card" style="margin-top:12px">
      <h3 style="margin:0 0 6px">Reproducibility</h3>
      <p class="subtle">All repositories include detailed READMEs and <code>requirements.txt</code> files for reproducibility.</p>
    </div>
  </div>
</section>

<!-- RESEARCH -->
<section id="research" class="wrap" style="padding:20px 24px 8px">
  <div class="eyebrow">Research Projects</div>
  <h2>Applied ML & Bioengineering</h2>
  <p>Automated segmentation of collagen sub‑types in histopathology slides for permeability simulation; and comparative studies of model robustness under controlled data corruptions.</p>

  <div class="cards" style="margin-top:14px">
    <div class="card">
      <h3>Research Paper 1 — Collagen Segmentation</h3>
      <p class="subtle">Automated segmentation of collagen sub‑types in histopathology slides for permeability simulation.</p>
      <p><a class="cta secondary" href="./projects/research1/">View Code & Docs → GitHub Repository</a></p>
    </div>
    <div class="card">
      <h3>Research Paper 2 — ML Data Optimization / Robustness</h3>
      <p class="subtle">Compared machine‑learning models under different data corruptions to evaluate robustness and validation stability.</p>
      <p><a class="cta secondary" href="./projects/research2/">View Code & Docs → GitHub Repository</a></p>
    </div>
  </div>
</section>

<!-- ENGINEERING -->
<section id="engineering" class="wrap" style="padding:24px">
  <div class="eyebrow">Engineering & Applied Projects</div>
  <h2>Robotics, Systems, and Hackathons</h2>
  <p>Selected builds spanning autonomous control, computer vision, and full‑stack prototyping.</p>

  <div class="cards" style="margin-top:14px">
    <div class="card">
      <h3>FTC Robotics Codebase</h3>
      <p class="subtle">Full autonomous and tele‑op control system for our FTC robot, including vision pipelines and PID tuning.</p>
      <p><a class="cta secondary" href="./projects/robotics/">View Code → GitHub Repository</a></p>
    </div>
    <div class="card">
      <h3>KoHack App — Hackathon Project (2nd Place)</h3>
      <p class="subtle">24‑hour hackathon app built to [describe problem later]; front‑end + back‑end completed under tight deadline.</p>
      <p><a class="cta secondary" href="./projects/kohack/">View Code → GitHub Repository</a></p>
    </div>
  </div>

  <div class="quote" style="margin-top:16px">
    <em>“All repositories include detailed READMEs and requirements.txt files for reproducibility.”</em>
  </div>
</section>

<!-- CONTACT -->
<section id="contact" class="wrap" style="padding:12px 24px 64px">
  <div class="eyebrow">Contact</div>
  <h2>Let’s connect</h2>
  <p><strong>Email:</strong> your.email@example.com<br>
     <strong>GitHub:</strong> <a href="https://github.com/IlayGibor">github.com/IlayGibor</a></p>
  <div class="btnrow">
    <a class="cta" href="mailto:your.email@example.com">Email Me</a>
    <a class="cta secondary" href="https://github.com/IlayGibor">GitHub Profile</a>
  </div>
</section>

<!-- FOOTER -->
<footer class="footer">
  <div class="wrap">
    <div>© <span id="y"></span> Ilay Gibor. All rights reserved.</div>
    <div>Built with static HTML/CSS. Zero dependencies.</div>
  </div>
</footer>
<script>document.getElementById('y').textContent=new Date().getFullYear()</script>
