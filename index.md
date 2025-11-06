---
layout: default
title: Vishal Patel
---

<!-- Icon styles for this page -->
<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"
  integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA=="
  crossorigin="anonymous"
  referrerpolicy="no-referrer"
/>
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/gh/devicons/devicon@v2.15.1/devicon.min.css"
/>

<style>
  /* Quick knobs you can tweak */
  :root {
    --pfp-size: 220px;     /* change to resize profile photo */
    --pfp-zoom: 1.00;      /* 1.0 = no zoom; increase to zoom in */
    --pfp-y: 60%;          /* vertical focus point (0% top, 50% center) */
    --tech-size: 1.6rem;   /* icon size for technologies */
    --social-size: 30px;   /* icon size for socials */
  }
  /* Hide default Minimal theme chrome */
  header,
  footer,
  .view {
    display: none !important;
  }

  /* Expand the Minimal theme canvas so two columns fit side-by-side */
  .wrapper {
    width: min(1200px, 92vw) !important;
    margin: 0 auto !important;
  }

  /* Let our page content use full width instead of the theme's 500px */
  .wrapper > section {
    width: 100% !important;
    float: none !important;
    padding: 0 !important;
    margin: 0 !important;
    border: 0 !important;
  }

  /* Minimal navigation */
  .simple-nav {
    display: flex;
    gap: 0.75rem;
    align-items: center;
    padding: 0.6rem 0.25rem;
    margin: 0.25rem 0 0.75rem;
    border-bottom: 1px solid #e5e7eb;
    position: sticky;
    top: 0;
    background: #fff;
    z-index: 20;
  }
  .simple-nav a {
    color: #374151;
    text-decoration: none;
    font-weight: 600;
    padding: 0.25rem 0.5rem;
    border-radius: 6px;
  }
  .simple-nav a:hover { background: #f3f4f6; }
  .simple-nav a[aria-current="page"] { color: #1f4ba0; }

  .page-layout {
    display: flex;
    flex-wrap: wrap;
    align-items: flex-start;
    gap: 2.5rem;
    margin-top: 0;
  }

  .page-left {
    flex: 0 0 300px;
    max-width: 300px;
  }

  .page-right {
    flex: 1 1 420px;
    min-width: 340px;
  }

  .profile-hero h1 {
    margin: 0;
    font-size: 2rem;
    line-height: 1.2;
  }

  .profile-hero p {
    margin: 0.35rem 0 0;
    font-size: 1.05rem;
    color: #333;
  }

  .resume-link {
    display: inline-block;
    margin-top: 0.75rem;
    font-weight: 600;
    text-decoration: none;
    color: #1f4ba0;
  }

  .resume-link:hover,
  .resume-link:focus {
    text-decoration: underline;
  }

  .profile-card {
    text-align: left;
    margin-top: 0.75rem;
  }

  /* Circle mask stays fixed; image inside zooms */
  .pfp-wrap {
    width: var(--pfp-size);
    height: var(--pfp-size);
    border-radius: 50%;
    overflow: hidden; /* crop the zoomed image */
    margin: 0 0 0.9rem 0;
    box-shadow: 0 2px 10px rgba(0,0,0,0.06);
  }
  .profile-card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: 50% var(--pfp-y);
    transform: scale(var(--pfp-zoom));
    transform-origin: 50% var(--pfp-y);
    display: block;
  }

  .profile-summary { margin: 0.4rem 0 0.6rem; }

  .profile-socials {
    margin-top: 0.45rem;
  }

  .profile-socials a {
    margin-right: 0.45rem;
    display: inline-block;
    vertical-align: middle;
  }

  .profile-socials { display: flex; gap: 0.55rem; align-items: center; }
  .profile-socials a { line-height: 0; }
  .profile-socials svg { width: var(--social-size); height: var(--social-size); fill: #333; }
  .profile-socials a:hover svg, .profile-socials a:focus svg { fill: #0a66c2; }

  .tech-label { font-size: 0.9rem; color: #6b7280; letter-spacing: .02em; text-transform: uppercase; font-weight: 600; margin-top: 0.4rem; }
  .tech-pills { margin-top: 0.35rem; display: flex; flex-wrap: wrap; gap: 0.5rem; align-items: center; }
  .tech-pill { display: inline-flex; align-items: center; gap: 0.35rem; padding: 0.25rem 0.5rem; border-radius: 999px; background: #eef2f7; color: #334155; border: 1px solid #e5e7eb; line-height: 1; }
  .tech-pill i { font-size: var(--tech-size); line-height: 1; }
  .tech-pill svg { width: calc(var(--tech-size) * 0.9); height: calc(var(--tech-size) * 0.9); display: inline-block; }
  .tech-pill img { width: calc(var(--tech-size) * 0.95); height: calc(var(--tech-size) * 0.95); display: inline-block; object-fit: contain; }
  .badge { font-size: 0.70rem; font-weight: 600; padding: 0.25rem 0.45rem; border-radius: 999px; background: #eef2f7; color: #334155; border: 1px solid #e5e7eb; }

  .project-heading {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    gap: 0.75rem;
    flex-wrap: wrap;
  }

  .project-links {
    display: flex;
    gap: 0.65rem;
    font-size: 0.9rem;
  }

  .project-links a {
    color: #1f4ba0;
    text-decoration: none;
    font-weight: 600;
  }

  .project-links a:hover,
  .project-links a:focus {
    text-decoration: underline;
  }

  .open-modal { cursor: pointer; }

  .modal-overlay {
    position: fixed;
    inset: 0;
    background: rgba(15, 23, 42, 0.65);
    display: none;
    align-items: center;
    justify-content: center;
    padding: 1.5rem;
    z-index: 100;
  }

  .modal-overlay.active { display: flex; }

  .modal-content {
    width: min(840px, 100%);
    background: #fff;
    border-radius: 12px;
    box-shadow: 0 25px 60px rgba(15, 23, 42, 0.25);
    padding: 1.25rem;
    position: relative;
  }

  .modal-close {
    position: absolute;
    top: 0.75rem;
    right: 0.75rem;
    background: transparent;
    border: none;
    font-size: 1.5rem;
    cursor: pointer;
    color: #111827;
  }

  .modal-close:hover,
  .modal-close:focus { color: #1f4ba0; }

  .modal-body { margin-top: 1.5rem; }

  .modal-body iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border-radius: 8px;
    border: 0;
  }

  .modal-fallback { margin-top: 0.75rem; font-size: 0.9rem; }

  /* Faint shadow-like dividers */
  .shadow-divider {
    height: 1px;
    border: 0;
    background: linear-gradient(to right, rgba(0,0,0,0.10), rgba(0,0,0,0.04), rgba(0,0,0,0.02), rgba(0,0,0,0));
    box-shadow: 0 1px 2px rgba(0,0,0,0.06);
    margin: 1rem 0;
  }

  /* Responsive: stack columns on smaller screens */
  @media (max-width: 980px) {
    .page-layout {
      flex-direction: column;
      gap: 1.5rem;
    }
    .page-left,
    .page-right {
      flex: 1 1 auto;
      max-width: 100%;
      min-width: 0;
    }
  }
</style>




<nav class="simple-nav">
  <a href="{{ site.baseurl }}/" aria-current="page">Home</a>
  <a href="{{ site.baseurl }}/projects">Projects</a>
</nav>

<div class="page-layout">
  <!-- LEFT COLUMN: PFP → name/desc → socials → tech -->
  <aside class="page-left">
    <div class="profile-card">
      <div class="pfp-wrap">
        <img src="{{ site.baseurl }}/assets/pfp.png" alt="Vishal Patel profile picture" />
      </div>
    </div>

    <hr class="shadow-divider" />

    <div class="profile-hero">
      <h1>Vishal Patel</h1>
      <p>Software Engineer – Backend, AI, Fintech, Solutions Engineering</p>
      <a
        class="resume-link"
        href="{{ site.baseurl }}/vishal-patel-resume.pdf"
        target="_blank"
        rel="noopener noreferrer"
      >
        Download Resume
      </a>
    </div>

    <hr class="shadow-divider" />

    <div class="profile-socials" aria-label="Social links">
      <!-- GitHub (inline SVG to ensure it always renders) -->
      <a href="https://github.com/ChiefVishPat" target="_blank" rel="noopener noreferrer" aria-label="GitHub">
        <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M12 .5a12 12 0 0 0-3.79 23.4c.6.11.82-.26.82-.58l-.02-2.03c-3.34.73-4.04-1.61-4.04-1.61-.55-1.41-1.34-1.79-1.34-1.79-1.1-.75.08-.73.08-.73 1.22.09 1.86 1.26 1.86 1.26 1.08 1.85 2.83 1.31 3.52 1 .11-.78.42-1.31.76-1.61-2.67-.31-5.47-1.33-5.47-5.93 0-1.31.47-2.38 1.24-3.22-.12-.31-.54-1.56.12-3.26 0 0 1.01-.32 3.3 1.23a11.5 11.5 0 0 1 6 0c2.28-1.55 3.29-1.23 3.29-1.23.66 1.7.24 2.95.12 3.26.77.84 1.23 1.91 1.23 3.22 0 4.61-2.8 5.61-5.48 5.92.43.38.81 1.12.81 2.26l-.01 3.35c0 .32.22.69.82.58A12 12 0 0 0 12 .5Z"/></svg>
      </a>
      <!-- LinkedIn -->
      <a href="https://www.linkedin.com/in/vishalpatel2003" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn">
        <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M4.98 3.5C4.98 4.88 3.86 6 2.5 6S0 4.88 0 3.5 1.12 1 2.5 1 4.98 2.12 4.98 3.5zM.5 8h4V24h-4V8zM8 8h3.8v2.2h.06c.53-1 1.82-2.2 3.75-2.2 4.01 0 4.75 2.64 4.75 6.08V24h-4v-7.2c0-1.72-.03-3.94-2.4-3.94-2.4 0-2.77 1.87-2.77 3.8V24h-4V8z"/></svg>
      </a>
      <!-- Email -->
      <a href="mailto:vishpat2003@gmail.com" target="_blank" rel="noopener noreferrer" aria-label="Email">
        <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M20 4H4a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2Zm0 4-8 5L4 8V6l8 5 8-5v2Z"/></svg>
      </a>
    </div>

    <hr class="shadow-divider" />

    <div class="tech-label">Technologies</div>
    <div class="tech-pills" aria-label="Technologies">
      <span class="tech-pill" title="Python"><i class="devicon-python-plain colored" aria-hidden="true"></i><span>Python</span></span>
      <span class="tech-pill" title="Java"><i class="devicon-java-plain colored" aria-hidden="true"></i><span>Java</span></span>
      <span class="tech-pill" title="FastAPI"><i class="devicon-fastapi-plain colored" aria-hidden="true"></i><span>FastAPI</span></span>
      <span class="tech-pill" title="PostgreSQL"><i class="devicon-postgresql-plain colored" aria-hidden="true"></i><span>PostgreSQL</span></span>
      <span class="tech-pill" title="Redis"><i class="devicon-redis-plain colored" aria-hidden="true"></i><span>Redis</span></span>
      <span class="tech-pill" title="React"><i class="devicon-react-original colored" aria-hidden="true"></i><span>React</span></span>
      <span class="tech-pill" title="TypeScript"><i class="devicon-typescript-plain colored" aria-hidden="true"></i><span>TypeScript</span></span>
      <span class="tech-pill" title="LangGraph">
        <img src="https://cdn.simpleicons.org/langgraph/2563eb" alt="LangGraph logo" />
        <span>LangGraph</span>
      </span>
      <span class="tech-pill" title="LangChain">
        <img src="https://cdn.simpleicons.org/langchain/00bf9a" alt="LangChain logo" />
        <span>LangChain</span>
      </span>
      <span class="tech-pill" title="PydanticAI">
        <img src="https://cdn.simpleicons.org/pydantic/0ea5e9" alt="Pydantic logo" />
        <span>PydanticAI</span>
      </span>
      <span class="tech-pill" title="OpenAI">
        <img src="https://cdn.simpleicons.org/openai/412991" alt="OpenAI logo" />
        <span>OpenAI</span>
      </span>
      <span class="tech-pill" title="Git"><i class="devicon-git-plain colored" aria-hidden="true"></i><span>Git</span></span>
    </div>
  </aside>

  <!-- RIGHT COLUMN: whole main content (About, Experience, Projects) -->
  <section class="page-right" markdown="1">
## About Me

I’m a software engineer who enjoys building reliable systems and intelligent workflows that make real-world products more efficient and user-focused. Most of my experience has been in backend and AI-driven automation within fintech, but I’m always eager to learn across the stack and take on engineering challenges that deliver tangible impact.

I am a **U.S. citizen and do not require visa sponsorship**.

Recently, I’ve:

- Contracted at **Ramp**, shipping backend receipt integrations used by major
  merchants like United Airlines, Delta Airlines, and Walmart.
- Built AI-driven agents that automate inboxes, document workflows, and data
  extraction.

I enjoy working close to the product: understanding real customer pain points,
then building systems that are observable, resilient, and easy to iterate on.

---

## Experience

### Stealth AI FinTech Startup – Credit Risk & Fraud Automation  
**Software Engineer (Contract)** · August 2025 – November 2025  
Python, SQL (PostgreSQL), LangChain/LangGraph, PydanticAI  

- Architected an AI-driven email agent that triaged high-volume AP/AR inboxes in real time, eliminating manual sorting and reducing missed vendor/customer inquiries.
- Automated intent detection and response drafting for common finance workflows (payment status, invoice copies, disputes), reducing analyst workload by an estimated 60–70%.
- Designed an extensible orchestration layer (LangGraph + PydanticAI) that scaled across multiple tenants and channels (email, WhatsApp, Slack), supporting enterprise-grade throughput.

---

### Ramp  
**Software Engineer (Contract)** · July 2024 – December 2024  
Python, SQL (PostgreSQL)

- Developed backend receipt integrations with high-TPV merchants (+$421.85M, >1.26M transactions annually), including United Airlines, Delta Airlines, and Walmart, driving adoption of Ramp Plus.
- Built internal APIs and DB migrations to capture structured receipt data and improve cross-service communication.
- Helped drive rollout from internal launch → alpha → beta → GA, improving the receipt experience of thousands of users with ~87% success across shipped integrations.

---

## Projects

Here are a few selected projects. For the full list, see the Projects page or my GitHub.

<div class="project-heading">
  <h3>Interactive Story Generator – Full-stack AI Storytelling Engine</h3>
  <div class="project-links">
    <a href="https://github.com/ChiefVishPat/interactive-story-generator" target="_blank" rel="noopener noreferrer">Source Code</a>
    <a href="https://dd4da2b8-8671-4d7c-9aa9-41425b5926a6.e1-us-east-azure.choreoapps.dev/" target="_blank" rel="noopener noreferrer">Demo App</a>
  </div>
</div>
**Tech:** TypeScript, React, FastAPI, PostgreSQL, OpenAI, LangChain, SQLAlchemy, Vite  

Built an LLM-powered “choose your own adventure” engine: users provide a theme, and the system generates a branching narrative with multiple endings and shareable URLs.

- Recursive story-tree processing and async job queues.
- LangChain + Pydantic pipeline to validate deeply nested JSON into structured DB rows.

---

<div class="project-heading">
  <h3>Google Shopping Web Scraper using Crawl4AI</h3>
  <div class="project-links">
    <a href="https://github.com/ChiefVishPat/web_crawler" target="_blank" rel="noopener noreferrer">Source Code</a>
    <a href="#" class="open-modal" data-modal="loom-web-crawler-home">Demo Video</a>
  </div>
</div>
**Tech:** Python, Crawl4AI, Playwright, Pydantic, OpenAI, uv  

Built an AI-assisted crawler for Google Shopping.

- Clicks each search result, opens the sidebar, and extracts product data (name, reviews, ratings, prices, store links).
- Generates the CSS/JSON extraction schema once with GPT-4.1‑nano, caches it, and reuses it to cut token usage.
- Provides an interactive CLI to prompt for a query, launch a headless browser, and save JSON output into a `scrapes/` directory.

<div id="loom-web-crawler-home" class="modal-overlay" role="dialog" aria-modal="true" aria-labelledby="loom-web-crawler-home-title">
  <div class="modal-content">
    <button class="modal-close" type="button" aria-label="Close">×</button>
    <h4 id="loom-web-crawler-home-title">Google Shopping Web Scraper Demo</h4>
    <div class="modal-body">
      <div style="position: relative; padding-bottom: 64.63195691202873%; height: 0;">
        <iframe data-src="https://www.loom.com/embed/d87f88f6918a48b2b121e1afcc40b761" allowfullscreen></iframe>
      </div>
      <p class="modal-fallback">
        Prefer a new tab?
        <a href="https://www.loom.com/share/d87f88f6918a48b2b121e1afcc40b761" target="_blank" rel="noopener noreferrer">Watch on Loom</a>.
      </p>
    </div>
  </div>
</div>

---

<div class="project-heading">
  <h3>Pharmaceutical Voice AI Assistant</h3>
  <div class="project-links">
    <a href="https://github.com/ChiefVishPat/pharmacist-voice-assistant" target="_blank" rel="noopener noreferrer">Source Code</a>
  </div>
</div>
**Tech:** Python, WebSockets, Asyncio, Deepgram, Twilio, OpenAI  

Real-time voice pharmacy assistant that handles drug inquiries, orders, and tracking over natural phone conversations.

- Built a bidirectional streaming pipeline between Twilio MediaStreams and Deepgram’s Agent API.
- Designed an LLM-driven function-calling system for operations like drug lookup, order placement, and tracking via schema-validated JSON.
- Implemented intelligent barge-in handling so users can interrupt mid-sentence.

---

[View detailed projects →]({{ site.baseurl }}/projects)  
[View all repositories on GitHub →](https://github.com/ChiefVishPat?tab=repositories){:target="_blank" rel="noopener noreferrer"}

  </section>
</div>

<script>
  (function() {
    const modalTriggers = document.querySelectorAll('.open-modal');
    const modals = document.querySelectorAll('.modal-overlay');

    if (!modalTriggers.length || !modals.length) return;

    function closeModal(modal) {
      if (!modal) return;
      modal.classList.remove('active');
      const iframe = modal.querySelector('iframe');
      if (iframe && iframe.src) {
        iframe.dataset.src = iframe.src;
        iframe.src = '';
      }
    }

    modalTriggers.forEach(trigger => {
      trigger.addEventListener('click', event => {
        event.preventDefault();
        const id = trigger.getAttribute('data-modal');
        const modal = document.getElementById(id);
        if (modal) {
          modal.classList.add('active');
          const iframe = modal.querySelector('iframe');
          if (iframe && iframe.dataset.src) {
            iframe.src = iframe.dataset.src;
            delete iframe.dataset.src;
          }
        }
      });
    });

    modals.forEach(modal => {
      modal.addEventListener('click', event => {
        if (event.target === modal || event.target.classList.contains('modal-close')) {
          closeModal(modal);
        }
      });
    });

    document.addEventListener('keydown', event => {
      if (event.key === 'Escape') {
        modals.forEach(closeModal);
      }
    });
  })();
</script>
