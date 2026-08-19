<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pratishtha Kiran | Customer Success & Enterprise Account Leadership</title>
  <meta name="description" content="Five years owning enterprise accounts for American Express and Google. CSAT turnaround 4.1 to 4.9, 98% SLA, team of 82. IIM Nagpur PGDM.">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-base: #0a0d14;
      --bg-surface: #111622;
      --bg-card: #182030;
      --border: rgba(255, 255, 255, 0.08);
      --text-main: #f3f4f6;
      --text-muted: #9ca3af;
      --accent: #6366f1;
      --accent-light: #818cf8;
      --accent-emerald: #10b981;
      --font: 'Plus Jakarta Sans', -apple-system, BlinkMacSystemFont, sans-serif;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    body {
      font-family: var(--font);
      background-color: var(--bg-base);
      color: var(--text-main);
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
    }

    a { color: inherit; text-decoration: none; }
    .container { max-width: 1140px; margin: 0 auto; padding: 0 24px; }

    /* Header */
    header {
      position: sticky;
      top: 0;
      background: rgba(10, 13, 20, 0.88);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--border);
      z-index: 100;
      padding: 16px 0;
    }
    .nav-wrap { display: flex; justify-content: space-between; align-items: center; }
    .logo { font-size: 1.25rem; font-weight: 800; letter-spacing: -0.5px; color: #fff; }
    .logo span { color: var(--accent-light); }
    .nav-menu { display: flex; gap: 20px; align-items: center; }
    .nav-menu a {
      font-size: 0.84rem;
      font-weight: 600;
      color: var(--text-muted);
      letter-spacing: 0.5px;
      text-transform: uppercase;
      transition: color 0.2s;
    }
    .nav-menu a:hover { color: #fff; }
    
    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      padding: 9px 18px;
      border-radius: 8px;
      font-size: 0.88rem;
      font-weight: 600;
      transition: all 0.2s;
      cursor: pointer;
    }
    .btn-primary {
      background: linear-gradient(135deg, #4f46e5 0%, #7c3aed 100%);
      color: #fff;
      border: none;
    }
    .btn-primary:hover { opacity: 0.95; transform: translateY(-1px); }
    .btn-outline {
      background: rgba(255, 255, 255, 0.04);
      border: 1px solid var(--border);
      color: var(--text-main);
    }
    .btn-outline:hover { background: rgba(255, 255, 255, 0.08); border-color: rgba(255, 255, 255, 0.2); }

    /* Ticker Tape */
    .ticker {
      background: #111827;
      border-top: 1px solid var(--border);
      border-bottom: 1px solid var(--border);
      overflow: hidden;
      white-space: nowrap;
      padding: 10px 0;
      font-size: 0.82rem;
      font-weight: 600;
      color: var(--accent-light);
      letter-spacing: 0.5px;
    }
    .ticker-content {
      display: inline-block;
      animation: marquee 25s linear infinite;
    }
    @keyframes marquee {
      0% { transform: translateX(0); }
      100% { transform: translateX(-50%); }
    }

    /* Hero */
    .hero { padding: 70px 0 50px; }
    .hero-grid {
      display: grid;
      grid-template-columns: 1.2fr 0.8fr;
      gap: 40px;
      align-items: center;
    }
    .location-badge {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      background: rgba(16, 185, 129, 0.1);
      border: 1px solid rgba(16, 185, 129, 0.25);
      color: var(--accent-emerald);
      padding: 4px 12px;
      border-radius: 50px;
      font-size: 0.8rem;
      font-weight: 600;
      margin-bottom: 20px;
    }
    .hero-h1 {
      font-size: 2.6rem;
      line-height: 1.15;
      font-weight: 800;
      letter-spacing: -1px;
      margin-bottom: 18px;
    }
    .hero-p {
      font-size: 1.05rem;
      color: var(--text-muted);
      margin-bottom: 28px;
      line-height: 1.65;
    }
    .hero-actions { display: flex; gap: 12px; flex-wrap: wrap; }

    .hero-card {
      background: var(--bg-surface);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 28px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.3);
    }
    .hero-stat-row {
      display: flex;
      justify-content: space-between;
      border-bottom: 1px solid var(--border);
      padding-bottom: 14px;
      margin-bottom: 14px;
    }
    .hero-stat-row:last-child { border: none; padding: 0; margin: 0; }
    .hero-stat-label { font-size: 0.85rem; color: var(--text-muted); }
    .hero-stat-val { font-weight: 700; color: #fff; font-size: 0.95rem; }

    /* Sections */
    .section { padding: 70px 0; border-top: 1px solid var(--border); }
    .sec-tag {
      font-size: 0.8rem;
      font-weight: 700;
      color: var(--accent-light);
      text-transform: uppercase;
      letter-spacing: 1px;
      margin-bottom: 6px;
      display: block;
    }
    .sec-title { font-size: 1.85rem; font-weight: 800; letter-spacing: -0.5px; margin-bottom: 30px; }

    /* Metrics 4-Grid */
    .metrics-4 {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 16px;
      margin-bottom: 36px;
    }
    .m-box {
      background: var(--bg-surface);
      border: 1px solid var(--border);
      border-radius: 14px;
      padding: 24px;
    }
    .m-num {
      font-size: 2rem;
      font-weight: 800;
      color: #fff;
      margin-bottom: 4px;
    }
    .m-num.accent { color: var(--accent-light); }
    .m-lbl { font-size: 0.85rem; color: var(--text-muted); font-weight: 500; }

    /* Analysis Split */
    .analysis-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 24px;
    }
    .card {
      background: var(--bg-surface);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 28px;
    }
    .card-h3 { font-size: 1.1rem; font-weight: 700; margin-bottom: 20px; color: #fff; }

    /* Skills Bars */
    .skill-row { margin-bottom: 16px; }
    .skill-head { display: flex; justify-content: space-between; font-size: 0.85rem; font-weight: 600; margin-bottom: 6px; }
    .skill-bar { height: 7px; background: rgba(255,255,255,0.06); border-radius: 50px; overflow: hidden; }
    .skill-fill { height: 100%; background: linear-gradient(90deg, #4f46e5, #818cf8); border-radius: 50px; }

    /* Video Player */
    .film-wrap {
      max-width: 820px;
      margin: 0 auto;
      background: var(--bg-surface);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 24px;
    }
    .vid-box {
      position: relative;
      width: 100%;
      padding-bottom: 56.25%;
      height: 0;
      border-radius: 10px;
      overflow: hidden;
      background: #000;
      margin-bottom: 14px;
    }
    .vid-box iframe, .vid-box video {
      position: absolute; top: 0; left: 0; width: 100%; height: 100%; border: 0;
    }

    /* Cover Letter & Resume Split */
    .resume-split {
      display: grid;
      grid-template-columns: 1fr 1.2fr;
      gap: 28px;
    }
    .letter-box {
      background: var(--bg-surface);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 30px;
      font-size: 0.94rem;
      color: #d1d5db;
      line-height: 1.7;
    }
    .letter-box p { margin-bottom: 16px; }
    .letter-box blockquote {
      border-left: 3px solid var(--accent-light);
      padding-left: 14px;
      font-style: italic;
      color: #fff;
      margin: 16px 0;
    }

    /* Timeline */
    .exp-item {
      position: relative;
      padding-left: 24px;
      border-left: 2px solid var(--border);
      margin-bottom: 24px;
    }
    .exp-item:last-child { margin-bottom: 0; border-left-color: transparent; }
    .exp-dot {
      position: absolute;
      left: -6px;
      top: 4px;
      width: 10px;
      height: 10px;
      border-radius: 50%;
      background: var(--accent-light);
    }
    .exp-role { font-size: 1.05rem; font-weight: 700; color: #fff; }
    .exp-sub { font-size: 0.84rem; color: var(--accent-light); margin-bottom: 6px; }
    .exp-desc { font-size: 0.88rem; color: var(--text-muted); line-height: 1.5; }

    /* Work 4-Grid */
    .work-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 18px;
    }
    .work-card {
      background: var(--bg-surface);
      border: 1px solid var(--border);
      border-radius: 14px;
      padding: 24px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }
    .work-tag { font-size: 0.75rem; font-weight: 700; color: var(--accent-light); text-transform: uppercase; margin-bottom: 8px; }
    .work-h4 { font-size: 1.05rem; font-weight: 700; margin-bottom: 10px; color: #fff; }
    .work-p { font-size: 0.88rem; color: var(--text-muted); line-height: 1.55; }

    .tag-cloud { display: flex; flex-wrap: wrap; gap: 8px; margin-top: 12px; }
    .tag {
      background: rgba(255,255,255,0.05);
      border: 1px solid var(--border);
      border-radius: 6px;
      padding: 4px 10px;
      font-size: 0.8rem;
      color: #e5e7eb;
    }

    /* Contact CTA */
    .contact-card {
      background: linear-gradient(135deg, rgba(79, 70, 229, 0.15) 0%, rgba(124, 58, 237, 0.15) 100%);
      border: 1px solid rgba(99, 102, 241, 0.3);
      border-radius: 16px;
      padding: 48px 32px;
      text-align: center;
    }
    .contact-links { display: flex; justify-content: center; gap: 14px; flex-wrap: wrap; margin-top: 24px; }

    footer {
      padding: 36px 0;
      text-align: center;
      font-size: 0.85rem;
      color: var(--text-muted);
      border-top: 1px solid var(--border);
    }

    @media (max-width: 860px) {
      .hero-grid, .analysis-grid, .resume-split { grid-template-columns: 1fr; }
      .nav-menu { display: none; }
      .hero-h1 { font-size: 2.1rem; }
    }
  </style>
</head>
<body>

  <header>
    <div class="container nav-wrap">
      <div class="logo">Pratishtha<span>.</span></div>
      <nav class="nav-menu">
        <a href="#analysis">The Analysis</a>
        <a href="#film">The Film</a>
        <a href="#resume">Résumé</a>
        <a href="#work">Portfolio</a>
        <a href="#person">The Person</a>
        <a href="#contact">Say Hello</a>
      </nav>
      <a href="#contact" class="btn btn-primary">Say Hello</a>
    </div>
  </header>

  <div class="ticker">
    <div class="ticker-content">
      Escalation Management &nbsp;•&nbsp; Retention & Expansion &nbsp;•&nbsp; Account Health Scoring &nbsp;•&nbsp; 98% SLA &nbsp;•&nbsp; CSAT 4.8+ &nbsp;•&nbsp; Onboarding &nbsp;•&nbsp; QBRs & Reviews &nbsp;•&nbsp; Rebuilt Cadences &nbsp;•&nbsp; Escalation Management &nbsp;•&nbsp; Retention & Expansion &nbsp;•&nbsp; Account Health Scoring &nbsp;•&nbsp; 98% SLA &nbsp;•&nbsp; CSAT 4.8+
    </div>
  </div>

  <section class="hero">
    <div class="container hero-grid">
      <div>
        <div class="location-badge">📍 Bengaluru, India • Open to CS & Key Account Roles</div>
        <h1 class="hero-h1">"Customers stay when someone cares. I'm that someone."</h1>
        <p class="hero-p">
          Five years owning enterprise accounts for American Express and Google — onboarding, QBRs, escalations, renewals — with an IIM Nagpur PGDM on top. This page is my whole story in one link: the résumé, the letter, the analysis, and the film.
        </p>
        <div class="hero-actions">
          <a href="#analysis" class="btn btn-primary">Read the Analysis</a>
          <a href="#film" class="btn btn-outline">Watch the Film</a>
          <a href="resume.pdf" class="btn btn-outline" download target="_blank">Download Résumé (PDF)</a>
        </div>
      </div>

      <div class="hero-card">
        <div class="hero-stat-row">
          <span class="hero-stat-label">Core Specialization</span>
          <span class="hero-stat-val">Enterprise Customer Success & Ops</span>
        </div>
        <div class="hero-stat-row">
          <span class="hero-stat-label">Clients Managed</span>
          <span class="hero-stat-val">American Express, Google</span>
        </div>
        <div class="hero-stat-row">
          <span class="hero-stat-label">Stakeholders Scaled</span>
          <span class="hero-stat-val">3,000+ Users Daily</span>
        </div>
        <div class="hero-stat-row">
          <span class="hero-stat-label">Team Leadership</span>
          <span class="hero-stat-val">82 Direct & Site Associates</span>
        </div>
        <div class="hero-stat-row">
          <span class="hero-stat-label">Education</span>
          <span class="hero-stat-val">PGDM, IIM Nagpur</span>
        </div>
      </div>
    </div>
  </section>

  <!-- 01 The Analysis -->
  <section class="section" id="analysis">
    <div class="container">
      <span class="sec-tag">01 What I'm Made Of</span>
      <h2 class="sec-title">The Analysis</h2>

      <div class="metrics-4">
        <div class="m-box">
          <div class="m-num">3,000+</div>
          <div class="m-lbl">Enterprise stakeholders served</div>
        </div>
        <div class="m-box">
          <div class="m-num accent">4.1 → 4.9</div>
          <div class="m-lbl">CSAT turnaround in 60 days</div>
        </div>
        <div class="m-box">
          <div class="m-num">98%</div>
          <div class="m-lbl">SLA held throughout</div>
        </div>
        <div class="m-box">
          <div class="m-num">82</div>
          <div class="m-lbl">Team members led</div>
        </div>
      </div>

      <div class="analysis-grid">
        <div class="card">
          <h3 class="card-h3">Work Style & Attributes</h3>
          <div style="width: 100%; height: 260px; display: flex; justify-content: center; align-items: center;">
            <canvas id="radarChart" width="280" height="260"></canvas>
          </div>
          <div class="tag-cloud" style="justify-content: center; margin-top: 16px;">
            <span class="tag">Customer-first</span>
            <span class="tag">Calm in escalations</span>
            <span class="tag">Data-driven</span>
            <span class="tag">Writes the playbook</span>
          </div>
        </div>

        <div class="card">
          <h3 class="card-h3">Top Competencies</h3>
          <div class="skill-row">
            <div class="skill-head"><span>Onboarding & Activation</span><span>96%</span></div>
            <div class="skill-bar"><div class="skill-fill" style="width: 96%;"></div></div>
          </div>
          <div class="skill-row">
            <div class="skill-head"><span>Escalation Management</span><span>95%</span></div>
            <div class="skill-bar"><div class="skill-fill" style="width: 95%;"></div></div>
          </div>
          <div class="skill-row">
            <div class="skill-head"><span>Playbooks & SOPs</span><span>94%</span></div>
            <div class="skill-bar"><div class="skill-fill" style="width: 94%;"></div></div>
          </div>
          <div class="skill-row">
            <div class="skill-head"><span>Account Health & Risk</span><span>93%</span></div>
            <div class="skill-bar"><div class="skill-fill" style="width: 93%;"></div></div>
          </div>
          <div class="skill-row">
            <div class="skill-head"><span>QBRs & Business Reviews</span><span>92%</span></div>
            <div class="skill-bar"><div class="skill-fill" style="width: 92%;"></div></div>
          </div>
          <div class="skill-row">
            <div class="skill-head"><span>Retention & Expansion</span><span>90%</span></div>
            <div class="skill-bar"><div class="skill-fill" style="width: 90%;"></div></div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- 02 The Film -->
  <section class="section" id="film">
    <div class="container">
      <div style="text-align: center; margin-bottom: 30px;">
        <span class="sec-tag">02 Hear It From The AI Me</span>
        <h2 class="sec-title">The Film</h2>
        <p style="color: var(--text-muted); font-size: 0.95rem;">A 48-second walkthrough of my operational approach, built with Google Flow & ElevenLabs.</p>
      </div>

      <div class="film-wrap">
        <video controls playsinline preload="metadata" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 10px; background: #000;">
  <source src="intro-video.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
        <div style="display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 12px; font-size: 0.85rem; color: var(--text-muted);">
          <span>⏱️ Length: 48 seconds</span>
          <a href="mailto:pratishthakiranvt@gmail.com" style="color: var(--accent-light); text-decoration: underline;">Request full case walk-through</a>
        </div>
      </div>
    </div>
  </section>

  <!-- 03 Résumé & Cover Letter -->
  <section class="section" id="resume">
    <div class="container">
      <span class="sec-tag">03 On Paper, In Person</span>
      <h2 class="sec-title">Résumé & Cover Letter</h2>

      <div class="resume-split">
        <div class="letter-box">
          <h3 style="font-size: 1.15rem; font-weight: 700; color: #fff; margin-bottom: 16px;">A Letter, Briefly</h3>
          <p>Most cover letters open with a summary of what a candidate has done. I want to open with a number instead: <strong>4.1 to 4.9</strong>.</p>
          <p>That's the CSAT score I inherited on the American Express account at Sodexo, and where I took it within two months — sustained above 4.8 for the rest of the engagement, on an account serving 3,000+ stakeholders with a team of 82 reporting to me.</p>
          <blockquote>
            "For 5+ years I've built my career in hospitality and enterprise services — industries where the customer is right there, expectations are immediate, and there's nowhere to hide behind a process."
          </blockquote>
          <p>I've sat across the table from enterprise stakeholders at American Express and Google, managed escalations, and owned SLAs and QBRs against real consequences, not hypotheticals.</p>
          <p>If you're looking for someone who has already been doing the work of Customer Success — under different job titles, with real accounts and real consequences — I'd welcome the conversation about how that translates to your customers.</p>
          <p style="margin-top: 20px; font-weight: 600; color: #fff;">Warm regards,<br>Pratishtha</p>
          <a href="cover-letter.pdf" class="btn btn-outline" style="margin-top: 16px; font-size: 0.82rem;" download target="_blank">Download Letter (PDF)</a>
        </div>

        <div class="card">
          <h3 class="card-h3">Experience Timeline</h3>
          
          <div class="exp-item">
            <div class="exp-dot"></div>
            <div class="exp-role">Stakeholder & Site Operations Manager</div>
            <div class="exp-sub">Sodexo (Client: American Express) | Oct 2025 – Present</div>
            <div class="exp-desc">
              Owned the end-to-end customer journey for a major US enterprise client — 3,000+ stakeholders, team of 82. Rebuilt escalation paths; CSAT 4.1 → 4.9 in 60 days. Held 98% SLA and presented insights in QBRs.
            </div>
          </div>

          <div class="exp-item">
            <div class="exp-dot"></div>
            <div class="exp-role">Frontline Operations Manager</div>
            <div class="exp-sub">Sodexo (Client: Google) | Oct 2024 – Oct 2025</div>
            <div class="exp-desc">
              Owned day-to-day customer success and account management for a high-profile US tech client across 12 touchpoints. Developed escalation playbooks and trained teams to one delivery standard.
            </div>
          </div>

          <div class="exp-item">
            <div class="exp-dot"></div>
            <div class="exp-role">Brand Operations & Business Development Head</div>
            <div class="exp-sub">VietNom India | Oct 2023 – Oct 2024</div>
            <div class="exp-desc">
              Owned client relationships for five B2B contracts; improved retention 15% through proactive onboarding. Built operational playbooks and scaled standard frameworks.
            </div>
          </div>

          <div class="exp-item">
            <div class="exp-dot"></div>
            <div class="exp-role">Operations & Hospitality Manager</div>
            <div class="exp-sub">ITC Hotels | Aug 2021 – Oct 2023</div>
            <div class="exp-desc">
              Delivered high-touch service to VIP clients; authored SOPs and playbooks that standardized quality across luxury properties.
            </div>
          </div>

          <div style="margin-top: 24px; padding-top: 18px; border-top: 1px solid var(--border);">
            <h4 style="font-size: 0.95rem; font-weight: 700; margin-bottom: 8px;">Education</h4>
            <p style="font-size: 0.85rem; color: var(--text-muted);">
              • <strong>PGDM (Product & Brand Management)</strong> — IIM Nagpur (2024–2025)<br>
              • <strong>B.Sc. (Hospitality & Hotel Administration)</strong> — IHM Bhopal (2017–2020)
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- 04 Selected Work -->
  <section class="section" id="work">
    <div class="container">
      <span class="sec-tag">04 Things I've Built & Hosted</span>
      <h2 class="sec-title">Selected Work & Portfolio</h2>

      <div class="work-grid">
        <div class="work-card">
          <div>
            <div class="work-tag">Turnaround</div>
            <h4 class="work-h4">The Enterprise Turnaround</h4>
            <p class="work-p">
              Inherited an account with trust breaking down at American Express. Rebuilt escalation paths, tightened accountability, and instituted daily cadences. CSAT 4.1 → 4.9 in 60 days; 98% SLA maintained.
            </p>
          </div>
        </div>

        <div class="work-card">
          <div>
            <div class="work-tag">Governance</div>
            <h4 class="work-h4">Tech Account Governance</h4>
            <p class="work-p">
              Unified 12 touchpoints at Google into one operating rhythm with escalation playbooks and QBR-style reviews — strengthening client trust, adoption, and retention.
            </p>
          </div>
        </div>

        <div class="work-card">
          <div>
            <div class="work-tag">Systems</div>
            <h4 class="work-h4">CRM Rollout for Expansion</h4>
            <p class="work-p">
              Implemented a CRM mapping employee journeys with an NPS feedback loop — deployed across the new American Express site without disrupting service.
            </p>
          </div>
        </div>

        <div class="work-card">
          <div>
            <div class="work-tag">AI Innovation</div>
            <h4 class="work-h4">This Portfolio System</h4>
            <p class="work-p">
              Architected with Claude, filmed with Google Flow, voiced with ElevenLabs, and deployed on GitHub Pages as a permanent interactive briefing.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- 05 Off The Clock -->
  <section class="section" id="person">
    <div class="container">
      <span class="sec-tag">05 The Person Behind The Résumé</span>
      <h2 class="sec-title">Off The Clock</h2>

      <div class="work-grid" style="grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));">
        <div class="card">
          <h3 class="card-h3">How I Communicate</h3>
          <p style="font-size: 0.9rem; color: var(--text-muted); margin-bottom: 14px;">
            Warm, direct, and unhurried. <em>"In a room full of voices, I listen for what isn't being said — then I answer that."</em>
          </p>
          <div class="tag-cloud">
            <span class="tag">Warm but precise</span>
            <span class="tag">Listens first</span>
            <span class="tag">Says the hard thing kindly</span>
            <span class="tag">Zero jargon</span>
          </div>
        </div>

        <div class="card">
          <h3 class="card-h3">Lifelong Certifications</h3>
          <ul style="font-size: 0.85rem; color: var(--text-muted); list-style: none; display: flex; flex-direction: column; gap: 6px;">
            <li>✓ Google Project Management Professional Certificate</li>
            <li>✓ SQL Certification — LearnSQL.com</li>
            <li>✓ Revenue Management — ESSEC Business School</li>
            <li>✓ Finance for Managers — IESE Business School</li>
            <li>✓ Digital Marketing — Google Certified</li>
            <li>✓ Public Relations — SWAYAM, Chandigarh University</li>
            <li>✓ Diploma in HR Development — AIIMAS Chennai</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- 06 Contact -->
  <section class="section" id="contact">
    <div class="container">
      <div class="contact-card">
        <span class="sec-tag" style="color: var(--accent-light);">06 Let's Talk</span>
        <h2 style="font-size: 2.2rem; font-weight: 800; margin: 8px 0 12px;">One Link, One Hello.</h2>
        <p style="color: var(--text-muted); font-size: 1rem; max-width: 600px; margin: 0 auto;">
          Looking for a Customer Success or Key Account Leader who has managed real enterprise accounts under pressure? Let's connect.
        </p>
        <div class="contact-links">
          <a href="mailto:pratishthakiranvt@gmail.com" class="btn btn-primary">pratishthakiranvt@gmail.com</a>
          <a href="https://linkedin.com/in/pratishthakiran" target="_blank" class="btn btn-outline">LinkedIn Profile</a>
          <a href="tel:+918269722787" class="btn btn-outline">+91 8269722787</a>
        </div>
      </div>
    </div>
  </section>

  <footer>
    <div class="container">
      <p style="font-style: italic; margin-bottom: 8px;">"Luxury is a feeling, not a fixture."</p>
      <p>© 2026 Pratishtha Kiran • Permanent GitHub Dossier</p>
    </div>
  </footer>

  <script>
    window.addEventListener('DOMContentLoaded', () => {
      const canvas = document.getElementById('radarChart');
      if (!canvas) return;
      const ctx = canvas.getContext('2d');
      const centerX = 140, centerY = 130, radius = 90;
      const labels = ['Ownership', 'Composure', 'Empathy', 'Rigour', 'Communication', 'Adaptability'];
      const values = [0.95, 0.90, 0.94, 0.92, 0.95, 0.88];
      const total = labels.length;

      ctx.strokeStyle = 'rgba(255, 255, 255, 0.1)';
      ctx.lineWidth = 1;
      for (let r = 0.2; r <= 1.0; r += 0.2) {
        ctx.beginPath();
        for (let i = 0; i < total; i++) {
          const angle = (Math.PI * 2 / total) * i - Math.PI / 2;
          const x = centerX + Math.cos(angle) * radius * r;
          const y = centerY + Math.sin(angle) * radius * r;
          if (i === 0) ctx.moveTo(x, y);
          else ctx.lineTo(x, y);
        }
        ctx.closePath();
        ctx.stroke();
      }

      for (let i = 0; i < total; i++) {
        const angle = (Math.PI * 2 / total) * i - Math.PI / 2;
        ctx.beginPath();
        ctx.moveTo(centerX, centerY);
        ctx.lineTo(centerX + Math.cos(angle) * radius, centerY + Math.sin(angle) * radius);
        ctx.stroke();
      }

      ctx.beginPath();
      for (let i = 0; i < total; i++) {
        const angle = (Math.PI * 2 / total) * i - Math.PI / 2;
        const x = centerX + Math.cos(angle) * radius * values[i];
        const y = centerY + Math.sin(angle) * radius * values[i];
        if (i === 0) ctx.moveTo(x, y);
        else ctx.lineTo(x, y);
      }
      ctx.closePath();
      ctx.fillStyle = 'rgba(99, 102, 241, 0.4)';
      ctx.fill();
      ctx.strokeStyle = '#818cf8';
      ctx.lineWidth = 2;
      ctx.stroke();

      ctx.fillStyle = '#9ca3af';
      ctx.font = '10px Plus Jakarta Sans, sans-serif';
      ctx.textAlign = 'center';
      for (let i = 0; i < total; i++) {
        const angle = (Math.PI * 2 / total) * i - Math.PI / 2;
        const x = centerX + Math.cos(angle) * (radius + 18);
        const y = centerY + Math.sin(angle) * (radius + 14);
        ctx.fillText(labels[i], x, y);
      }
    });
  </script>

</body>
</html># Pratishtha Portfolio
