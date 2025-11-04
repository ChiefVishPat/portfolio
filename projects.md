---
layout: default
title: Projects
permalink: /projects
---

# Projects

A few projects that represent how I like to build: practical, reliable, and focused on real workflows.

---

## Interactive Story Generator – Full-stack AI Storytelling Engine

**Tech:** TypeScript, React, FastAPI, PostgreSQL, OpenAI, LangChain, SQLAlchemy, Vite  

Built an LLM-powered “choose your own adventure” engine from scratch.

- Users input a theme and receive a playable branching narrative with multiple endings.
- Recursive story-tree processing and async job queues to generate and store story branches.
- LangChain + Pydantic pipeline to validate deeply nested JSON into structured DB rows.

**Code:** [GitHub](https://github.com/ChiefVishPat/your-repo-here)  
**Live Demo:** [App](https://dd4da2b8-8671-4d7c-9aa9-41425b5926a6.e1-us-east-azure.choreoapps.dev/)  

---

## Google Shopping Web Scraper using Crawl4AI

**Tech:** Python, Crawl4AI, Playwright, Pydantic, OpenAI, uv  

- AI-assisted crawler that traverses Google Shopping results and extracts structured product data.
- GPT-generated CSS/JSON extraction schema cached to disk to minimize token usage.
- Interactive CLI prompts for search terms, launches a headless browser, and saves JSON results to `scrapes/`.

**Code:** [GitHub](https://github.com/ChiefVishPat/web_crawler)  
**Video Demo:** [Loom](https://www.loom.com/share/d87f88f6918a48b2b121e1afcc40b761)

---

## 🧾 Expense Policy Agent – AI-Powered Email Automation

**Tech:** Python, LangGraph, PydanticAI, FastAPI, Redis, Gmail API, OpenAI  

Built an AI agent that automates AP/AR inboxes in real time by classifying incoming vendor and expense-related emails, fetching matching receipts or invoices, and drafting accurate replies.

- Designed a robust orchestration layer (LangGraph + PydanticAI) for multi-step intent detection and validation.  
- Integrated Gmail API with Redis-backed queues for async message handling and error retries.  
- Created a modular architecture for plug-and-play business workflows (invoice lookup, promise-to-pay, validation checks).  
- Demonstrated reliability across thousands of automated email actions.

**Code:** [GitHub](https://github.com/ChiefVishPat/expense-policy-agent)  
**Video Demo:** [Loom](https://www.loom.com/share/454f7f5716c94de4b64474612a10660d)

--

## Intelligent Slack Agent for Document Processing & Summarization

**Tech:** Python, Slack API, OpenAI GPT, GitHub API  

- Slack agent that ingests PDFs/DOCX/TXT, summarizes them with GPT, and posts readable summaries back to Slack.
- Dynamic prompt switching to tailor summaries by team/context.
- Async file handling and GitHub issue creation for follow-ups and collaboration.

**Code:** [GitHub](https://github.com/ChiefVishPat/missing-contract-legal-agent)  
**Video Demo:** [Loom](https://www.loom.com/share/c7ac32dee35e47cb89f2a810589b3284)
