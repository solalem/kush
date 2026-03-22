---
title: "Portfolio - Solomon Amognu"
layout: "empty"
---

{{< section-container class="bg-gradient-to-b from-blue-50 via-blue-50 to-white pt-20 pb-32" >}}

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Solomon Amognu — Solution Architect</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;500;600;700;800&family=IBM+Plex+Mono:wght@300;400;500&family=Fraunces:ital,wght@0,300;0,400;1,300;1,400&display=swap" rel="stylesheet">
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --ink: #0f0e0b;
    --paper: #f5f0e8;
    --amber: #d4700a;
    --amber-light: #f0a030;
    --moss: #2a3a2a;
    --rust: #8b3a1a;
    --cream: #faf7f0;
    --line: rgba(15,14,11,0.12);
  }

  html { scroll-behavior: smooth; }

  body {
    background: var(--paper);
    color: var(--ink);
    font-family: 'IBM Plex Mono', monospace;
    font-size: 13px;
    line-height: 1.7;
    overflow-x: hidden;
  }

  /* ── NAV ── */
  nav {
    position: fixed; top: 0; left: 0; right: 0; z-index: 100;
    display: flex; justify-content: space-between; align-items: center;
    padding: 1.2rem 3rem;
    background: var(--paper);
    border-bottom: 1px solid var(--line);
    backdrop-filter: blur(8px);
  }
  .nav-logo {
    font-family: 'Syne', sans-serif;
    font-weight: 800; font-size: 1rem;
    letter-spacing: -0.02em; color: var(--ink);
    text-decoration: none;
  }
  .nav-links { display: flex; gap: 2.5rem; list-style: none; }
  .nav-links a {
    color: var(--ink); text-decoration: none; font-size: 11px;
    letter-spacing: 0.12em; text-transform: uppercase; opacity: 0.6;
    transition: opacity 0.2s;
  }
  .nav-links a:hover { opacity: 1; }

  /* ── HERO ── */
  .hero {
    min-height: 100vh;
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding-top: 4rem;
  }
  .hero-left {
    display: flex; flex-direction: column; justify-content: center;
    padding: 5rem 3rem 5rem 3rem;
    border-right: 1px solid var(--line);
  }
  .hero-tag {
    font-size: 10px; letter-spacing: 0.18em; text-transform: uppercase;
    color: var(--amber); margin-bottom: 1.5rem;
    display: flex; align-items: center; gap: 0.8rem;
  }
  .hero-tag::before { content: ''; display: block; width: 2rem; height: 1px; background: var(--amber); }
  h1 {
    font-family: 'Fraunces', serif;
    font-size: clamp(3rem, 6vw, 5.5rem);
    font-weight: 300; line-height: 1.05;
    letter-spacing: -0.02em;
    color: var(--ink);
    margin-bottom: 0.3rem;
  }
  h1 em { font-style: italic; color: var(--amber); }
  .hero-title {
    font-family: 'Syne', sans-serif;
    font-size: clamp(0.7rem, 1.2vw, 0.9rem);
    letter-spacing: 0.15em; text-transform: uppercase;
    color: var(--moss); margin-bottom: 2.5rem; margin-top: 0.5rem;
  }
  .hero-summary {
    max-width: 42ch; font-size: 12.5px; opacity: 0.75;
    line-height: 1.8; margin-bottom: 3rem;
  }
  .hero-cta {
    display: inline-flex; align-items: center; gap: 0.7rem;
    background: var(--ink); color: var(--paper);
    padding: 0.8rem 1.8rem; font-family: 'Syne', sans-serif;
    font-size: 11px; font-weight: 600; letter-spacing: 0.12em;
    text-transform: uppercase; text-decoration: none;
    transition: background 0.25s;
  }
  .hero-cta:hover { background: var(--amber); }
  .hero-cta::after { content: '→'; font-size: 1rem; }

  .hero-right {
    display: flex; flex-direction: column; justify-content: flex-end;
    padding: 5rem 3rem 5rem 4rem;
    position: relative;
  }
  .hero-stats {
    display: grid; grid-template-columns: 1fr 1fr;
    gap: 0; border: 1px solid var(--line);
    margin-bottom: 3rem;
  }
  .stat {
    padding: 1.8rem 1.5rem;
    border-right: 1px solid var(--line);
    border-bottom: 1px solid var(--line);
  }
  .stat:nth-child(2n) { border-right: none; }
  .stat:nth-child(3), .stat:nth-child(4) { border-bottom: none; }
  .stat-num {
    font-family: 'Fraunces', serif; font-size: 2.8rem;
    font-weight: 300; color: var(--amber); line-height: 1;
    margin-bottom: 0.3rem;
  }
  .stat-label { font-size: 10px; letter-spacing: 0.1em; text-transform: uppercase; opacity: 0.55; }

  .hero-stack {
    font-size: 10px; letter-spacing: 0.05em;
    opacity: 0.45; line-height: 2;
  }
  .hero-stack strong {
    font-family: 'Syne', sans-serif; letter-spacing: 0.1em;
    text-transform: uppercase; font-size: 9px; color: var(--amber);
    opacity: 1; display: block; margin-bottom: 0.5rem;
  }

  /* ── SECTION COMMON ── */
  section { border-top: 1px solid var(--line); }
  .section-inner { max-width: 1200px; margin: 0 auto; padding: 6rem 3rem; }
  .section-label {
    font-size: 9px; letter-spacing: 0.2em; text-transform: uppercase;
    color: var(--amber); margin-bottom: 3rem;
    display: flex; align-items: center; gap: 1rem;
  }
  .section-label::after { content: ''; flex: 1; height: 1px; background: var(--line); }
  h2 {
    font-family: 'Fraunces', serif; font-size: clamp(2rem, 4vw, 3.2rem);
    font-weight: 300; line-height: 1.15; letter-spacing: -0.02em;
    margin-bottom: 3rem;
  }

  /* ── SKILLS ── */
  #skills .section-inner {
    display: grid; grid-template-columns: 1fr 2fr; gap: 5rem; align-items: start;
  }
  .skills-grid { display: flex; flex-direction: column; gap: 2.5rem; }
  .skill-group {}
  .skill-group-title {
    font-family: 'Syne', sans-serif; font-size: 10px; font-weight: 700;
    letter-spacing: 0.15em; text-transform: uppercase;
    color: var(--moss); margin-bottom: 1rem;
    padding-bottom: 0.5rem; border-bottom: 1px solid var(--line);
  }
  .skill-tags { display: flex; flex-wrap: wrap; gap: 0.4rem; }
  .tag {
    display: inline-block; padding: 0.3rem 0.7rem;
    background: var(--cream); border: 1px solid var(--line);
    font-size: 10.5px; letter-spacing: 0.03em;
    transition: border-color 0.2s, color 0.2s;
  }
  .tag:hover { border-color: var(--amber); color: var(--amber); }

  /* ── EXPERIENCE ── */
  .timeline { display: flex; flex-direction: column; gap: 0; }
  .timeline-item {
    display: grid; grid-template-columns: 14rem 1fr;
    border-bottom: 1px solid var(--line);
    padding: 2.5rem 0;
    transition: background 0.2s;
  }
  .timeline-item:hover { background: rgba(212,112,10,0.03); }
  .timeline-meta { padding-right: 2rem; }
  .tl-dates {
    font-size: 10px; letter-spacing: 0.08em; color: var(--amber);
    margin-bottom: 0.4rem;
  }
  .tl-company { font-size: 11px; opacity: 0.5; }
  .tl-location { font-size: 10px; opacity: 0.35; margin-top: 0.2rem; }
  .tl-role {
    font-family: 'Syne', sans-serif; font-size: 1.05rem; font-weight: 700;
    letter-spacing: -0.01em; margin-bottom: 0.8rem;
  }
  .tl-desc { font-size: 12px; opacity: 0.65; max-width: 58ch; line-height: 1.8; }

  /* ── PROJECTS ── */
  .projects-grid {
    display: grid; grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
    gap: 1.5rem;
  }
  .project-card {
    border: 1px solid var(--line); padding: 2rem;
    background: var(--cream);
    transition: border-color 0.25s, transform 0.25s;
    position: relative; overflow: hidden;
  }
  .project-card::before {
    content: '';
    position: absolute; top: 0; left: 0; right: 0; height: 2px;
    background: var(--amber);
    transform: scaleX(0); transform-origin: left;
    transition: transform 0.3s;
  }
  .project-card:hover { border-color: var(--amber); transform: translateY(-2px); }
  .project-card:hover::before { transform: scaleX(1); }
  .project-client {
    font-size: 9px; letter-spacing: 0.18em; text-transform: uppercase;
    color: var(--amber); margin-bottom: 0.6rem;
  }
  .project-name {
    font-family: 'Syne', sans-serif; font-size: 0.95rem; font-weight: 700;
    margin-bottom: 0.8rem; line-height: 1.3;
  }
  .project-desc { font-size: 11.5px; opacity: 0.6; line-height: 1.8; margin-bottom: 1.2rem; }
  .project-role {
    display: inline-block; font-size: 9.5px; letter-spacing: 0.1em;
    text-transform: uppercase; padding: 0.2rem 0.6rem;
    border: 1px solid var(--line); color: var(--moss);
  }

  /* ── NOTABLE ── */
  .notable-list { display: flex; flex-direction: column; gap: 1px; }
  .notable-item {
    display: flex; justify-content: space-between; align-items: baseline;
    padding: 1.2rem 0; border-bottom: 1px solid var(--line);
    gap: 2rem;
  }
  .notable-name {
    font-family: 'Syne', sans-serif; font-weight: 600; font-size: 0.88rem;
  }
  .notable-tag-label {
    font-size: 10px; opacity: 0.4; white-space: nowrap;
    font-style: italic; font-family: 'Fraunces', serif;
  }

  /* ── EDUCATION ── */
  #education .section-inner {
    display: grid; grid-template-columns: 1fr 1fr; gap: 5rem; align-items: start;
  }
  .edu-block {
    border: 1px solid var(--line); padding: 2.5rem;
    background: var(--cream);
  }
  .edu-degree {
    font-family: 'Fraunces', serif; font-size: 1.3rem; font-weight: 300;
    font-style: italic; margin-bottom: 0.8rem;
  }
  .edu-school { font-family: 'Syne', sans-serif; font-weight: 700; margin-bottom: 0.3rem; }
  .edu-date { font-size: 11px; color: var(--amber); }

  /* ── FOOTER ── */
  footer {
    border-top: 1px solid var(--line);
    padding: 3rem;
    display: flex; justify-content: space-between; align-items: center;
    background: var(--ink); color: var(--paper);
  }
  .footer-name {
    font-family: 'Fraunces', serif; font-size: 1.1rem; font-weight: 300;
    font-style: italic;
  }
  .footer-note { font-size: 10px; opacity: 0.35; letter-spacing: 0.08em; }

  /* ── ANIMATIONS ── */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(24px); }
    to   { opacity: 1; transform: translateY(0); }
  }
  .hero-left > * { animation: fadeUp 0.7s ease forwards; }
  .hero-left > *:nth-child(1) { animation-delay: 0.1s; opacity: 0; }
  .hero-left > *:nth-child(2) { animation-delay: 0.2s; opacity: 0; }
  .hero-left > *:nth-child(3) { animation-delay: 0.3s; opacity: 0; }
  .hero-left > *:nth-child(4) { animation-delay: 0.4s; opacity: 0; }
  .hero-left > *:nth-child(5) { animation-delay: 0.5s; opacity: 0; }

  /* ── RESPONSIVE ── */
  @media (max-width: 768px) {
    nav { padding: 1rem 1.5rem; }
    .nav-links { display: none; }
    .hero { grid-template-columns: 1fr; min-height: auto; }
    .hero-left { padding: 5rem 1.5rem 3rem; border-right: none; border-bottom: 1px solid var(--line); }
    .hero-right { padding: 3rem 1.5rem; }
    .section-inner { padding: 4rem 1.5rem; }
    #skills .section-inner, #education .section-inner {
      grid-template-columns: 1fr;
    }
    .timeline-item { grid-template-columns: 1fr; }
    .timeline-meta { margin-bottom: 0.5rem; }
    footer { flex-direction: column; gap: 1rem; text-align: center; }
  }
