---
layout: default
title: Vishal Patel
---

<!-- Icon styles: Font Awesome + Devicon -->
<link rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"
      integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA=="
      crossorigin="anonymous" referrerpolicy="no-referrer" />
<link rel="stylesheet"
      href="https://cdn.jsdelivr.net/gh/devicons/devicon@v2.15.1/devicon.min.css" />

<style>
  /* Hide the default “View the Project on GitHub” block for this repo */
  a[href^="https://github.com/ChiefVishPat/portfolio"],
  a[href^="https://github.com/ChiefVishPat/portfolio"] + ul {
    display: none !important;
  }

  /* Simple, centered profile block at the top of the page */
  .profile-card {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    align-items: center;
    margin-bottom: 1.75rem;
  }

  .profile-card img {
    border-radius: 50%;
    width: 110px;
    height: 110px;
    object-fit: cover;
  }

  .profile-card-main {
    min-width: 220px;
  }

  .profile-card .socials a {
    margin-right: 0.5rem;
    display: inline-block;
  }

  .profile-card .socials img {
    vertical-align: middle;
  }

  .tech-icons i {
    font-size: 1.5rem;
    margin-right: 0.4rem;
    vertical-align: middle;
  }
</style>

<div class="profile-card">
  <img src="{{ site.baseurl }}/assets/pfp.jpeg" alt="Vishal Patel profile picture" />

  <div class="profile-card-main">
    <strong>Vishal Patel</strong><br />
    Software engineer specializing in backend systems, but open to all types of engineering roles. Adaptable, determined builder, hungry to learn and ship products that actually move the needle.

    <div class="socials" style="margin-top:0.6rem;">
      <!-- GitHub via Simple Icons CDN -->
      <a href="https://github.com/ChiefVishPat"
         target="_blank" rel="noopener noreferrer" aria-label="GitHub">
        <img src="https://cdn.simpleicons.org/github/ffffff"
             width="24" height="24" alt="GitHub" />
      </a>

      <!-- LinkedIn via Simple Icons CDN -->
      <a href="https://www.linkedin.com/in/vishalpatel2003"
         target="_blank" rel="noopener noreferrer" aria-label="LinkedIn">
        <img src="https://cdn.simpleicons.org/linkedin/0A66C2"
             width="24" height="24" alt="LinkedIn" />
      </a>

      <!-- Resume icon (PDF) -->
      <a href="{{ site.baseurl }}/vishal-patel-resume.pdf"
         target="_blank" rel="noopener noreferrer" aria-label="Resume PDF">
        <i class="fa-solid fa-file-pdf"></i>
      </a>
    </div>

    <div class="tech-icons" style="margin-top:0.4rem;">
      <!-- Tech stack with Devicon -->
      <i class="devicon-python-plain colored" title="Python"></i>
      <i class="devicon-postgresql-plain colored" title="PostgreSQL"></i>
      <i class="devicon-fastapi-plain colored" title="FastAPI"></i>
      <i class="devicon-react-original colored" title="React"></i>
      <i class="devicon-typescript-plain colored" title="TypeScript"></i>
      <i class="devicon-git-plain colored" title="Git"></i>
    </div>
  </div>
</div>

# Vishal Patel

**Software Engineer – AI, Fintech, and Backend Systems**  
Based in Clifton, NJ · Python, SQL, LangChain/LangGraph, FastAPI, TypeScript/React

[Download Resume]({{ site.baseurl }}/vishal-patel-resume.pdf){:target="_blank" rel="noopener noreferrer"}

---

## About

I'm a software engineer focused on building reliable backend systems and AI-powered workflows for real-world finance and operations use cases. I specialize in backend engineering, but I’m open to all kinds of engineering roles because I’m an adaptable, determined builder who enjoys learning quickly and shipping impactful products.

I am a **U.S. citizen and do not require visa sponsorship**.

Recently, I’ve:

- Contracted at **Ramp**, shipping backend receipt integrations used by major merchants like United Airlines, Delta Airlines, and Walmart.
- Built AI-driven agents that automate inboxes, document workflows, and data extraction.

I enjoy working close to the product: understanding real customer pain points, then building systems that are observable, resilient, and easy to iterate on.

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
- Helped drive rollout from internal launch → alpha → beta → GA, improving the receipt experience for thousands of users with ~87% success across shipped integrations.

---

## Projects

Here are a few selected projects. See more of my work on GitHub.

### Interactive Story Generator – Full-stack AI Storytelling Engine
**Tech:** TypeScript, React, FastAPI, PostgreSQL, OpenAI, LangChain, SQLAlchemy, Vite  

Built an LLM-powered “choose your own adventure” engine: users provide a theme, and the system generates a branching narrative with multiple endings and shareable URLs.

- Recursive story-tree processing and async job queues.
- LangChain + Pydantic pipeline to validate deeply nested JSON into structured DB rows.

**Code:** [GitHub](https://github.com/ChiefVishPat/interactive-story-generator){:target="_blank" rel="noopener noreferrer"}  
**Live Demo:** [App](https://dd4da2b8-8671-4d7c-9aa9-41425b5926a6.e1-us-east-azure.choreoapps.dev/){:target="_blank" rel="noopener noreferrer"}  

---

### Google Shopping Web Scraper using Crawl4AI
**Tech:** Python, Crawl4AI, Playwright, Pydantic, OpenAI, uv  

An AI-assisted crawler that clicks through Google Shopping results, opens sidebars, and extracts product data (name, reviews, ratings, prices, store links).

**Code:** [GitHub](https://github.com/ChiefVishPat/web_crawler){:target="_blank" rel="noopener noreferrer"}  
**Video Demo:** [Loom](https://www.loom.com/share/d87f88f6918a48b2b121e1afcc40b761){:target="_blank" rel="noopener noreferrer"}

---

[View all projects on GitHub →](https://github.com/ChiefVishPat?tab=repositories){:target="_blank" rel="noopener noreferrer"}
