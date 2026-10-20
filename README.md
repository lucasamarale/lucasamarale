<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/lucasamarale/lucasamarale/main/assets/header-dark.svg">
  <img alt="Lucas Amaral Evangelista, Software Engineer and AI Engineer. I build systems that ship." src="https://raw.githubusercontent.com/lucasamarale/lucasamarale/main/assets/header-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://lucasamarale.dev"><img src="https://img.shields.io/badge/lucasamarale.dev-B45309?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/lucasamarale"><img src="https://img.shields.io/badge/LinkedIn-4A3B33?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:lucasamarale.dev@gmail.com"><img src="https://img.shields.io/badge/Email-4A3B33?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

I'm a software engineer and an AI engineer. I build whole products: mobile and web apps in React Native, React and TypeScript, APIs and data pipelines in Python and Node.js, PostgreSQL underneath, and the parts people skip when they're in a hurry: tests, CI, containers, error handling, retries and circuit breakers, and a rollback that works.

**AI is where I go deepest.** I don't just call a model, I engineer around it. I designed and run my own multi-agent development orchestra: a planner, an executor in a network-free sandbox, and a rival model from a different provider that attacks every plan and every diff before merge, all behind a risk gate wired into the agents' hooks. Around that: context engineering, structured outputs, tool calling, MCP servers with real read and write access, retrieval over governed knowledge bases, transcription and classification chains, and the evaluation and guardrails that let a pipeline run unattended. Claude Code, Codex, Claude Skills, the Gemini API, Groq and LLaMA, Whisper and n8n are the tools. The engineering around them is what makes them production.

I'm also the founder of **[Casaly](https://getcasaly.com)**, a wedding planning app for iOS, Android and web, and the Partnerships & Channels Manager at **Life Link**, a technology company in Brasília, where I work with seven global vendors, IBM, Sangfor and Perforce among them. Computer Science at UniCEUB (2025 to 2028), with an exchange at BCIT in Vancouver and a semester of high school in New Zealand.

The person who writes the pipelines is the one who negotiates the contracts.

## What I'm building