</style>
</head>
<body>

<nav>
  <a class="nav-logo" href="#">SA</a>
  <ul class="nav-links">
    <li><a href="#skills">Skills</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#education">Education</a></li>
  </ul>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-left">
    <p class="hero-tag">Portfolio</p>
    <h1>Solomon<br><em>Amognu</em></h1>
    <p class="hero-title">Senior Solution Architect</p>
	<p class="hero-title">+251921734577 | solalem2001@gmail.com</p>
    <p class="hero-summary">
      Over 15 years designing and building systems — from hardware-interfacing tools and government platforms to large-scale SaaS microservice migrations. Domain-driven, architecture-first, continuously learning.
    </p>
    <a class="hero-cta" href="#projects">View Projects</a>
  </div>
  <div class="hero-right">
    <div class="hero-stats">
      <div class="stat">
        <div class="stat-num">15+</div>
        <div class="stat-label">Years experience</div>
      </div>
      <div class="stat">
        <div class="stat-num">12+</div>
        <div class="stat-label">Major projects</div>
      </div>
      <div class="stat">
        <div class="stat-num">8</div>
        <div class="stat-label">Languages</div>
      </div>
      <div class="stat">
        <div class="stat-num">5+</div>
        <div class="stat-label">Employers / clients</div>
      </div>
    </div>
    <div class="hero-stack">
      <strong>Core Stack</strong>
      C# · Java · TypeScript · Python · .NET · Spring Boot · Angular · React · PostgreSQL · Azure · RabbitMQ · Docker · DDD · CQRS · Microservices
    </div>
  </div>
