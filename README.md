<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Teja Achanta · Data Analyst Portfolio</title>
  <meta name="description" content="Portfolio of Teja Achanta — Data Analyst with 5+ years of experience in finance, banking, and insurance. Python, SQL, Power BI, Tableau, Looker, Snowflake, BigQuery." />
  <meta name="theme-color" content="#0ea5e9" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0b1020;          /* deep ink */
      --panel:#0f172a;       /* slate-900 */
      --muted:#94a3b8;       /* slate-400 */
      --text:#e2e8f0;        /* slate-200 */
      --brand:#22d3ee;       /* cyan-400 */
      --brand-2:#38bdf8;     /* sky-400 */
      --chip:#1f2937;        /* gray-800 */
      --card:#0b1224;        /* blend */
      --ring: rgba(56,189,248,.35);
      --shadow: 0 10px 30px rgba(2,6,23,.45);
    }
    *{box-sizing:border-box}
    html,body{margin:0;height:100%;background:linear-gradient(180deg,var(--bg),#060913);color:var(--text);font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,Arial,"Noto Sans",sans-serif;}
    a{color:inherit}
    .container{max-width:1100px;margin:0 auto;padding:28px}
    header{position:sticky;top:0;backdrop-filter:saturate(160%) blur(8px);background:linear-gradient(180deg,rgba(2,6,23,.7),rgba(2,6,23,.2));border-bottom:1px solid rgba(148,163,184,.12);z-index:50}
    .nav{display:flex;align-items:center;justify-content:space-between;gap:16px}
    .brand{display:flex;align-items:center;gap:12px;font-weight:700;letter-spacing:.3px}
    .badge{display:inline-flex;align-items:center;gap:8px;background:linear-gradient(120deg,var(--brand),var(--brand-2));color:#0b1020;border-radius:999px;padding:8px 14px;font-weight:700;box-shadow:var(--shadow)}
    .links a{margin:0 10px;text-decoration:none;color:var(--muted)}
    .links a:hover{color:white}
    .btn{display:inline-flex;align-items:center;gap:10px;border:1px solid rgba(56,189,248,.45);color:#e0f2fe;background:rgba(2,132,199,.15);padding:12px 16px;border-radius:14px;text-decoration:none}
    .btn:hover{background:rgba(56,189,248,.2)}

    /* hero */
    .hero{display:grid;grid-template-columns:1.3fr .7fr;gap:28px;align-items:center;padding-top:28px}
    .card{background:linear-gradient(180deg,var(--panel),var(--card));border:1px solid rgba(148,163,184,.12);border-radius:22px;box-shadow:var(--shadow)}
    .hero .left{padding:32px}
    .title{font-size:clamp(30px,5vw,46px);line-height:1.1;margin:8px 0 12px;font-weight:800}
    .subtitle{color:var(--muted);font-size:clamp(14px,2vw,16px)}
    .chiprow{display:flex;flex-wrap:wrap;gap:10px;margin-top:14px}
    .chip{background:var(--chip);border:1px solid rgba(148,163,184,.18);padding:8px 12px;border-radius:999px;font-size:13px;color:#cbd5e1}
    .hero .right{padding:24px;display:grid;gap:12px}
    .kpi{padding:18px;border-radius:18px;background:linear-gradient(180deg,#0c1328,#0a162f);border:1px solid rgba(148,163,184,.14)}
    .kpi h3{margin:0 0 6px;font-size:28px}
    .kpi p{margin:0;color:var(--muted);font-size:14px}

    section{margin-top:34px}
    h2{font-size:24px;margin:0 0 14px}

    /* grid lists */
    .grid{display:grid;gap:14px}
    .grid.cols-3{grid-template-columns:repeat(auto-fit,minmax(240px,1fr))}
    .grid.cols-2{grid-template-columns:repeat(auto-fit,minmax(300px,1fr))}
    .tile{padding:18px;border-radius:18px;background:linear-gradient(180deg,#0c1226,#0b152c);border:1px solid rgba(148,163,184,.12)}
    .tile h3{margin:0 0 6px;font-size:18px}
    .tile p{margin:0;color:var(--muted);font-size:14px}
    .list{display:flex;flex-direction:column;gap:10px;margin-top:10px}
    .list li{color:#cbd5e1}

    /* experience */
    .xp{display:grid;gap:14px}
    .role{display:grid;gap:8px;padding:18px;border-radius:18px;background:linear-gradient(180deg,#0b1328,#0a152b);border:1px solid rgba(148,163,184,.12)}
    .role .meta{display:flex;flex-wrap:wrap;gap:10px;color:var(--muted);font-size:14px}
    .role ul{margin:6px 0 0 18px}
    .role li{margin:6px 0;color:#cbd5e1}

    .footer{margin:34px 0 20px;color:var(--muted);text-align:center}

    /* responsive */
    @media (max-width: 880px){
      .hero{grid-template-columns:1fr}
    }
  </style>
  <script>
    // smooth nav
    addEventListener('DOMContentLoaded', () => {
      document.querySelectorAll('a[href^="#"]').forEach(a=>{
        a.addEventListener('click', e=>{const id=a.getAttribute('href'); if(id.length>1){e.preventDefault(); document.querySelector(id)?.scrollIntoView({behavior:'smooth', block:'start'});}})
      })
    })
  </script>
  <!-- Schema.org Person -->
  <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Person",
      "name": "Teja Achanta",
      "jobTitle": "Data Analyst",
      "url": "https://your-github-username.github.io/",
      "email": "mailto:teja.a.work.950@gmail.com",
      "telephone": "+1-940-969-1711",
      "address": {"@type":"PostalAddress","addressLocality":"Denton","addressRegion":"TX","addressCountry":"US"},
      "sameAs": [
        "https://www.linkedin.com/in/YOUR-LINKEDIN-HANDLE",
        "https://github.com/YOUR-GITHUB-USERNAME"
      ]
    }
  </script>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="brand">
        <span class="badge">TA</span>
        <span>Teja Achanta</span>
      </div>
      <nav class="links" aria-label="Primary">
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#experience">Experience</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
      </nav>
      <a class="btn" href="#contact" aria-label="Contact Teja">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M22 12h-4"/><path d="M2 12h4"/><path d="M12 2v4"/><path d="M12 22v-4"/><circle cx="12" cy="12" r="7"/></svg>
        Hire Me
      </a>
    </div>
  </header>

  <main class="container">
    <!-- HERO -->
    <section class="hero">
      <div class="left card">
        <div class="badge" style="margin-bottom:12px">Data Analyst · Finance · Banking · Insurance</div>
        <h1 class="title">Hi, I'm Teja — I turn <span style="background:linear-gradient(120deg,var(--brand),var(--brand-2));-webkit-background-clip:text;background-clip:text;color:transparent">complex data</span> into business impact.</h1>
        <p class="subtitle">5+ years building dashboards, analytics, and ETL across Capital Group, Axis Bank, and Bajaj Allianz. Python · SQL · Power BI · Tableau · Looker · Snowflake · BigQuery.</p>
        <div class="chiprow" aria-label="Highlights">
          <span class="chip">Automated 75% of reporting (Python + SQL)</span>
          <span class="chip">5M+ rows analyzed (BigQuery/Postgres)</span>
          <span class="chip">98%+ data integrity (Great Expectations)</span>
          <span class="chip">Regulatory & governance ready (SOX/GDPR)</span>
        </div>
      </div>
      <div class="right">
        <div class="kpi">
          <h3>40% faster</h3>
          <p>Report delivery timelines after Python automation at Capital Group.</p>
        </div>
        <div class="kpi">
          <h3>30% ↑ engagement</h3>
          <p>Power BI investment dashboards used by stakeholders.</p>
        </div>
        <div class="kpi">
          <h3>22% ↑ conversions</h3>
          <p>R-based banking customer segmentation at Axis Bank.</p>
        </div>
      </div>
    </section>

    <!-- ABOUT -->
    <section id="about" class="card" style="padding:24px">
      <h2>About</h2>
      <p class="subtitle">I specialize in data wrangling, statistical modeling (T‑Test, ANOVA, regression), and building scalable analytics. I’ve shipped interactive reports in Power BI, Tableau, and Looker; built pipelines in Informatica, Python, and Airflow; and modeled data in Snowflake and BigQuery. I care about reliable data, reproducible analysis, and clean, user‑friendly visuals.</p>
      <ul class="list" style="margin-top:12px">
        <li>Located in Denton, TX · Open to relocation</li>
        <li>Hands‑on with REST APIs (Postman) and data quality frameworks (Great Expectations, Talend)</li>
        <li>Comfortable across cloud stacks: AWS · Azure · GCP</li>
      </ul>
    </section>

    <!-- SKILLS -->
    <section id="skills">
      <h2>Skills</h2>
      <div class="grid cols-3">
        <div class="tile">
          <h3>Programming</h3>
          <p>Python, SQL, R, SAS, MATLAB</p>
        </div>
        <div class="tile">
          <h3>Visualization</h3>
          <p>Power BI (DAX), Tableau, Looker, Google Data Studio, Excel Dashboards, Matplotlib, Seaborn</p>
        </div>
        <div class="tile">
          <h3>Databases</h3>
          <p>MySQL, PostgreSQL, MS SQL Server, Google BigQuery</p>
        </div>
        <div class="tile">
          <h3>Cloud & DWH</h3>
          <p>Snowflake, Redshift, AWS, Azure, GCP, Docker, Kubernetes, Serverless</p>
        </div>
        <div class="tile">
          <h3>ETL & Big Data</h3>
          <p>Informatica PowerCenter, Alteryx, Trifacta, SSIS, Airflow, Spark, Python ETL</p>
        </div>
        <div class="tile">
          <h3>Governance</h3>
          <p>Great Expectations, Talend Data Quality, Informatica DQ, Data Masking, Access Controls, SOX/GDPR</p>
        </div>
      </div>
    </section>

    <!-- EXPERIENCE -->
    <section id="experience">
      <h2>Experience</h2>
      <div class="xp">
        <article class="role">
          <div class="meta"><strong>Data Analyst</strong> · Capital Group · Los Angeles, CA <span>· Dec 2023 – Present</span></div>
          <ul>
            <li>Automated <strong>75%</strong> of financial reporting with Python + SQL, cutting delivery times by <strong>40%</strong>.</li>
            <li>Built ETL with <strong>Informatica</strong> + Python into <strong>Snowflake</strong>; optimized models for 5M+ records.</li>
            <li>Implemented data governance (access controls, masking, audit logs) to meet <strong>SOX/GDPR</strong>.</li>
            <li>Enhanced <strong>Power BI</strong> & <strong>Tableau</strong> dashboards for investment performance and risk/return.</li>
            <li>Used Python/R for regression, hypothesis tests, T‑Tests; ran A/B tests to improve ROI.</li>
            <li>Data quality checks with <strong>Great Expectations</strong> achieved <strong>98%+</strong> integrity.</li>
          </ul>
        </article>
        <article class="role">
          <div class="meta"><strong>Data Analyst</strong> · Axis Bank · India <span>· Mar 2022 – Dec 2022</span></div>
          <ul>
            <li>R‑based customer segmentation drove <strong>+22%</strong> cross‑sell/upsell in retail banking.</li>
            <li>ETL via <strong>Informatica</strong> & <strong>Alteryx</strong> into EDW; automated Power BI & Excel reports.</li>
            <li>Strengthened governance with <strong>Informatica DQ</strong> & <strong>Talend</strong>; supported Snowflake migration.</li>
            <li>Analyzed MS SQL/MySQL data for fraud & behavior insights; built exec Tableau dashboards.</li>
          </ul>
        </article>
        <article class="role">
          <div class="meta"><strong>Data Analyst</strong> · Bajaj Allianz Life Insurance · India <span>· Jun 2019 – Feb 2022</span></div>
          <ul>
            <li>Claims tracking dashboards in Excel improved SLA monitoring by <strong>35%</strong>.</li>
            <li>Supported Snowflake DWH creation and Informatica‑based pipelines for policy & claims data.</li>
            <li>Performed EDA with Python (Pandas/Seaborn); published Tableau reports on complaint trends.</li>
          </ul>
        </article>
      </div>
    </section>

    <!-- PROJECTS / CASE STUDIES -->
    <section id="projects">
      <h2>Projects & Case Studies</h2>
      <div class="grid cols-2">
        <div class="tile">
          <h3>Investment KPI Suite (Power BI)</h3>
          <p>Interactive dashboards tracking fund performance, risk/return, and quarterly KPIs. Role: data modeling in Snowflake, DAX measures, stakeholder reviews.</p>
          <ul class="list">
            <li>Outcome: 30% increase in stakeholder engagement</li>
            <li>Stack: Power BI, Snowflake, Python</li>
          </ul>
        </div>
        <div class="tile">
          <h3>Automated Reporting (Python + SQL)</h3>
          <p>Refactored manual Excel workflows into reproducible Python notebooks and scheduled jobs.</p>
          <ul class="list">
            <li>Outcome: 40% faster reporting cadence</li>
            <li>Stack: Python (Pandas), PostgreSQL/BigQuery</li>
          </ul>
        </div>
        <div class="tile">
          <h3>Banking Segmentation (R)</h3>
          <p>Customer segmentation for targeted offers across retail portfolios.</p>
          <ul class="list">
            <li>Outcome: +22% cross‑sell/upsell</li>
            <li>Stack: R, SQL, Tableau</li>
          </ul>
        </div>
        <div class="tile">
          <h3>Data Quality Framework</h3>
          <p>Implemented validation checks for board‑level reporting using Great Expectations.</p>
          <ul class="list">
            <li>Outcome: 98%+ integrity in quarterly reporting</li>
            <li>Stack: Great Expectations, Snowflake</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact" class="card" style="padding:24px">
      <h2>Contact</h2>
      <p class="subtitle">Let’s talk about analytics, dashboards, or data engineering opportunities.</p>
      <div class="grid cols-3">
        <div class="tile">
          <h3>Email</h3>
          <p><a href="mailto:teja.a.work.950@gmail.com">teja.a.work.950@gmail.com</a></p>
        </div>
        <div class="tile">
          <h3>Phone</h3>
          <p><a href="tel:+19409691711">(940) 969-1711</a></p>
        </div>
        <div class="tile">
          <h3>LinkedIn</h3>
          <p><a href="https://www.linkedin.com/in/YOUR-LINKEDIN-HANDLE" target="_blank" rel="noopener">linkedin.com/in/YOUR‑LINKEDIN‑HANDLE</a></p>
        </div>
      </div>
      <div style="margin-top:14px;display:flex;gap:10px;flex-wrap:wrap">
        <a class="btn" href="resume.pdf" target="_blank" rel="noopener">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6"/></svg>
          Download Résumé
        </a>
        <a class="btn" href="https://github.com/YOUR-GITHUB-USERNAME" target="_blank" rel="noopener">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M12 1C5.925 1 1 5.925 1 12a10.998 10.998 0 0 0 7.5 10.46c.55.1.75-.24.75-.53 0-.26-.01-1.12-.02-2.03-3.05.66-3.7-1.3-3.7-1.3-.5-1.26-1.22-1.6-1.22-1.6-.99-.68.08-.67.08-.67 1.1.08 1.68 1.12 1.68 1.12.98 1.67 2.58 1.19 3.21.9.1-.71.38-1.19.69-1.46-2.43-.28-4.99-1.22-4.99-5.43 0-1.2.43-2.18 1.12-2.95-.11-.28-.49-1.4.1-2.91 0 0 .92-.29 3.02 1.12A10.52 10.52 0 0 1 12 6.84c.93.01 1.86.13 2.73.37 2.1-1.41 3.02-1.12 3.02-1.12.59 1.51.21 2.63.1 2.91.69.77 1.11 1.75 1.11 2.95 0 4.22-2.57 5.14-5.01 5.41.39.34.74 1.02.74 2.06 0 1.49-.01 2.69-.01 3.06 0 .28.2.62.76.51A11 11 0 0 0 23 12c0-6.075-4.925-11-11-11z"/></svg>
          GitHub
        </a>
      </div>
    </section>

    <p class="footer">© <span id="y"></span> Teja Achanta · Built with semantic HTML & a dash of CSS ✨</p>
  </main>

  <script>
    document.getElementById('y').textContent = new Date().getFullYear();
  </script>
</body>
</html>
