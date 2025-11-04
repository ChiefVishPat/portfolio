---
layout: null
title: Vishal Patel
---

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Vishal Patel – Software Engineer</title>

  <!-- Icon styles: Font Awesome + Devicon -->
  <link rel="stylesheet"
        href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"
        integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA=="
        crossorigin="anonymous" referrerpolicy="no-referrer" />
  <link rel="stylesheet"
        href="https://cdn.jsdelivr.net/gh/devicons/devicon@v2.15.1/devicon.min.css" />

  <style>
    :root {
      --bg: #f6e7d8;
      --bg-light: #fffaf6;
      --accent: #8b1538;
      --accent-light: #c74a5d;
      --accent-muted: #e0b0a0;
      --text: #2b2523;
      --muted: #7b6b67;
      --border: #e1cbb5;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: -apple-system, BlinkMacSystemFont, system-ui, -system-ui,
                   "Segoe UI", sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
    }

    a {
      color: var(--accent);
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    /* Hero banner inspired by Merlot */
    .hero {
      background: linear-gradient(135deg, var(--accent) 0%, var(--accent-light) 100%);
      color: #fff;
      padding: 2.8rem 1rem 3.4rem;
      text-align: center;
      position: relative;
      overflow: hidden;
    }

    .hero::before,
    .hero::after {
      content: "";
      position: absolute;
      left: 50%;
      transform: translateX(-50%);
      border-style: solid;
      border-width: 0 110px 40px 110px;
      border-color: transparent transparent #5c0e25 transparent;
      opacity: 0.8;
    }

    .hero::before {
      bottom: 0;
    }

    .hero-badge {
      display: inline-block;
      padding: 0.6rem 2.6rem 0.9rem;
      border-radius: 6px;
      border: 3px solid #5c0e25;
      background: linear-gradient(135deg, #b63a4b 0%, #8b1538 100%);
      box-shadow: 0 10px 25px rgba(0,0,0,0.18);
      position: relative;
      z-index: 1;
    }

    .hero-title {
      font-size: 2.4rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      margin: 0;
      font-weight: 700;
    }

    .hero-subtitle {
      margin: 0.3rem 0 0;
      font-size: 0.95rem;
      opacity: 0.9;
      font-style: italic;
    }

    /* Content container */
    .page {
      max-width: 960px;
      margin: -2.2rem auto 3rem;
      padding: 0 1rem 3rem;
    }

    .card {
      background: var(--bg-light);
      border-radius: 12px;
      border: 1px solid var(--border);
      box-shadow: 0 12px 30px rgba(0,0,0,0.07);
      padding: 1.7rem 1.7rem 2.2rem;
    }

    .layout {
      display: flex;
      flex-wrap: wrap;
      gap: 2rem;
    }

    .layout-left {
      flex: 0 0 260px;
      max-width: 260px;
    }

    .layout-right {
      flex: 1 1 0;
      min-width: 260px;
    }

    /* Profile block */
    .profile {
      text-align: center;
      margin-bottom: 1.2rem;
    }

    .profile img {
      border-radius: 50%;
      width: 130px;
      height: 130px;
      object-fit: cover;
      border: 3px solid #fff;
      box-shadow: 0 6px 20px rgba(0,0,0,0.25);
      margin-bottom: 0.6rem;
    }

    .profile-name {
      font-weight: 600;
    }

    .profile-tagline {
      font-size: 0.93rem;
      color: var(--muted);
      margin-top: 0.3rem;
    }

    .profile-socials {
      margin-top: 0.8rem;
    }

    .profile-socials a {
      margin: 0 0.25rem;
      display: inline-block;
      vertical-align: middle;
    }

    .profile-socials img {
      vertical-align: middle;
    }

    .profile-socials i {
      font-size: 1.2rem;
      vertical-align: middle;
    }

    .profile-tech {
      margin-top: 0.9rem;
      font-size: 1.5rem;
    }

    .profile-tech i {
      margin: 0 0.25rem;
      vertical-align: middle;
    }

    .profile-meta {
      margin-top: 0.9rem;
      font-size: 0.85rem;
      color: var(--muted);
    }

    /* Typography */
    h1, h2, h3 {
      font-family: inherit;
      color: var(--accent);
      margin-top: 1.2rem;
      margin-bottom: 0.6rem;
    }

    h1 {
      font-size: 1.6rem;
    }

    h2 {
      font-size: 1.25rem;
      border-bottom: 1px solid var(--border);
      padding-bottom: 0.3rem;
    }

    h3 {
      font-size: 1.05rem;
      margin-top: 1rem;
    }

    .section {
      margin-bottom: 1.6rem;
    }

    .subtitle-line {
      font-size: 0.92rem;
      color: var(--muted);
      margin-bottom: 0.4rem;
    }

    ul {
      padding-left: 1.1rem;
      margin-top: 0.4rem;
      margin-bottom: 0.4rem;
    }

    /* Buttons/links */
    .btn {
      display: inline-block;
      padding: 0.5rem 0.9rem;
      border-radius: 999px;
      background: var(--accent);
      color: #fff;
      font-size: 0.9rem;
      font-weight: 500;
      text-decoration: none;
      border: none;
      cursor: pointer;
    }

    .btn:hover {
      background: #5c0e25;
      text-decoration: none;
    }

    .muted {
      color: var(--muted);
    }

    .projects-list h3 {
      margin-bottom: 0.15rem;
    }

    .projects-meta {
      font-size: 0.87rem;
      color: var(--muted);
      margin-bottom: 0.35rem;
    }

    .project-links a {
      margin-right: 0.6rem;
      font-size: 0.88rem;
    }

    @media (max-width: 720px) {
      .page {
        margin-top: -1.5rem;
      }
      .layout-left, .layout-right {
        max-width: 100%;
        flex: 1 1 100%;
      }
      .card {
        padding: 1.4rem 1.2rem 1.8rem;
      }
    }
  </style>
</head>

<body>
  <header class="hero">
    <div class="hero-badge">
      <h1 class="hero-title">Vishal Patel</h1>
      <p class="hero-subtitle">
        Software Engineer – AI, Fintech, and Backend Systems
      </p>
    </div>
  </header>

  <main class="page">
    <section class="card">
      <div class="layout">
        <!-- LEFT: profile & sidebar-ish info -->
        <aside class="layout-left">
          <div class="profile">
            <img src="assets/pfp.jpeg" alt="Vishal Patel profile picture" />

            <div class="profile-name">Vishal Patel</div>
            <div class="profile-tagline">
              Backend-leaning software engineer, open to all engineering roles.
              Adaptable, determined builder, hungry to learn and ship products that actually move the needle.
            </div>

            <div class="profile-socials">
              <!-- GitHub via Simple Icons CDN -->
              <a href="https://github.com/ChiefVishPat"
                 target="_blank" rel="noopener noreferrer" aria-label="GitHub">
                <img src="https://cdn.simpleicons.org/github/ffffff"
                     width="26" height="26" alt="GitHub" />
              </a>

              <!-- LinkedIn via Simple Icons CDN -->
              <a href="https://www.linkedin.com/in/vishalpatel2003"
                 target="_blank" rel="noopener noreferrer" aria-label="LinkedIn">
                <img src="https://cdn.simpleicons.org/linkedin/0A66C2"
                     width="26" height="26" alt="LinkedIn" />
              </a>

              <!-- Resume icon -->
              <a href="vishal-patel-resume.pdf"
                 target="_blank" rel="noopener noreferrer" aria-label="Resume PDF">
                <i class="fa-solid fa-file-pdf"></i>
              </a>
            </div>

            <div class="profile-tech">
              <i class="devicon-python-plain colored" title="Python"></i>
              <i class="devicon-postgresql-plain colored" title="PostgreSQL"></i>
              <i class="devicon-fastapi-plain colored" title="FastAPI"></i>
              <i class="devicon-react-original colored" title="React"></i>
              <i class="devicon-typescript-plain colored" title="TypeScript"></i>
              <i class="devicon-git-plain colored" title="Git"></i>
            </div>

            <div class="profile-meta">
              Based in Clifton, NJ · **U.S. citizen, no sponsorship required**
            </div>

            <div style="margin-top:0.8rem;">
              <a class="btn" href="vishal-patel-resume.pdf"
                 target="_blank" rel="noopener noreferrer">
                Download Resume
              </a>
            </div>
          </div>
        </aside>

        <!-- RIGHT: main content -->
        <section class="layout-right">
          <!-- About -->
          <section class="section" id="about">
            <h2>About</h2>
            <p>
              I'm a software engineer focused on building reliable backend systems and
              AI-powered workflows for real-world finance and operations use cases.
              I specialize in backend engineering, but I’m open to all kinds of engineering roles
              because I’m an adaptable, determined builder who enjoys learning quickly and shipping
              products that matter.
            </p>
            <p>
              I am a <strong>U.S. citizen and do not require visa sponsorship</strong>.
            </p>
            <p>
              Recently, I’ve:
            </p>
            <ul>
              <li>
                Contracted at <strong>Ramp</strong>, shipping backend receipt integrations used by major
                merchants like United Airlines, Delta Airlines, and Walmart.
              </li>
              <li>
                Built AI-driven agents that automate inboxes, document workflows, and data extraction.
              </li>
            </ul>
            <p>
              I enjoy working close to the product: understanding real customer pain points,
              then building systems that are observable, resilient, and easy to iterate on.
            </p>
          </section>

          <!-- Experience -->
          <section class="section" id="experience">
            <h2>Experience</h2>

            <h3>Stealth AI FinTech Startup – Credit Risk &amp; Fraud Automation</h3>
            <div class="subtitle-line">
              <strong>Software Engineer (Contract)</strong> · August 2025 – November 2025 ·
              Python, SQL (PostgreSQL), LangChain/LangGraph, PydanticAI
            </div>
            <ul>
              <li>
                Architected an AI-driven email agent that triaged high-volume AP/AR inboxes in real time,
                eliminating manual sorting and reducing missed vendor/customer inquiries.
              </li>
              <li>
                Automated intent detection and response drafting for common finance workflows
                (payment status, invoice copies, disputes), reducing analyst workload by an estimated 60–70%.
              </li>
              <li>
                Designed an extensible orchestration layer (LangGraph + PydanticAI) that scaled across
                multiple tenants and channels (email, WhatsApp, Slack), supporting enterprise-grade throughput.
              </li>
            </ul>

            <h3>Ramp</h3>
            <div class="subtitle-line">
              <strong>Software Engineer (Contract)</strong> · July 2024 – December 2024 ·
              Python, SQL (PostgreSQL)
            </div>
            <ul>
              <li>
                Developed backend receipt integrations with high-TPV merchants (+$421.85M, &gt;1.26M transactions
                annually), including United Airlines, Delta Airlines, and Walmart, driving adoption of Ramp Plus.
              </li>
              <li>
                Built internal APIs and database migrations to capture structured receipt data and improve
                cross-service communication.
              </li>
              <li>
                Helped drive rollout from internal launch → alpha → beta → GA, improving the receipt experience
                of thousands of users with ~87% success across shipped integrations.
              </li>
            </ul>
          </section>

          <!-- Projects -->
          <section class="section" id="projects">
            <h2>Selected Projects</h2>
            <p class="muted">
              A few projects that represent how I like to build: practical, reliable, and focused on real workflows.
            </p>

            <div class="projects-list">
              <h3>Interactive Story Generator – Full-stack AI Storytelling Engine</h3>
              <div class="projects-meta">
                TypeScript, React, FastAPI, PostgreSQL, OpenAI, LangChain, SQLAlchemy, Vite
              </div>
              <p>
                Full-stack LLM-powered “choose your own adventure” engine. Users provide a theme and receive a
                playable branching narrative with multiple endings and shareable URLs.
              </p>
              <ul>
                <li>Recursive story-tree processing and async job queues.</li>
                <li>
                  LangChain + Pydantic pipeline to validate deeply nested JSON into structured DB rows.
                </li>
              </ul>
              <div class="project-links">
                <a href="https://github.com/ChiefVishPat/your-repo-here"
                   target="_blank" rel="noopener noreferrer">Code</a>
                <a href="https://dd4da2b8-8671-4d7c-9aa9-41425b5926a6.e1-us-east-azure.choreoapps.dev/"
                   target="_blank" rel="noopener noreferrer">Live demo</a>
              </div>
              <!-- TODO: replace `your-repo-here` with the actual repo name -->
            </div>

            <div class="projects-list">
              <h3>Google Shopping Web Scraper using Crawl4AI</h3>
              <div class="projects-meta">
                Python, Crawl4AI, Playwright, Pydantic, OpenAI, uv
              </div>
              <p>
                AI-assisted crawler that clicks through Google Shopping results, opens product sidebars,
                and extracts structured data (name, reviews, ratings, prices, and outbound store links).
              </p>
              <ul>
                <li>
                  GPT-generated CSS/JSON extraction schema cached to disk to minimize token usage.
                </li>
                <li>
                  Interactive CLI that prompts for a search term, launches a headless browser,
                  and saves JSON results into a <code>scrapes/</code> directory.
                </li>
              </ul>
              <div class="project-links">
                <a href="https://github.com/ChiefVishPat/web_crawler"
                   target="_blank" rel="noopener noreferrer">Code</a>
                <a href="https://www.loom.com/share/d87f88f6918a48b2b121e1afcc40b761"
                   target="_blank" rel="noopener noreferrer">Video demo</a>
              </div>
            </div>

            <div class="projects-list">
              <h3>Expense Policy Agent – AI-Powered Email Automation</h3>
              <div class="projects-meta">
                Python, LangGraph, PydanticAI, FastAPI, Redis, Gmail API, OpenAI
              </div>
              <p>
                AI agent that automates AP/AR inboxes in real time by classifying incoming vendor and
                expense-related emails, fetching matching receipts or invoices, and drafting accurate replies.
              </p>
              <ul>
                <li>
                  Robust orchestration layer (LangGraph + PydanticAI) for multi-step intent detection and validation.
                </li>
                <li>
                  Redis-backed queues for async message handling and retry logic.
                </li>
              </ul>
              <div class="project-links">
                <a href="https://github.com/ChiefVishPat/expense-policy-agent"
                   target="_blank" rel="noopener noreferrer">Code</a>
                <a href="https://www.loom.com/share/454f7f5716c94de4b64474612a10660d"
                   target="_blank" rel="noopener noreferrer">Video demo</a>
              </div>
            </div>

            <div class="projects-list">
              <h3>Intelligent Slack Agent for Document Processing &amp; Summarization</h3>
              <div class="projects-meta">
                Python, Slack API, OpenAI GPT, GitHub API
              </div>
              <p>
                Slack agent that automates document intake workflows by ingesting PDFs/DOCX/TXT,
                summarizing them with GPT, and posting readable summaries back to Slack.
              </p>
              <ul>
                <li>Dynamic prompt switching for context-specific summaries.</li>
                <li>
                  Async file handling and GitHub issue creation for collaboration and follow-ups.
                </li>
              </ul>
              <div class="project-links">
                <a href="https://github.com/ChiefVishPat/missing-contract-legal-agent"
                   target="_blank" rel="noopener noreferrer">Code</a>
                <a href="https://www.loom.com/share/c7ac32dee35e47cb89f2a810589b3284"
                   target="_blank" rel="noopener noreferrer">Video demo</a>
              </div>
            </div>

            <p style="margin-top:1.1rem;">
              <a class="btn"
                 href="https://github.com/ChiefVishPat?tab=repositories"
                 target="_blank" rel="noopener noreferrer">
                View all projects on GitHub
              </a>
            </p>
          </section>
        </section>
      </div>
    </section>
  </main>
</body>
</html>