</section>

<!-- SKILLS -->
<section id="skills">
  <div class="section-inner">
    <div>
      <p class="section-label">Technical Expertise</p>
      <h2>A broad<br><em style="font-style:italic;color:var(--amber)">and deep</em><br>toolkit.</h2>
    </div>
    <div class="skills-grid">
      <div class="skill-group">
        <p class="skill-group-title">Languages</p>
        <div class="skill-tags">
          <span class="tag">C#</span><span class="tag">Java</span><span class="tag">TypeScript</span>
          <span class="tag">JavaScript</span><span class="tag">Python</span><span class="tag">C</span>
          <span class="tag">C++</span><span class="tag">Matlab</span><span class="tag">VB</span>
        </div>
      </div>
      <div class="skill-group">
        <p class="skill-group-title">Architecture & Design</p>
        <div class="skill-tags">
          <span class="tag">Domain Driven Design</span><span class="tag">Clean Architecture</span>
          <span class="tag">Microservices</span><span class="tag">CQRS</span>
          <span class="tag">C4 Modelling</span><span class="tag">Wardley Mapping</span>
          <span class="tag">Configuration Driven Design</span>
        </div>
      </div>
      <div class="skill-group">
        <p class="skill-group-title">Frameworks & Tools</p>
        <div class="skill-tags">
          <span class="tag">.NET / ASP.NET</span><span class="tag">Vert.x</span><span class="tag">Spring Boot</span>
          <span class="tag">Entity Framework</span><span class="tag">Angular</span><span class="tag">React</span>
          <span class="tag">Laravel</span><span class="tag">RabbitMQ</span><span class="tag">Redis</span>
          <span class="tag">Dapper</span>
        </div>
      </div>
      <div class="skill-group">
        <p class="skill-group-title">Databases & DevOps</p>
        <div class="skill-tags">
          <span class="tag">PostgreSQL</span><span class="tag">MS SQL Server</span><span class="tag">MongoDB</span>
          <span class="tag">Azure DevOps</span><span class="tag">GitHub Actions</span><span class="tag">Jenkins</span>
          <span class="tag">Azure Cloud</span><span class="tag">AWS</span>
        </div>
      </div>
      <div class="skill-group">
        <p class="skill-group-title">Management & Process</p>
        <div class="skill-tags">
          <span class="tag">Scrum</span><span class="tag">Agile</span><span class="tag">CI/CD</span>
          <span class="tag">Team Leadership</span><span class="tag">Process Design</span>
          <span class="tag">Continuous Delivery</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- EXPERIENCE -->
