---
layout: default
title: Projects
permalink: /projects
---

<style>
  /* Hide Minimal theme chrome so only our content shows */
  header, footer, .view { display: none !important; }

  /* Give us a wider canvas like the home page */
  .wrapper { width: min(1200px, 96vw) !important; margin: 0 auto !important; }
  .wrapper > section { width: 100% !important; float: none !important; padding: 0 !important; margin: 0 !important; border: 0 !important; }

  .page-layout { display: flex; flex-wrap: wrap; align-items: flex-start; gap: 2rem; }
  .page-left  { flex: 1 1 58%; min-width: 420px; }
  .page-right { flex: 1 1 34%; min-width: 280px; }

  .shadow-divider { height: 1px; border: 0; background: linear-gradient(to right, rgba(0,0,0,0.10), rgba(0,0,0,0.04), rgba(0,0,0,0.02), rgba(0,0,0,0)); box-shadow: 0 1px 2px rgba(0,0,0,0.06); margin: 1rem 0; }

  /* Minimal navigation */
  .simple-nav { display: flex; gap: .75rem; align-items: center; padding: .6rem .25rem; margin: .25rem 0 .75rem; border-bottom: 1px solid #e5e7eb; position: sticky; top: 0; background: #fff; z-index: 20; }
  .simple-nav a { color: #374151; text-decoration: none; font-weight: 600; padding: .25rem .5rem; border-radius: 6px; }
  .simple-nav a:hover { background: #f3f4f6; }
  .simple-nav a[aria-current="page"] { color: #1f4ba0; }

  /* Left column typography */
  .page-left h1 { margin: 0 0 .75rem; }
  .page-left h3 { margin: 1rem 0 .35rem; }
  .page-left p  { margin: 0.25rem 0 0.5rem; }
  .page-left ul { margin: 0.25rem 0 0.75rem 1.2rem; }
  .page-left a { text-decoration: none; color: #1f4ba0; }
  .page-left a:hover { text-decoration: underline; }

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
    font-weight: 600;
    text-decoration: none;
  }

  .project-links a:hover,
  .project-links a:focus { text-decoration: underline; }

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

  /* Repo list */
  .repo-box { border: 1px solid #e1e4e8; border-radius: 6px; padding: 0.75rem 1rem; background: #fafbfc; max-height: 70vh; overflow-y: auto; }
  .repo-item { margin-bottom: 0.45rem; }
  .repo-item a { font-weight: 500; }
  .repo-item span { color: #66727f; font-size: 0.9rem; }

  @media (max-width: 980px) {
    .page-layout { flex-direction: column; gap: 1.5rem; }
    .page-left, .page-right { flex: 1 1 auto; max-width: 100%; }
  }
</style>

<nav class="simple-nav">
  <a href="{{ site.baseurl }}/">Home</a>
  <a href="{{ site.baseurl }}/projects" aria-current="page">Projects</a>
</nav>

<div class="page-layout">
<!-- LEFT: Featured projects -->
<section class="page-left" markdown="1">

# Projects

A few projects that represent how I like to build: practical, reliable, and focused on real-world workflows.

---

## Featured Projects

<div class="project-heading">
  <h3>🧾 Expense Policy Agent – AI-Powered Email Automation</h3>
  <div class="project-links">
    <a href="https://github.com/ChiefVishPat/expense-policy-chatbot" target="_blank" rel="noopener noreferrer">Source Code</a>
    <a href="#" class="open-modal" data-modal="loom-expense-policy">Demo Video</a>
  </div>
</div>

**Tech:** Python, FastAPI, Slack API, OpenAI, LangChain/LangGraph, Pydantic  

- Parses natural-language expense requests into structured JSON with OpenAI.
- Enforces policy (spend caps, categories, pre-approval thresholds) via a rules engine.
- Routes out-of-policy requests to Finance for one-click approval/rejection with threaded Slack workflows.

<div id="loom-expense-policy" class="modal-overlay" role="dialog" aria-modal="true" aria-labelledby="loom-expense-policy-title">
  <div class="modal-content">
    <button class="modal-close" type="button" aria-label="Close">×</button>
    <h4 id="loom-expense-policy-title">Expense Policy Agent Demo</h4>
    <div class="modal-body">
      <div style="position: relative; padding-bottom: 64.63195691202873%; height: 0;">
        <iframe data-src="https://www.loom.com/embed/454f7f5716c94de4b64474612a10660d" allowfullscreen></iframe>
      </div>
      <p class="modal-fallback">
        Prefer a new tab?
        <a href="https://www.loom.com/share/454f7f5716c94de4b64474612a10660d" target="_blank" rel="noopener noreferrer">Watch on Loom</a>.
      </p>
    </div>
  </div>
</div>

---

<div class="project-heading">
  <h3>🧠 Interactive Story Generator – Full-stack AI Storytelling Engine</h3>
  <div class="project-links">
    <a href="https://github.com/ChiefVishPat/interactive-story-generator" target="_blank" rel="noopener noreferrer">Source Code</a>
    <a href="https://dd4da2b8-8671-4d7c-9aa9-41425b5926a6.e1-us-east-azure.choreoapps.dev/" target="_blank" rel="noopener noreferrer">Demo App</a>
  </div>
</div>

**Tech:** TypeScript, React, FastAPI, PostgreSQL, OpenAI, LangChain, SQLAlchemy, Vite  

- Built an LLM-powered “choose your own adventure” engine with multiple endings and shareable URLs.
- Architected recursive story-tree processing, async job queues, and a LangChain + Pydantic pipeline to validate deeply nested JSON into structured DB rows.

---

<div class="project-heading">
  <h3>🛒 Google Shopping Web Scraper using Crawl4AI</h3>
  <div class="project-links">
    <a href="https://github.com/ChiefVishPat/web_crawler" target="_blank" rel="noopener noreferrer">Source Code</a>
    <a href="#" class="open-modal" data-modal="loom-web-crawler">Demo Video</a>
  </div>
</div>

**Tech:** Python, Crawl4AI, Playwright, Pydantic, OpenAI, uv  

- Clicks each Google Shopping result, opens the sidebar, and extracts product name, reviews, ratings, prices, and store links.
- Generates the CSS/JSON extraction schema once with GPT‑4.1‑nano, caches it, and reuses it to minimize token usage.
- Interactive CLI prompts for a query, launches a headless browser, and saves JSON results into a `scrapes/` directory.

<div id="loom-web-crawler" class="modal-overlay" role="dialog" aria-modal="true" aria-labelledby="loom-web-crawler-title">
  <div class="modal-content">
    <button class="modal-close" type="button" aria-label="Close">×</button>
    <h4 id="loom-web-crawler-title">Google Shopping Web Scraper Demo</h4>
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
  <h3>💬 Intelligent Slack Agent for Document Processing &amp; Summarization</h3>
  <div class="project-links">
    <a href="https://github.com/ChiefVishPat/missing-contract-legal-agent" target="_blank" rel="noopener noreferrer">Source Code</a>
    <a href="#" class="open-modal" data-modal="loom-slack-agent">Demo Video</a>
  </div>
</div>

**Tech:** Python, Slack API, OpenAI GPT, GitHub API  

- Automates document intake by extracting and summarizing PDFs/DOCX/TXT with OpenAI GPT models.
- Dynamic prompt switching tailors summaries to user context, improving accuracy and usefulness.
- Async file handling and Slack messaging produce readable, well-formatted summaries.
- Auto-creates GitHub issues for follow-ups; modular design supports other ticketing systems.

<div id="loom-slack-agent" class="modal-overlay" role="dialog" aria-modal="true" aria-labelledby="loom-slack-agent-title">
  <div class="modal-content">
    <button class="modal-close" type="button" aria-label="Close">×</button>
    <h4 id="loom-slack-agent-title">Intelligent Slack Agent Demo</h4>
    <div class="modal-body">
      <div style="position: relative; padding-bottom: 64.5933014354067%; height: 0;">
        <iframe data-src="https://www.loom.com/embed/c7ac32dee35e47cb89f2a810589b3284" allowfullscreen></iframe>
      </div>
      <p class="modal-fallback">
        Prefer a new tab?
        <a href="https://www.loom.com/share/c7ac32dee35e47cb89f2a810589b3284" target="_blank" rel="noopener noreferrer">Watch on Loom</a>.
      </p>
    </div>
  </div>
</div>

---

<div class="project-heading">
  <h3>🗣️ Pharmaceutical Voice AI Assistant</h3>
  <div class="project-links">
    <a href="https://github.com/ChiefVishPat/pharmacist-voice-assistant" target="_blank" rel="noopener noreferrer">Source Code</a>
  </div>
</div>

**Tech:** Python, WebSockets, Asyncio, Deepgram, Twilio, OpenAI  

- Real-time voice pharmacy assistant that handles drug inquiries, orders, and tracking via natural phone conversations.
- Bidirectional streaming pipeline between Twilio MediaStreams and Deepgram’s Agent API.
- Intelligent barge-in detection and schema-validated function calls for accurate operations.

</section>

  <!-- RIGHT: Dynamic GitHub list -->
  <aside class="page-right">
    <h2>All Repositories</h2>
    <div class="repo-box">
      <div id="repo-list">Loading repositories...</div>
    </div>
  </aside>

</div>

<script>
  (function() {
    const modalTriggers = document.querySelectorAll('.open-modal');
    const modals = document.querySelectorAll('.modal-overlay');

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

    const username = "ChiefVishPat";
    const container = document.getElementById("repo-list");
    if (!container) return;

    fetch(`https://api.github.com/users/${username}/repos?per_page=100&sort=updated`)
      .then(res => res.json())
      .then(repos => {
        container.innerHTML = "";
        repos
          .filter(r => !r.fork)
          .forEach(r => {
            const div = document.createElement("div");
            div.className = "repo-item";
            const desc = r.description ? `<span> – ${r.description}</span>` : "";
            div.innerHTML = `<a href="${r.html_url}" target="_blank" rel="noopener noreferrer">${r.name}</a>${desc}`;
            container.appendChild(div);
          });
      })
      .catch(err => {
        const div = document.createElement("div");
        div.textContent = "Could not load repositories from GitHub.";
        container.appendChild(div);
        console.error(err);
      });
  })();
</script>
