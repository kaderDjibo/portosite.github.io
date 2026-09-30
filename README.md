#  Portfolio for ,Data Science, Machine learning, AI
Html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Abdoul Kader Djibo · Data Analyst & AI/ML Enthusiast</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="description" content="Portfolio of Abdoul Kader Djibo, entry-level Data Analyst and AI/ML enthusiast focusing on Python, data analytics, and machine learning." />
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet" />
  <style>
    :root {
      --bg: #050816;
      --bg-alt: #0b1020;
      --card: #111827;
      --accent: #22c55e;
      --accent-soft: rgba(34, 197, 94, 0.12);
      --accent-2: #3b82f6;
      --text: #e5e7eb;
      --muted: #9ca3af;
      --border: #1f2937;
      --danger: #f97373;
      --radius-lg: 16px;
      --radius-md: 10px;
      --radius-pill: 999px;
      --shadow-soft: 0 20px 40px rgba(0,0,0,0.4);
      --shadow-subtle: 0 10px 30px rgba(0,0,0,0.3);
      --transition-fast: 0.2s ease-out;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: "Poppins", system-ui, -apple-system, BlinkMacSystemFont, sans-serif;
      background: radial-gradient(circle at top, #1f2937 0, #020617 45%, #000 80%);
      color: var(--text);
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
      scroll-behavior: smooth;
    }

    a { color: inherit; text-decoration: none; }
    img { max-width: 100%; display: block; }

    ::selection {
      background: var(--accent);
      color: #020617;
    }

    /* TOP NAVBAR */

    .navbar {
      position: sticky;
      top: 0;
      z-index: 50;
      backdrop-filter: blur(18px);
      background: rgba(2, 6, 23, 0.92);
      border-bottom: 1px solid rgba(55, 65, 81, 0.9);
    }

    .navbar-inner {
      max-width: 1120px;
      margin: 0 auto;
      padding: 10px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 12px;
    }

    .nav-brand {
      font-size: 0.95rem;
      font-weight: 600;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      color: var(--muted);
    }

    .nav-links {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      font-size: 0.82rem;
    }

    .nav-link {
      padding: 4px 10px;
      border-radius: var(--radius-pill);
      border: 1px solid transparent;
      color: var(--muted);
      cursor: pointer;
      transition: background var(--transition-fast), color var(--transition-fast), border-color var(--transition-fast), transform var(--transition-fast);
    }

    .nav-link:hover {
      border-color: var(--accent);
      color: var(--accent);
      background: rgba(15, 23, 42, 0.9);
      transform: translateY(-1px);
    }

    .nav-link-primary {
      border-color: rgba(55, 65, 81, 0.9);
      background: rgba(15, 23, 42, 0.95);
      color: #f9fafb;
    }

    .nav-link-primary:hover {
      border-color: var(--accent);
      color: var(--accent);
    }

    @media (max-width: 700px) {
      .nav-brand {
        font-size: 0.8rem;
      }
      .nav-links {
        font-size: 0.78rem;
      }
    }

    /* PAGE LAYOUT */

    .page {
      max-width: 1120px;
      margin: 0 auto;
      padding: 24px 20px 64px;
      display: grid;
      grid-template-columns: minmax(0, 3fr) minmax(0, 2.1fr);
      gap: 32px;
    }

    @media (max-width: 900px) {
      .page {
        grid-template-columns: minmax(0, 1fr);
        padding-top: 16px;
      }
    }

    /* HERO */

    .hero-card {
      background: radial-gradient(circle at top left, rgba(34,197,94,0.18), transparent 45%),
                  radial-gradient(circle at top right, rgba(59,130,246,0.18), transparent 45%),
                  linear-gradient(135deg, #020617, #020617 40%, #020617);
      border-radius: 24px;
      padding: 28px 28px 24px;
      border: 1px solid rgba(148,163,184,0.22);
      box-shadow: var(--shadow-soft);
      position: relative;
      overflow: hidden;
    }

    .hero-header {
      display: flex;
      align-items: center;
      gap: 18px;
    }

    .avatar {
      width: 80px;
      height: 80px;
      border-radius: 24px;
      background: linear-gradient(135deg, #22c55e, #3b82f6);
      padding: 3px;
      box-shadow: 0 12px 30px rgba(34,197,94,0.5);
      flex-shrink: 0;
    }

    .avatar-inner {
      width: 100%;
      height: 100%;
      border-radius: 20px;
      background: #020617 url("YOUR_PHOTO_URL_HERE") center/cover no-repeat;
    }

    .hero-text h1 {
      font-size: clamp(1.9rem, 3vw, 2.4rem);
      font-weight: 700;
      letter-spacing: 0.02em;
      margin-bottom: 4px;
    }

    .hero-role {
      font-weight: 500;
      font-size: 0.95rem;
      color: var(--accent);
      text-transform: uppercase;
      letter-spacing: 0.18em;
    }

    .hero-subtitle {
      font-size: 0.9rem;
      color: var(--muted);
      margin-top: 8px;
    }

    .hero-badges {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-top: 14px;
    }

    .badge {
      border-radius: var(--radius-pill);
      padding: 4px 10px;
      border: 1px solid rgba(148,163,184,0.4);
      font-size: 0.75rem;
      color: var(--muted);
      display: inline-flex;
      align-items: center;
      gap: 6px;
      background: rgba(15,23,42,0.9);
      backdrop-filter: blur(16px);
    }

    .badge-dot {
      width: 7px;
      height: 7px;
      border-radius: 999px;
      background: var(--accent);
      box-shadow: 0 0 0 5px rgba(34,197,94,0.25);
    }

    .hero-actions {
      margin-top: 20px;
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .btn {
      border-radius: var(--radius-pill);
      padding: 9px 18px;
      border: 1px solid transparent;
      font-size: 0.87rem;
      font-weight: 500;
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      transition: transform var(--transition-fast), box-shadow var(--transition-fast), background var(--transition-fast), border-color var(--transition-fast), color var(--transition-fast);
      background: none;
      color: inherit;
    }

    .btn-primary {
      background: linear-gradient(135deg, #22c55e, #16a34a);
      color: #020617;
      box-shadow: 0 14px 30px rgba(22,163,74,0.55);
    }

    .btn-primary:hover {
      transform: translateY(-1px);
      box-shadow: 0 20px 40px rgba(22,163,74,0.65);
    }

    .btn-ghost {
      border-color: rgba(148,163,184,0.5);
      background: rgba(15,23,42,0.75);
      backdrop-filter: blur(16px);
    }

    .btn-ghost:hover {
      border-color: var(--accent);
      color: var(--accent);
      transform: translateY(-1px);
      box-shadow: 0 12px 30px rgba(15,23,42,0.8);
    }

    .hero-metrics {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 10px;
      margin-top: 24px;
      font-size: 0.8rem;
    }

    .metric {
      border-radius: 14px;
      background: rgba(15,23,42,0.86);
      border: 1px solid rgba(148,163,184,0.35);
      padding: 8px 10px;
    }

    .metric-label {
      color: var(--muted);
      font-size: 0.7rem;
      margin-bottom: 4px;
    }

    .metric-value {
      font-weight: 600;
      font-size: 0.95rem;
    }

    .hero-scroll {
      margin-top: 26px;
      font-size: 0.8rem;
      color: var(--muted);
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .hero-scroll span {
      width: 28px;
      height: 28px;
      border-radius: 999px;
      border: 1px solid rgba(148,163,184,0.6);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 0.7rem;
    }

    /* SECTIONS */

    .sections {
      margin-top: 28px;
      display: flex;
      flex-direction: column;
      gap: 26px;
    }

    .section {
      padding: 20px 18px;
      border-radius: 18px;
      background: rgba(15,23,42,0.9);
      border: 1px solid rgba(55,65,81,0.8);
      box-shadow: var(--shadow-subtle);
    }

    .section-header {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      gap: 10px;
      margin-bottom: 14px;
    }

    .section-title {
      font-size: 1rem;
      font-weight: 600;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--muted);
    }

    .section-kicker {
      font-size: 0.75rem;
      color: var(--accent-2);
    }

    .section-body {
      font-size: 0.88rem;
      color: var(--text);
    }

    .section-body p + p {
      margin-top: 8px;
    }

    .section-body strong {
      color: #f9fafb;
    }

    .section-footer {
      margin-top: 14px;
      display: flex;
      justify-content: flex-end;
    }

    .next-link {
      font-size: 0.8rem;
      color: var(--accent-2);
      display: inline-flex;
      align-items: center;
      gap: 6px;
      cursor: pointer;
    }

    .next-link span {
      font-size: 0.85rem;
    }

    /* TIMELINE */

    .timeline {
      margin-top: 10px;
      border-left: 1px solid rgba(55,65,81,0.8);
      padding-left: 16px;
      display: flex;
      flex-direction: column;
      gap: 18px;
    }

    .timeline-item {
      position: relative;
    }

    .timeline-item::before {
      content: "";
      position: absolute;
      left: -17px;
      top: 4px;
      width: 10px;
      height: 10px;
      border-radius: 999px;
      background: var(--accent);
      box-shadow: 0 0 0 4px rgba(34,197,94,0.25);
    }

    .timeline-role {
      font-weight: 500;
      font-size: 0.9rem;
    }

    .timeline-meta {
      font-size: 0.78rem;
      color: var(--muted);
      margin-top: 2px;
    }

    .timeline-desc {
      margin-top: 6px;
      font-size: 0.84rem;
      color: var(--text);
    }

    /* PROJECTS */

    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
      gap: 14px;
      margin-top: 8px;
    }

    .project-card {
      border-radius: 16px;
      background: radial-gradient(circle at top left, rgba(34,197,94,0.08), transparent 55%),
                  radial-gradient(circle at bottom right, rgba(59,130,246,0.08), transparent 55%),
                  #020617;
      border: 1px solid rgba(55,65,81,0.9);
      padding: 12px 12px 10px;
      transition: transform var(--transition-fast), box-shadow var(--transition-fast), border-color var(--transition-fast), background var(--transition-fast);
      cursor: pointer;
    }

    .project-card:hover {
      transform: translateY(-3px);
      box-shadow: 0 16px 35px rgba(15,23,42,0.95);
      border-color: var(--accent);
    }

    .project-tag {
      display: inline-flex;
      align-items: center;
      gap: 4px;
      padding: 2px 8px;
      border-radius: var(--radius-pill);
      background: rgba(15,23,42,0.9);
      border: 1px solid rgba(55,65,81,0.8);
      font-size: 0.7rem;
      color: var(--muted);
      margin-bottom: 6px;
    }

    .project-title {
      font-size: 0.92rem;
      font-weight: 600;
      margin-bottom: 4px;
    }

    .project-desc {
      font-size: 0.8rem;
      color: var(--muted);
      margin-bottom: 6px;
    }

    .project-meta {
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: 0.75rem;
      color: var(--muted);
    }

    .project-stack {
      font-size: 0.72rem;
      color: var(--muted);
    }

    .project-link {
      color: var(--accent);
      font-weight: 500;
      font-size: 0.75rem;
    }

    /* SKILLS */

    .skill-groups {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 10px 16px;
      margin-top: 8px;
    }

    .skill-group-title {
      font-size: 0.8rem;
      font-weight: 600;
      color: var(--muted);
      text-transform: uppercase;
      letter-spacing: 0.12em;
      margin-bottom: 6px;
    }

    .chips {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
    }

    .chip {
      border-radius: var(--radius-pill);
      padding: 3px 9px;
      border: 1px solid rgba(55,65,81,0.9);
      font-size: 0.74rem;
      color: var(--text);
      background: rgba(15,23,42,0.9);
    }

    .chip.strong {
      border-color: var(--accent);
      background: rgba(34,197,94,0.1);
    }

    /* SIDEBAR */

    .sidebar {
      display: flex;
      flex-direction: column;
      gap: 18px;
    }

    .card {
      border-radius: 18px;
      background: rgba(15,23,42,0.94);
      border: 1px solid rgba(55,65,81,0.9);
      padding: 16px 16px 14px;
      box-shadow: var(--shadow-subtle);
      font-size: 0.84rem;
    }

    .card-header {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      margin-bottom: 8px;
    }

    .card-title {
      font-size: 0.9rem;
      font-weight: 600;
      color: var(--muted);
      text-transform: uppercase;
      letter-spacing: 0.16em;
    }

    .card-pill {
      font-size: 0.7rem;
      border-radius: var(--radius-pill);
      padding: 2px 8px;
      border: 1px solid rgba(55,65,81,0.9);
      color: var(--muted);
    }

    .contact-list {
      display: flex;
      flex-direction: column;
      gap: 8px;
      margin-top: 6px;
    }

    .contact-item {
      display: flex;
      flex-direction: column;
      gap: 2px;
    }

    .contact-label {
      font-size: 0.74rem;
      color: var(--muted);
      text-transform: uppercase;
      letter-spacing: 0.14em;
    }

    .contact-value {
      font-size: 0.88rem;
      word-break: break-all;
    }

    .social-links {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-top: 8px;
    }

    .social-chip {
      border-radius: var(--radius-pill);
      padding: 4px 10px;
      border: 1px solid rgba(55,65,81,0.9);
      font-size: 0.78rem;
      color: var(--muted);
      cursor: pointer;
      transition: background var(--transition-fast), color var(--transition-fast), border-color var(--transition-fast), transform var(--transition-fast);
    }

    .social-chip:hover {
      border-color: var(--accent-2);
      color: #e5f2ff;
      background: rgba(37,99,235,0.2);
      transform: translateY(-1px);
    }

    .blog-list {
      display: flex;
      flex-direction: column;
      gap: 10px;
      margin-top: 6px;
    }

    .blog-item-title {
      font-size: 0.86rem;
      font-weight: 500;
    }

    .blog-meta {
      font-size: 0.75rem;
      color: var(--muted);
      margin-top: 2px;
    }

    .email-highlight {
      margin-top: 8px;
      font-size: 0.8rem;
      padding: 8px 10px;
      border-radius: 12px;
      background: rgba(34,197,94,0.08);
      border: 1px dashed rgba(34,197,94,0.6);
      color: var(--accent);
      word-break: break-all;
    }

    .footnote {
      font-size: 0.7rem;
      color: var(--muted);
      margin-top: 6px;
    }
  </style>
</head>
<body>

  <!-- TOP NAVBAR -->
  <header class="navbar">
    <div class="navbar-inner">
      <div class="nav-brand">DJIBO KADER · DATA ANALYTICS &amp; ML</div>
      <nav class="nav-links">
        <a href="#top" class="nav-link nav-link-primary">Home</a>
        <a href="#about" class="nav-link">About</a>
        <a href="#skills" class="nav-link">Skills</a>
        <a href="#projects" class="nav-link">Projects</a>
        <a href="#contact" class="nav-link">Contact</a>
      </nav>
    </div>
  </header>

  <main class="page" id="top">
    <!-- LEFT COLUMN -->
    <section>
      <!-- HERO -->
      <header class="hero-card">
        <div class="hero-header">
          <div class="avatar">
            <div class="avatar-inner"></div>
          </div>
          <div class="hero-text">
            <div class="hero-role">Entry Level Data Analyst · AI &amp; ML Enthusiast</div>
            <h1>Abdoul Kader Djibo</h1>
            <p class="hero-subtitle">
              I turn raw data into clean insights and simple interfaces using Python, SQL, and machine learning – with a strong focus on clear communication and reproducible analysis.
            </p>
          </div>
        </div>

        <div class="hero-badges">
          <div class="badge">
            <span class="badge-dot"></span>
            Open to Data Analyst &amp; AI/ML roles
          </div>
          <div class="badge">BCA · University of Mysore (Jun 2026)</div>
          <div class="badge">Python · pandas · scikit learn · Streamlit</div>
        </div>

        <div class="hero-actions">
          <a href="#projects" class="btn btn-primary">
            View Data Projects →
          </a>
          <a href="#about" class="btn btn-ghost">
            Next: About me →
          </a>
        </div>

        <div class="hero-metrics">
          <div class="metric">
            <div class="metric-label">Core project</div>
            <div class="metric-value">Heart Disease ML App</div>
          </div>
          <div class="metric">
            <div class="metric-label">Internship</div>
            <div class="metric-value">Cognifyz · 2026</div>
          </div>
          <div class="metric">
            <div class="metric-label">Tech stack</div>
            <div class="metric-value">Python · SQL · ML</div>
          </div>
        </div>

        <div class="hero-scroll">
          <span>↓</span>
          Scroll or use the menu to move through sections
        </div>
      </header>

      <!-- MAIN SECTIONS -->
      <div class="sections">
        <!-- ABOUT -->
        <section class="section" id="about">
          <div class="section-header">
            <h2 class="section-title">About</h2>
            <div class="section-kicker">From BCA to applied data &amp; AI</div>
          </div>
          <div class="section-body">
            <p>
              I’m Djibo Kader, an entry level <strong>Data Analyst and AI/ML enthusiast</strong> currently finishing my BCA at the University of Mysore.
              I enjoy taking messy data and turning it into something clear and useful – whether that’s a simple chart, a clean notebook,
              or a small app someone can actually use.
            </p>
            <p>
              Most of my work so far has been in <strong>Python</strong> with <strong>pandas, NumPy, scikit learn, and Streamlit</strong>.
              I’ve built an AI driven heart disease diagnosis app and completed a software development internship at Cognifyz Technologies,
              which taught me how to write cleaner code, debug faster, and think about structure and readability.
            </p>
            <p>
              I’m now looking for opportunities as a <strong>Data Analyst or junior ML engineer</strong> where I can keep learning,
              work with real world datasets, and contribute to a team that cares about both technical quality and clear communication.
            </p>
          </div>
          <div class="section-footer">
            <a href="#education" class="next-link">Next: Education &amp; Experience <span>→</span></a>
          </div>
        </section>

        <!-- EDUCATION & EXPERIENCE -->
        <section class="section" id="education">
          <div class="section-header">
            <h2 class="section-title">Education &amp; Experience</h2>
            <div class="section-kicker">How I built my foundation</div>
          </div>
          <div class="section-body">
            <div class="timeline">
              <div class="timeline-item">
                <div class="timeline-role">Bachelor of Computer Applications (BCA)</div>
                <div class="timeline-meta">University of Mysore – Vidhyaashram First Grade College, Mysore · Expected Jun 2026</div>
                <p class="timeline-desc">
                  Relevant coursework: <strong>Data Structures and Algorithms, Database Management Systems, Web Technologies, Operating Systems, Computer Networks, Software Engineering, Data Analytics, Machine Learning (project based), Statistics for Computing.</strong>
                </p>
              </div>

              <div class="timeline-item">
                <div class="timeline-role">Software Development Intern</div>
                <div class="timeline-meta">Cognifyz Technologies · Jan 2026 – Mar 2026</div>
                <p class="timeline-desc">
                  Completed a structured internship focusing on <strong>coding, debugging, and modern development practices</strong>.
                  Worked on tasks involving writing, testing, and improving programs, which directly translates into
                  <strong>clean, maintainable, and reproducible data analysis code</strong>.
                </p>
              </div>

              <div class="timeline-item">
                <div class="timeline-role">Independent Data &amp; ML Projects</div>
                <div class="timeline-meta">2025 – Present · Python, pandas, NumPy, scikit learn, Streamlit</div>
                <p class="timeline-desc">
                  Built hands on projects such as a <strong>heart disease prediction app</strong> to practice the full workflow:
                  data collection, cleaning, feature engineering, model training/evaluation, and interactive visualization.
                </p>
              </div>
            </div>
          </div>
          <div class="section-footer">
            <a href="#skills" class="next-link">Next: Skills <span>→</span></a>
          </div>
        </section>

        <!-- SKILLS -->
        <section class="section" id="skills">
          <div class="section-header">
            <h2 class="section-title">Skills</h2>
            <div class="section-kicker">Practical tools I use</div>
          </div>
          <div class="section-body">
            <div class="skill-groups">
              <div>
                <div class="skill-group-title">Data &amp; Analytics</div>
                <div class="chips">
                  <span class="chip strong">Python (pandas, NumPy)</span>
                  <span class="chip strong">Data cleaning &amp; preprocessing</span>
                  <span class="chip">Handling missing values &amp; outliers</span>
                  <span class="chip">Encoding &amp; feature scaling</span>
                  <span class="chip">Exploratory data analysis (EDA)</span>
                  <span class="chip">Descriptive statistics &amp; correlation</span>
                  <span class="chip">Visualization (Matplotlib, Seaborn)</span>
                  <span class="chip">Basic dashboarding with Streamlit</span>
                </div>
              </div>

              <div>
                <div class="skill-group-title">Machine Learning</div>
                <div class="chips">
                  <span class="chip strong">Logistic Regression</span>
                  <span class="chip strong">Random Forest</span>
                  <span class="chip">SVM (concepts)</span>
                  <span class="chip">Ensemble methods (basics)</span>
                  <span class="chip">Train/test split &amp; cross validation</span>
                  <span class="chip">GridSearch hyperparameter tuning (basics)</span>
                  <span class="chip">Accuracy, Precision, Recall, F1 Score, ROC AUC</span>
                </div>
              </div>

              <div>
                <div class="skill-group-title">Software &amp; Tools</div>
                <div class="chips">
                  <span class="chip strong">Python</span>
                  <span class="chip">SQL · MySQL</span>
                  <span class="chip">C, C++, Java (basics)</span>
                  <span class="chip">Jupyter Notebook</span>
                  <span class="chip">VS Code</span>
                  <span class="chip">Git &amp; GitHub</span>
                  <span class="chip">HTML, CSS, JavaScript (basics)</span>
                  <span class="chip">Streamlit</span>
                </div>
              </div>

              <div>
                <div class="skill-group-title">Professional &amp; Languages</div>
                <div class="chips">
                  <span class="chip strong">Analytical &amp; problem solving mindset</span>
                  <span class="chip">Translating questions into analysis</span>
                  <span class="chip">Presenting findings clearly</span>
                  <span class="chip">English – Professional</span>
                  <span class="chip">French – Fluent / Professional</span>
                </div>
              </div>
            </div>
          </div>
          <div class="section-footer">
            <a href="#projects" class="next-link">Next: Projects <span>→</span></a>
          </div>
        </section>

        <!-- PROJECTS -->
        <section class="section" id="projects">
          <div class="section-header">
            <h2 class="section-title">Projects</h2>
            <div class="section-kicker">Applied data &amp; machine learning</div>
          </div>
          <div class="section-body">
            <p>
              I focus on projects that cover the full lifecycle: <strong>data preparation → modeling → evaluation → simple UI or visualization</strong>.
            </p>
            <div class="projects-grid">
              <!-- HEART DISEASE PROJECT -->
              <a class="project-card" href="https://github.com/kaderDjibo/heart-disease" target="_blank" rel="noopener">
                <div class="project-tag">
                  <span>ML · Streamlit App</span>
                </div>
                <h3 class="project-title">Medical Diagnosis of Heart Disease Using Machine Learning</h3>
                <p class="project-desc">
                  Built an AI driven system that predicts the likelihood of heart disease based on patient data, with an interactive interface for inputs and results.
                </p>
                <div class="project-meta">
                  <span class="project-stack">Python, pandas, NumPy, scikit learn, Streamlit, UCI Heart Disease Dataset</span>
                  <span class="project-link">View project →</span>
                </div>
              </a>

              <!-- SECOND DATA PROJECT -->
              <a class="project-card" href="https://github.com/kaderDjibo/BIG-DATA-ANALYSIS" target="_blank" rel="noopener">
                <div class="project-tag">
                  <span>Data Analysis</span>
                </div>
                <h3 class="project-title">Big Data Analysis</h3>
                <p class="project-desc">
                  Large-scale data analysis project focusing on cleaning, exploring, and visualizing big datasets to extract meaningful business insights.
                </p>
                <div class="project-meta">
                  <span class="project-stack">Python, pandas, Matplotlib/Seaborn</span>
                  <span class="project-link">View project →</span>
                </div>
              </a>

              <!-- SQL / BI PROJECT -->
              <a class="project-card" href="https://github.com/kaderDjibo/supermarket" target="_blank" rel="noopener">
                <div class="project-tag">
                  <span>SQL · Dashboard</span>
                </div>
                <h3 class="project-title">Supermarket Sales Dashboard</h3>
                <p class="project-desc">
                  Analysis of supermarket sales data using SQL and visual tools to understand revenue, product performance, and customer patterns.
                </p>
                <div class="project-meta">
                  <span class="project-stack">SQL, MySQL, BI / visualization tools</span>
                  <span class="project-link">View project →</span>
                </div>
              </a>
            </div>
          </div>
          <div class="section-footer">
            <a href="#certs" class="next-link">Next: Certifications <span>→</span></a>
          </div>
        </section>

        <!-- CERTIFICATIONS -->
        <section class="section" id="certs">
          <div class="section-header">
            <h2 class="section-title">Certifications &amp; Training</h2>
            <div class="section-kicker">Structured learning</div>
          </div>
          <div class="section-body">
            <p><strong>Industrial oriented Python Programming course</strong> (practical focus)</p>
            <p><strong>Practical course in Data Analysis &amp; Data Science</strong></p>
            <p><strong>Be 10X AI Course</strong> – exposure to applied AI tools and workflows</p>
            <p><strong>Internship Completion Certificate</strong> – Software Development Intern, Cognifyz Technologies</p>
          </div>
          <div class="section-footer">
            <a href="#contact" class="next-link">Next: Contact <span>→</span></a>
          </div>
        </section>
      </div>
    </section>

    <!-- RIGHT COLUMN / SIDEBAR -->
    <aside class="sidebar">
      <!-- CONTACT -->
      <section class="card" id="contact">
        <div class="card-header">
          <h2 class="card-title">Contact</h2>
          <span class="card-pill">Let&apos;s connect</span>
        </div>
        <div class="contact-list">
          <div class="contact-item">
            <span class="contact-label">Email</span>
            <a href="mailto:kadson82@gmail.com" class="contact-value">kadson82@gmail.com</a>
          </div>
          <div class="contact-item">
            <span class="contact-label">Phone</span>
            <span class="contact-value">+91 91 48 24 98 25</span>
          </div>
          <div class="contact-item">
            <span class="contact-label">Location</span>
            <span class="contact-value">Mysore, India</span>
          </div>
          <div class="contact-item">
            <span class="contact-label">Looking for</span>
            <span class="contact-value">Entry level Data Analyst · AI/ML Internships · Junior ML roles</span>
          </div>
        </div>
        <div class="email-highlight">
          Best way to reach me: <strong>kadson82@gmail.com</strong>
        </div>
        <p class="footnote">
          Open to remote and on site roles in India and internationally.
        </p>
      </section>

      <!-- LINKS -->
      <section class="card">
        <div class="card-header">
          <h2 class="card-title">Profiles</h2>
          <span class="card-pill">Online presence</span>
        </div>
        <div class="social-links">
          <a href="https://www.linkedin.com/in/djibo-abdoul-kader-8651a32ba/" target="_blank" rel="noopener" class="social-chip">LinkedIn</a>
          <a href="https://github.com/kaderDjibo" target="_blank" rel="noopener" class="social-chip">GitHub</a>
          <a href="https://www.kaggle.com/kadson" target="_blank" rel="noopener" class="social-chip">Kaggle</a>
        </div>
      </section>

      <!-- INSIGHTS / HOW YOU WORK -->
      <section class="card">
        <div class="card-header">
          <h2 class="card-title">How I Work</h2>
          <span class="card-pill">Process &amp; mindset</span>
        </div>
        <div class="blog-list">
          <div>
            <div class="blog-item-title">1. Start with the question</div>
            <div class="blog-meta">
              Clarify the business or domain question, define what a good answer looks like, and agree on metrics.
            </div>
          </div>
          <div>
            <div class="blog-item-title">2. Clean and understand the data</div>
            <div class="blog-meta">
              Handle missing values, outliers, encodings, and scaling. Use EDA to build intuition before modeling.
            </div>
          </div>
          <div>
            <div class="blog-item-title">3. Model, evaluate, and explain</div>
            <div class="blog-meta">
              Try simple, well understood models first. Focus on metrics like Precision, Recall, and ROC AUC and explain trade offs.
            </div>
          </div>
          <div>
            <div class="blog-item-title">4. Communicate &amp; iterate</div>
            <div class="blog-meta">
              Present results in clear language, with visuals and next step recommendations. Iterate based on feedback.
            </div>
          </div>
        </div>
        <p class="footnote">
          As I write blog posts or LinkedIn articles, I can link them here.
        </p>
      </section>
    </aside>
  </main>
</body>
</html>