<section id="experience">
  <div class="section-inner">
    <p class="section-label">Work History</p>
    <h2>Where I've<br>built things.</h2>
    <div class="timeline">

      <div class="timeline-item">
        <div class="timeline-meta">
          <p class="tl-dates">Feb 2025 — Present</p>
          <p class="tl-company">Excellerent Solutions</p>
          <p class="tl-location">Addis Ababa, Ethiopia</p>
        </div>
        <div>
          <p class="tl-role">Senior Solution Architect</p>
          <p class="tl-desc">Designing and developing new features, building internal tools to investigate infrastructure issues, and supporting developers and infrastructure teams.</p>
        </div>
      </div>

      <div class="timeline-item">
        <div class="timeline-meta">
          <p class="tl-dates">Feb 2025 — Aug 2025</p>
          <p class="tl-company">ETech SC</p>
          <p class="tl-location">Addis Ababa, Ethiopia</p>
        </div>
        <div>
          <p class="tl-role">Solution Architect <span style="font-size:10px;opacity:0.5;">(Contract)</span></p>
          <p class="tl-desc">6-month project responsible for designing system integration and deployment architecture, organizing dev teams, and consulting on Scrum processes for a large ERP initiative.</p>
        </div>
      </div>

      <div class="timeline-item">
        <div class="timeline-meta">
          <p class="tl-dates">Aug 2021 — Feb 2025</p>
          <p class="tl-company">Excellerent Solutions</p>
          <p class="tl-location">Addis Ababa, Ethiopia</p>
        </div>
        <div>
          <p class="tl-role">Associate Solution Architect</p>
          <p class="tl-desc">Led multiple software development teams. Worked on design, implementation, and mentoring across enterprise-scale systems for international clients.</p>
        </div>
      </div>

      <div class="timeline-item">
        <div class="timeline-meta">
          <p class="tl-dates">Jun 2020 — Aug 2021</p>
          <p class="tl-company">Ministry of Innovation & Technology</p>
          <p class="tl-location">Addis Ababa, Ethiopia</p>
        </div>
        <div>
          <p class="tl-role">Open Data & Emerging Topics Project Manager</p>
          <p class="tl-desc">Created platforms for open data sharing (data.gov.et). Oversaw adoption of new topics and cultivated open data sharing culture across government agencies.</p>
        </div>
      </div>

      <div class="timeline-item">
        <div class="timeline-meta">
          <p class="tl-dates">Jan 2019 — Aug 2021</p>
          <p class="tl-company">Perago Systems</p>
          <p class="tl-location">Addis Ababa, Ethiopia</p>
        </div>
        <div>
          <p class="tl-role">Technical Consultant</p>
          <p class="tl-desc">Oversaw software development lifecycle processes, developed systems, and created architectural and design tools including a flagship reference architecture used across federal and local government.</p>
        </div>
      </div>

      <div class="timeline-item">
        <div class="timeline-meta">
          <p class="tl-dates">Jan 2010 — Jun 2020</p>
          <p class="tl-company">Information Network Security Agency</p>
          <p class="tl-location">Addis Ababa, Ethiopia</p>
        </div>
        <div>
          <p class="tl-role">Researcher and Developer</p>
          <p class="tl-desc">Designed, developed, and integrated hardware and software systems including UAV/Drone GCS, telemetry tools, and critical infrastructure systems over a decade-long tenure.</p>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- PROJECTS -->
