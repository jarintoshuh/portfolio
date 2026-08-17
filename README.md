<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Javier Andrés Quintero Rojas — Companion Profile</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Archivo:wght@400;500;600;700;800;900&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --paper: #F1EAD9;
    --paper-card: #F7F2E6;
    --ink: #15130F;
    --ink-soft: #524B39;
    --ink-faint: #8C8168;
    --line: #C9BC9C;
    --accent: #D9531D;
    --accent-bg: rgba(217,83,29,0.10);
    --accent-ink: #F7F2E6;
    --display: 'Archivo', sans-serif;
    --mono: 'JetBrains Mono', monospace;
  }
  *{ box-sizing:border-box; margin:0; padding:0; }
  html{ scroll-behavior:smooth; }
  body{ background:var(--paper); color:var(--ink); font-family:var(--display); font-size:16px; line-height:1.5; }
  .wrap{ max-width: 980px; margin:0 auto; padding: 0 26px; }

  .corners{
    position:relative;
    background:
      linear-gradient(var(--ink), var(--ink)) top left / 13px 1.5px no-repeat,
      linear-gradient(var(--ink), var(--ink)) top left / 1.5px 13px no-repeat,
      linear-gradient(var(--ink), var(--ink)) top right / 13px 1.5px no-repeat,
      linear-gradient(var(--ink), var(--ink)) top right / 1.5px 13px no-repeat,
      linear-gradient(var(--ink), var(--ink)) bottom left / 13px 1.5px no-repeat,
      linear-gradient(var(--ink), var(--ink)) bottom left / 1.5px 13px no-repeat,
      linear-gradient(var(--ink), var(--ink)) bottom right / 13px 1.5px no-repeat,
      linear-gradient(var(--ink), var(--ink)) bottom right / 1.5px 13px no-repeat;
  }
  .corners--light{
    background:
      linear-gradient(var(--paper), var(--paper)) top left / 13px 1.5px no-repeat,
      linear-gradient(var(--paper), var(--paper)) top left / 1.5px 13px no-repeat,
      linear-gradient(var(--paper), var(--paper)) top right / 13px 1.5px no-repeat,
      linear-gradient(var(--paper), var(--paper)) top right / 1.5px 13px no-repeat,
      linear-gradient(var(--paper), var(--paper)) bottom left / 13px 1.5px no-repeat,
      linear-gradient(var(--paper), var(--paper)) bottom left / 1.5px 13px no-repeat,
      linear-gradient(var(--paper), var(--paper)) bottom right / 13px 1.5px no-repeat,
      linear-gradient(var(--paper), var(--paper)) bottom right / 1.5px 13px no-repeat;
  }

  .pill{
    display:inline-flex; align-items:center; font-family:var(--mono); font-size:11.5px;
    letter-spacing:.03em; border:1px solid currentColor; border-radius:999px; padding:4px 12px;
  }

  /* Top bar */
  .topbar{ display:flex; justify-content:space-between; align-items:center; padding: 22px 0; font-family:var(--mono); font-size:11px; letter-spacing:.08em; color:var(--ink-faint); text-transform:uppercase; }

  /* Hero black panel */
  .hero{ background:var(--ink); color:var(--paper-card); padding: 40px 34px 30px; margin-bottom: 40px; }
  .hero-top{ display:flex; justify-content:space-between; align-items:flex-start; margin-bottom: 60px; }
  .hero-top .pill{ color:var(--paper-card); }
  .hero-ref{ font-family:var(--mono); font-size:12px; color:#B8AE94; }
  .hero-name{ font-family:var(--display); font-weight:900; font-size:clamp(30px,5.4vw,50px); line-height:1.02; letter-spacing:-0.01em; }
  .hero-role{ font-family:var(--mono); font-size:13.5px; color:#C9BE9F; margin-top:14px; max-width:52ch; }
  .hero-bottom{ display:flex; justify-content:space-between; align-items:flex-end; flex-wrap:wrap; gap:10px; margin-top: 44px; padding-top:16px; border-top: 1px solid #3A362A; }
  .hero-bottom-label{ font-family:var(--mono); font-size:11px; letter-spacing:.06em; text-transform:uppercase; color:#9B917A; }

  /* Section shell */
  section.block{ padding: 8px 0 46px; }
  .rule-row{ display:flex; align-items:center; gap:10px; margin-bottom:24px; font-family:var(--mono); font-size:11.5px; letter-spacing:.08em; text-transform:uppercase; color:var(--ink-faint); }
  .rule-row .diamond{ color: var(--accent); }
  .rule-row::after{ content:""; flex:1; border-bottom: 1px dotted var(--line); }
  .block-title{ font-family:var(--display); font-weight:800; font-size: 24px; margin-bottom: 8px; }
  .block-lede{ color: var(--ink-soft); max-width: 62ch; margin-bottom: 22px; font-size:14.5px; }

  /* Snapshot strip */
  .snap-grid{ display:grid; grid-template-columns: repeat(auto-fit,minmax(160px,1fr)); gap: 14px; }
  .snap-card{ padding: 18px 18px; }
  .snap-num{ font-family:var(--display); font-weight:800; font-size: 28px; color: var(--accent); }
  .snap-label{ font-family:var(--mono); font-size: 10.5px; color: var(--ink-faint); text-transform:uppercase; letter-spacing:.04em; margin-top:4px; }

  /* Capability cards */
  .cap-grid{ display:grid; grid-template-columns: repeat(3, 1fr); gap: 14px; }
  @media (max-width:760px){ .cap-grid{ grid-template-columns: 1fr; } }
  .cap-card{ display:flex; flex-direction:column; }
  .cap-card.is-accent{ background: var(--accent); color: var(--accent-ink); }
  .cap-card.is-accent .cap-num, .cap-card.is-accent .cap-caption{ color: var(--accent-ink); opacity:.85; }
  .cap-top{ display:flex; justify-content:space-between; align-items:center; padding: 14px 16px 0; }
  .cap-num{ font-family:var(--mono); font-size:11px; color: var(--ink-faint); }
  .cap-icon{ padding: 18px 20px 8px; display:flex; justify-content:center; }
  .cap-icon svg{ width:64px; height:64px; }
  .cap-name{ font-family:var(--display); font-weight:700; font-size:17px; padding: 4px 18px 12px; }
  .cap-caption{ font-family:var(--mono); font-size:11.5px; color: var(--ink-soft); padding: 12px 16px 16px; border-top:1px solid var(--line); margin-top:auto; }
  .cap-card.is-accent .cap-caption{ border-top-color: rgba(247,242,230,0.35); }

  /* Experience */
  .job{ display:grid; grid-template-columns: 150px 1fr; gap: 18px; padding: 18px 0; border-bottom: 1px dotted var(--line); }
  .job:last-child{ border-bottom:none; }
  .job-when{ font-family:var(--mono); font-size:11.5px; color: var(--ink-faint); padding-top:3px; }
  .job-role{ font-family:var(--display); font-weight:700; font-size:16.5px; }
  .job-org{ color: var(--accent); font-weight:700; }
  .job p{ color: var(--ink-soft); font-size:14px; margin-top:6px; max-width:60ch; }

  .nda-line{ font-family:var(--mono); font-size:12px; color: var(--ink-faint); margin-top:18px; }

  /* Tools */
  .tool-groups{ display:grid; grid-template-columns: repeat(auto-fit,minmax(210px,1fr)); gap: 20px; }
  .tool-label{ font-family:var(--mono); font-size:10.5px; letter-spacing:.06em; text-transform:uppercase; color:var(--ink-faint); margin-bottom:8px; }
  .tool-pills{ display:flex; flex-wrap:wrap; gap:6px; }
  .tool-pill{ font-family:var(--mono); font-size:12px; background: var(--paper-card); border:1px solid var(--line); padding:4px 10px; }

  /* Credentials leader list */
  .leader{ display:flex; align-items:baseline; gap:10px; padding: 11px 0; border-bottom: 1px dotted var(--line); }
  .leader:last-child{ border-bottom:none; }
  .leader-num{ font-family:var(--mono); font-size:11.5px; color: var(--accent); flex-shrink:0; width:24px; }
  .leader-name{ font-family:var(--display); font-weight:600; font-size:14.5px; flex-shrink:0; }
  .leader-fill{ flex:1; border-bottom:1px dotted var(--line); transform: translateY(-5px); }
  .leader-status{ font-family:var(--mono); font-size:11px; color: var(--ink-faint); flex-shrink:0; text-transform:uppercase; }

  /* Info strip */
  .info-grid{ display:grid; grid-template-columns: repeat(auto-fit,minmax(190px,1fr)); gap:14px; }
  .info-card{ padding: 14px 16px; }
  .info-label{ font-family:var(--mono); font-size:10px; color:var(--ink-faint); text-transform:uppercase; letter-spacing:.05em; margin-bottom:5px; }
  .info-val{ font-size:14.5px; font-weight:600; }

  /* Footer */
  .footer{ background: var(--ink); color: var(--paper-card); margin-top:20px; padding: 30px 34px; display:flex; justify-content:space-between; flex-wrap:wrap; gap:14px; align-items:center; }
  .footer-note{ font-family:var(--mono); font-size:11.5px; color:#9B917A; }
  .footer-links{ display:flex; gap:16px; font-family:var(--mono); font-size:12.5px; flex-wrap:wrap; }
  .footer-links a{ color: var(--paper-card); text-decoration:none; border-bottom:1px solid #4A4536; }
  .footer-links a:hover{ border-color: var(--accent); color: var(--accent); }
</style>
</head>
<body>

<div class="wrap">
  <div class="topbar">
    <span>JAQR — Mechanical Design / Applied AI</span>
    <span>Companion profile</span>
  </div>
</div>

<div class="wrap">
  <div class="hero">
    <div class="hero-top">
      <span class="pill">001</span>
      <span class="hero-ref">CHIHUAHUA, MX — GMT-6</span>
    </div>
    <div class="hero-name">Javier Andrés<br>Quintero Rojas</div>
    <p class="hero-role">Mechanical Design Engineer working in CATIA V5 and GD&amp;T on commercial aircraft programs, building AI-assisted verification tools on the side. Two years in aerospace design, evaluating AI output with the same standard I hold engineering drawings to.</p>
    <div class="hero-bottom">
      <span class="hero-bottom-label">Aerospace Engineering — UACH</span>
      <span class="hero-bottom-label">javierquinro@gmail.com — +52 614 828 1961</span>
    </div>
  </div>
</div>

<div class="wrap">

  <section class="block">
    <div class="snap-grid">
      <div class="snap-card corners"><div class="snap-num">2+</div><div class="snap-label">Years, aerospace design</div></div>
      <div class="snap-card corners"><div class="snap-num">3</div><div class="snap-label">Aircraft/aerosystems programs</div></div>
      <div class="snap-card corners"><div class="snap-num">4</div><div class="snap-label">Certifications held</div></div>
      <div class="snap-card corners"><div class="snap-num">15–20</div><div class="snap-label">Hrs/wk available</div></div>
    </div>
  </section>

  <section class="block">
    <div class="rule-row"><span class="diamond">&#9671;</span> Capabilities</div>
    <div class="cap-grid">
      <div class="cap-card corners">
        <div class="cap-top"><span class="cap-num">001</span></div>
        <div class="cap-icon">
          <svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="1.4">
            <circle cx="32" cy="32" r="6"/><circle cx="32" cy="32" r="14"/><circle cx="32" cy="32" r="22"/>
          </svg>
        </div>
        <div class="cap-name">Design &amp; GD&amp;T</div>
        <div class="cap-caption">CATIA V5 surfacing, tolerancing, compliance review across commercial aircraft programs</div>
      </div>
      <div class="cap-card corners is-accent">
        <div class="cap-top"><span class="cap-num">002</span></div>
        <div class="cap-icon">
          <svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="1.4">
            <line x1="32" y1="10" x2="14" y2="52"/><line x1="32" y1="10" x2="50" y2="52"/>
            <line x1="21" y1="34" x2="43" y2="34"/><line x1="17" y1="44" x2="47" y2="44"/>
            <line x1="14" y1="52" x2="50" y2="52"/>
          </svg>
        </div>
        <div class="cap-name">Automation</div>
        <div class="cap-caption">CATIA and Excel VBA macros, PLC line automation, RFID tracking systems built end to end</div>
      </div>
      <div class="cap-card corners">
        <div class="cap-top"><span class="cap-num">003</span></div>
        <div class="cap-icon">
          <svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="1.4">
            <circle cx="24" cy="26" r="16"/><circle cx="40" cy="26" r="16"/><circle cx="32" cy="40" r="16"/>
          </svg>
        </div>
        <div class="cap-name">Applied AI evaluation</div>
        <div class="cap-caption">AI-assisted compliance tooling, data labeling, technical/STEM response review</div>
      </div>
    </div>
  </section>

  <section class="block">
    <div class="rule-row"><span class="diamond">&#9671;</span> Experience</div>
    <div class="job">
      <div class="job-when">Aug 2025 — Present</div>
      <div>
        <div class="job-role">Mechanical Design Engineer I — <span class="job-org">Safran Seats</span></div>
        <p>Leading CATIA V5 surfacing transferred from the France design team. Applying GD&amp;T across multiple international commercial aircraft seat programs. Built an AI-assisted GD&amp;T compliance checker and custom CATIA/Excel macros now used to automate recurring design steps.</p>
      </div>
    </div>
    <div class="job">
      <div class="job-when">Feb — Jun 2025</div>
      <div>
        <div class="job-role">Industrialization Intern — <span class="job-org">Safran Aerosystems</span></div>
        <p>Designed an overpressure test station fixture in CATIA V5, validated through TBF and VSM analysis. Built and coded an RFID-based tool tracking system. Led PDCA-based design improvements and new work instructions.</p>
      </div>
    </div>
    <div class="job">
      <div class="job-when">Feb — Jul 2024</div>
      <div>
        <div class="job-role">Design Engineer — <span class="job-org">Industrializadora SanZubia</span></div>
        <p>Designed precision brackets and couplings in Siemens NX. Automated a drawer production line with PLCs.</p>
      </div>
    </div>
    <p class="nda-line">— Aircraft program details are under NDA; scope above reflects what's disclosable.</p>
  </section>

  <section class="block">
    <div class="rule-row"><span class="diamond">&#9671;</span> Tools &amp; standards</div>
    <div class="tool-groups">
      <div>
        <div class="tool-label">CAD &amp; PLM</div>
        <div class="tool-pills">
          <span class="tool-pill">CATIA V5</span><span class="tool-pill">SmarTeam PLM</span>
          <span class="tool-pill">SolidWorks</span><span class="tool-pill">Siemens NX</span>
          <span class="tool-pill">Autodesk Inventor</span>
        </div>
      </div>
      <div>
        <div class="tool-label">Standards &amp; quality</div>
        <div class="tool-pills">
          <span class="tool-pill">GD&amp;T</span><span class="tool-pill">Lean Six Sigma</span>
          <span class="tool-pill">5S</span><span class="tool-pill">PDCA</span>
        </div>
      </div>
      <div>
        <div class="tool-label">Automation</div>
        <div class="tool-pills">
          <span class="tool-pill">Excel VBA</span><span class="tool-pill">CATIA macros</span>
          <span class="tool-pill">PLC programming</span><span class="tool-pill">RFID systems</span>
        </div>
      </div>
      <div>
        <div class="tool-label">Applied AI</div>
        <div class="tool-pills">
          <span class="tool-pill">AI Evaluation</span><span class="tool-pill">Data Labeling</span>
          <span class="tool-pill">AI-assisted coding</span><span class="tool-pill">STEM review</span>
        </div>
      </div>
    </div>
  </section>

  <section class="block">
    <div class="rule-row"><span class="diamond">&#9671;</span> Credentials</div>
    <div class="leader"><span class="leader-num">01</span><span class="leader-name">B.Sc. Aerospace Engineering</span><span class="leader-fill"></span><span class="leader-status">UACH, 2025</span></div>
    <div class="leader"><span class="leader-num">02</span><span class="leader-name">GD&amp;T Certification</span><span class="leader-fill"></span><span class="leader-status">Earned</span></div>
    <div class="leader"><span class="leader-num">03</span><span class="leader-name">CATIA Surfacing Certification</span><span class="leader-fill"></span><span class="leader-status">Earned</span></div>
    <div class="leader"><span class="leader-num">04</span><span class="leader-name">SolidWorks CSWA</span><span class="leader-fill"></span><span class="leader-status">CENALTEC, 2025</span></div>
    <div class="leader"><span class="leader-num">05</span><span class="leader-name">Lean Six Sigma Yellow Belt</span><span class="leader-fill"></span><span class="leader-status">Earned, 2025</span></div>
    <div class="leader"><span class="leader-num">06</span><span class="leader-name">TOEFL</span><span class="leader-fill"></span><span class="leader-status">ETS</span></div>
  </section>

  <section class="block">
    <div class="rule-row"><span class="diamond">&#9671;</span> Availability &amp; languages</div>
    <div class="info-grid">
      <div class="info-card corners"><div class="info-label">Location</div><div class="info-val">Chihuahua, Mexico (GMT-6)</div></div>
      <div class="info-card corners"><div class="info-label">Availability</div><div class="info-val">15–20 hrs/week</div></div>
      <div class="info-card corners"><div class="info-label">Spanish</div><div class="info-val">Native</div></div>
      <div class="info-card corners"><div class="info-label">English</div><div class="info-val">Fluent — C2</div></div>
      <div class="info-card corners"><div class="info-label">Mandarin</div><div class="info-val">Basic</div></div>
    </div>
  </section>

</div>

<div class="footer">
  <span class="footer-note">Full resume available on request.</span>
  <div class="footer-links">
    <a href="mailto:javierquinro@gmail.com">javierquinro@gmail.com</a>
    <a href="tel:+526148281961">+52 614 828 1961</a>
    <a href="https://linkedin.com/in/jaqraerospace">linkedin.com/in/jaqraerospace</a>
  </div>
</div>

</body>
</html>