| Project | What it is | Stack |
| --- | --- | --- |
| **AI agent orchestra** *(private)* | A reusable formation of agents for building software, in use across three projects and running on more than one ADE (Maestri and Elyra). The Maestro plans; the Executor builds in an isolated worktree inside a network-free sandbox that's re-proven on every Claude Code release; the Rival, from a different provider, attacks the plan until it converges and reviews the diff; subagents handle testing, security audit and deploy. A Node.js risk gate in the Claude Code and Codex hooks blocks destructive commands (488 test cases). Context lives in files, not in the session. I decide premises, plan, diff and merge. | `Claude Code` `Codex CLI` `Node.js` `Bash` `GitHub Actions` |
| **[Casaly](https://getcasaly.com)** *(founder, private repo)* | Wedding planning SaaS for iOS, Android and web: a quiz-generated plan, quantities sized by guest count, an offline queue and three languages from day one. Supabase with row-level access, subscriptions through App Store Connect and RevenueCat, and every PR tested on an iPhone before merge. Built with my own code and the agent orchestra. | `Expo` `React Native` `TypeScript` `Supabase` `RevenueCat` |
| **Court Docket Monitor, v2** *(private)* | My own TypeScript SaaS, rebuilt from the Python system below. Legal deadline counting under Brazil's Civil Procedure Code in auditable code (the model reads the text, the code counts the days), PostgreSQL with per-firm isolation, a DataJud adapter with network-free tests, and 298 tests so far. | `TypeScript` `PostgreSQL` `Kysely` `Vitest` `pnpm` |
| **[sdd-task-analyzer](https://github.com/lucasamarale/sdd-task-analyzer)** | A spec-driven workflow for AI-generated code: a versioned contract, context rules for the agent, 26 pytest tests written before the code and human sign-off on every PR, with CI on GitHub Actions and in Docker. I injected nine typical AI mistakes: tests caught seven, and the gap became a contract change and a new test. | `Python` `pytest` `Docker` `GitHub Actions` |
| **Internal CRM front end** *(Life Link)* | React 19 and Vite front end for an internal B2G CRM over a Rails API: a design system built on IBM Carbon, a demo mode covering all 141 API calls, roles and permissions. Built by the agent orchestra through reviewed PRs. | `React` `Vite` `TypeScript` `IBM Carbon` |

## Systems in production

| System | What it does | Stack |
| --- | --- | --- |
| **Court Docket Monitor** *(private, for a law firm)* | Tracks around 200 court cases a day: queries the DataJud API and higher courts, detects new activity by SHA-256 hash, classifies it with an LLM and notifies through WhatsApp, email and Google Calendar. Circuit breaker per court, outbox pattern, credential vault, LGPD policy, 205 pytest cases, CI on GitHub Actions. | `Python` `Claude API` `pytest` `GitHub Actions` |
| **Lucas Brain** | Knowledge base with a written constitution: typed frontmatter, controlled vocabulary, read-only and write zones enforced on the agent. Claude works inside it through MCP servers with real read and write access, and custom Skills distil meetings into filed notes and branded PDF minutes, aborting when the visual standard is violated. | `MCP` `Claude Skills` `Python` `Obsidian` |
| **Meeting pipeline** | Meetings are captured and exported to the vault on their own. A custom Skill asks the open questions before writing a word, cross-checks a second transcript, files decisions, tasks and people, and renders branded PDF minutes. | `Claude Skills` `Python` `WeasyPrint` `Obsidian` |
| **[nola AI](https://github.com/lucasamarale/nola-ai-chatbot)** | AI support chatbot for a restaurant-management SaaS: n8n orchestration, Groq and LLaMA inference over a curated knowledge base, web front end. Zero to production in 48 hours. | `n8n` `Groq` `LLaMA` `Python` |
| **[task-manager-extension](https://github.com/lucasamarale/task-manager-extension)** | Chrome extension (Manifest V3) with AI task suggestions through the Gemini API and one-click save to Google Calendar. TypeScript, Docker, tests and CI. | `TypeScript` `Gemini API` `Docker` |
| **[SUS transfer corrections](https://github.com/lucasamarale/Correcoes-repasses)** | Monetary correction of public health transfers to hospitals: CSV in, pandas processing, PDF reports and dashboards out. | `Python` `pandas` |
| **Document generator** | Python and Playwright generate branded documents, with a pre-flight verifier that aborts the build on any violation of the visual standard. | `Python` `Playwright` |
| **SharePoint tenant** | Nine corporate sites with a defined taxonomy, plus automated writes through the REST API instead of manual upkeep. | `SharePoint` `REST` |
| **[lucasamarale.dev](https://lucasamarale.dev)** | This portfolio: one vanilla HTML file with a scroll-locked 3D intro, canvas engines and a bilingual build. No frameworks, no build step, deployed on Netlify. | `HTML` `CSS` `JS` |

## Engineering

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![SQL](https://img.shields.io/badge/SQL-336791?style=flat-square) ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white) ![CSS](https://img.shields.io/badge/CSS-663399?style=flat-square&logo=css&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Frameworks and data**

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white) ![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![REST APIs](https://img.shields.io/badge/REST_APIs-6E4A2F?style=flat-square) ![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat-square&logo=chartdotjs&logoColor=white)

**Testing, delivery and infra**

![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white) ![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white) ![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square) ![Ruff](https://img.shields.io/badge/Ruff-D7FF64?style=flat-square&logo=ruff&logoColor=black) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) ![Cloudflare Pages](https://img.shields.io/badge/Cloudflare_Pages-F38020?style=flat-square&logo=cloudflarepages&logoColor=white) ![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=flat-square&logo=netlify&logoColor=white) ![App Store Connect](https://img.shields.io/badge/App_Store_Connect-0D96F6?style=flat-square&logo=appstore&logoColor=white) ![SharePoint](https://img.shields.io/badge/SharePoint-0078D4?style=flat-square)

## AI engineering

Multi-agent orchestration · cross-provider review · risk gates and sandboxing for agents · spec-driven development for AI-generated code · prompt and context engineering · structured outputs · tool and function calling · MCP servers · retrieval over governed knowledge bases · parallel subagents for long documents · transcription and classification chains · cost and latency budgets · evaluation, guardrails and human review gates

![Claude](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white) ![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white) ![Claude Skills](https://img.shields.io/badge/Claude_Skills-D97757?style=flat-square&logo=anthropic&logoColor=white) ![MCP](https://img.shields.io/badge/MCP-454545?style=flat-square&logo=modelcontextprotocol&logoColor=white) ![Codex](https://img.shields.io/badge/Codex-412991?style=flat-square) ![Maestri](https://img.shields.io/badge/Maestri-4A3B33?style=flat-square) ![Elyra](https://img.shields.io/badge/Elyra-4A3B33?style=flat-square) ![Gemini API](https://img.shields.io/badge/Gemini_API-8E75B2?style=flat-square&logo=googlegemini&logoColor=white) ![Groq](https://img.shields.io/badge/Groq-F55036?style=flat-square) ![LLaMA](https://img.shields.io/badge/LLaMA-0866FF?style=flat-square) ![Whisper](https://img.shields.io/badge/Whisper-412991?style=flat-square) ![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white) ![Obsidian](https://img.shields.io/badge/Obsidian-7C3AED?style=flat-square&logo=obsidian&logoColor=white)

## The business side

At Life Link I'm the single point of contact for seven technology vendors, IBM, Sangfor, Perforce, Hyperflow, Singular GovTech, Safiatech and GoLedger, and for the distributors behind them. I run channel enablement end to end, deploy and demo the products myself, sit between Sangfor's SOC and the client on the MDR service, and review international channel agreements clause by clause. On public tenders under Brazilian procurement law 14.133/2021, I've read a 4,500+ line software tender end to end with parallel AI subagents and item-by-item human review, and turned it into a portfolio fit matrix and a 17-page bid plan.

## Open source and coursework

- **[sdd-task-analyzer](https://github.com/lucasamarale/sdd-task-analyzer)** · Spec-driven development for AI-generated code: contract, test-first harness, human sign-off, CI and Docker. Tagged releases.
- **DevOps Market** *(class repository)* · Order history module for a Flask and SQLAlchemy store: filtering and sorting with 30 pytest tests and a three-stage GitHub Actions pipeline (Ruff, pytest, build). Also diagnosed and reported a core bug in the shared codebase, with root cause and a tested fix.
- **[fincontrol](https://github.com/lucasamarale/fincontrol)** · Personal finance app in React 18: budgets with alerts, filtered statements, CSV export. Runs fully offline in the browser.
- **[gym-management-system](https://github.com/lucasamarale/gym-management-system)** · Gym management system in PHP and SQLite: REST API over five entities, Chart.js dashboard, PDF reports with FPDF.
- **[task-manager-extension](https://github.com/lucasamarale/task-manager-extension)** · Chrome extension with Gemini API suggestions, Docker and CI on GitHub Actions.
- **[CEUB](https://github.com/lucasamarale/CEUB)** · Computer Science coursework, organized by discipline and delivery.

## Activity

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=lucasamarale&hide_border=true&disable_animations=true&background=1B1410&ring=F4AC4A&fire=F4AC4A&currStreakLabel=F4AC4A&currStreakNum=F3ECE2&sideNums=F3ECE2&sideLabels=B8A899&dates=B8A899">
  <img src="https://streak-stats.demolab.com?user=lucasamarale&hide_border=true&disable_animations=true&background=FDFBF7&ring=B45309&fire=B45309&currStreakLabel=B45309&currStreakNum=4A3B33&sideNums=4A3B33&sideLabels=7A6A60&dates=7A6A60" alt="GitHub streak" height="170">
</picture>

## Certifications

| Certificate | Issuer | Year |
| --- | --- | --- |
| Generative AI Explained | NVIDIA Deep Learning Institute | 2026 |
| Responsible Prompting (AI) | Santander Open Academy | 2026 |
| Instana Intermediate | IBM | 2026 |
| Instana Sales Foundation | IBM | 2026 |
| Networking Basics | Cisco Networking Academy | 2026 |
| Python | Versátil, Tecnologia em Informação | 2024 |
| IELTS Academic | British Council | 2022 |
| Advanced English Diploma | Casa Thomas Jefferson | 2010 to 2019 |

<p>
  <a href="https://www.credly.com/badges/cffb9ac8-8135-4d47-a21e-4d66c181be23"><img src="https://images.credly.com/size/220x220/images/289f631b-8cce-4115-8da1-75780c54fab7/blob" width="88" alt="IBM Instana Sales Foundation"></a>
  <a href="https://www.credly.com/badges/63158500-a67c-4fb4-bc36-0b61ef22b4e1"><img src="https://images.credly.com/size/220x220/images/faf29d25-5f48-47d9-af7f-6c6427312821/blob" width="88" alt="IBM Instana Intermediate"></a>
</p>

## Contact

One email, no forms: **lucasamarale.dev@gmail.com** · [lucasamarale.dev](https://lucasamarale.dev) · [LinkedIn](https://www.linkedin.com/in/lucasamarale)