<section id="projects">
  <div class="section-inner">
    <p class="section-label">Selected Projects</p>
    <h2>Things I've<br>shipped.</h2>
    <div class="projects-grid">

      <div class="project-card">
        <p class="project-client">ETech SC — 2025</p>
        <p class="project-name">ERP System (Ethio Engineering Group)</p>
        <p class="project-desc">Architecture and partial implementation of a 14-subsystem ERP built with Java + Angular, including Tenant Management and Auditing subsystems.</p>
        <span class="project-role">Architecture Consultant</span>
      </div>

      <div class="project-card">
        <p class="project-client">Hinda — 2025</p>
        <p class="project-name">Rewards Platform Service Integration</p>
        <p class="project-desc">Integrated new flight travel provider using OIDC auth, added retail merchant reward system, and automated DevOps workflows including PR approvals and release management.</p>
        <span class="project-role">Solution Architect</span>
      </div>

      <div class="project-card">
        <p class="project-client">Bluespark Technology — 2024</p>
        <p class="project-name">Sales Force Automation System</p>
        <p class="project-desc">Designed and developed a full MVP for sales force and route-to-market management using .NET backend and Blazor web frontend.</p>
        <span class="project-role">Creator</span>
      </div>

      <div class="project-card">
        <p class="project-client">Engage 2 Excel — 2022</p>
        <p class="project-name">Legacy to SaaS Microservice Migration</p>
        <p class="project-desc">Decomposed an employee recognition monolith serving hundreds of clients into a multitenant SaaS microservice platform. Created codegen tools, CDC-based sync, and reusable SDK packages.</p>
        <span class="project-role">Architect</span>
      </div>

      <div class="project-card">
        <p class="project-client">Agricultural Transformation Agency — 2021</p>
        <p class="project-name">BSC Automation System</p>
        <p class="project-desc">Automated strategic planning and scorecard execution monitoring. Achieved dramatic performance improvements — calculations that took 20+ minutes reduced to single-digit seconds.</p>
        <span class="project-role">Design Consultant & Developer</span>
      </div>

      <div class="project-card">
        <p class="project-client">Perago Systems — 2021</p>
        <p class="project-name">Business Intelligence Platform</p>
        <p class="project-desc">Built a generic BI system integrating OLAP Cube server with Angular frontend. Designed and implemented a separate ETL system to connect multiple data sources.</p>
        <span class="project-role">Design Consultant & Developer</span>
      </div>

      <div class="project-card">
        <p class="project-client">Public Procurement Agency — 2020</p>
        <p class="project-name">Electronic Government Procurement (egp.gov.et)</p>
        <p class="project-desc">Formalized implementation of a Microsoft Reference Architecture. Built code generators from DDD models and developed Catalog Management and Financial Assessment subsystems.</p>
        <span class="project-role">Design Consultant & Developer</span>
      </div>

      <div class="project-card">
        <p class="project-client">Perago Systems — 2019</p>
        <p class="project-name">Reference Architecture</p>
        <p class="project-desc">Created a canonical reference architecture based on Clean Architecture, CQRS, tactical DDD, and OpenAPI. Now used as the backbone across federal and local government platforms.</p>
        <span class="project-role">Architect & Trainer</span>
      </div>

      <div class="project-card">
        <p class="project-client">Ministry of Innovation — 2019</p>
        <p class="project-name">eService System (eservices.gov.et)</p>
        <p class="project-desc">Built knowledge base management, forum management, and a scheduling algorithm for appointment and queue management services powering multiple government agencies.</p>
        <span class="project-role">Development Contractor</span>
      </div>

    </div>
  </div>
</section>

<!-- NOTABLE OTHER PROJECTS -->
<section id="notable">
  <div class="section-inner">
    <p class="section-label">Also Notable</p>
    <h2>More work,<br>briefly.</h2>
    <div class="notable-list">
      <div class="notable-item">
        <span class="notable-name">Amora Ground Control Station (GCS)</span>
        <span class="notable-tag-label">UAV / Drone systems, INSA</span>
      </div>
      <div class="notable-item">
        <span class="notable-name">Solo SW Design & Modelling Tool</span>
        <span class="notable-tag-label">DDD code generator, personal project</span>
      </div>
      <div class="notable-item">
        <span class="notable-name">Common Data Exchange Platform</span>
        <span class="notable-tag-label">System integration middleware, Perago</span>
      </div>
      <div class="notable-item">
        <span class="notable-name">DoneDeal SFA</span>
        <span class="notable-tag-label">Multitenant sales rep tracker</span>
      </div>
      <div class="notable-item">
        <span class="notable-name">Green Legacy / Green Community</span>
        <span class="notable-tag-label">National tree-planting monitoring platforms</span>
      </div>
      <div class="notable-item">
        <span class="notable-name">Telemetry Parser & Router</span>
        <span class="notable-tag-label">Serial / UDP / TCP telemetry desktop apps</span>
      </div>
      <div class="notable-item">
        <span class="notable-name">Soccer Stat Tracker & Video Multiplexer</span>
        <span class="notable-tag-label">DirectX-powered side projects</span>
      </div>
    </div>
  </div>
</section>

<!-- EDUCATION -->
<section id="education">
  <div class="section-inner">
    <div>
      <p class="section-label">Education</p>
      <h2>Where it<br>started.</h2>
    </div>
    <div>
      <div class="edu-block">
        <p class="edu-degree">Bachelor of Science<br>in Electrical Engineering</p>
        <p class="edu-school">Bahir Dar University — Engineering Faculty</p>
        <p class="edu-date">September 2005 — July 2009 · Bahir Dar, Ethiopia</p>
      </div>
    </div>
  </div>
</section>

<footer>
  <span class="footer-name">Solomon Amognu Getahun | Senior Solution Architect </span>
  <span class="footer-note"> +251921734577 | solalem2001@gmail.com | Addis Ababa, Ethiopia</span>
</footer>

</body>
</html>

{{< /section-container >}}
