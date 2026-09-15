<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/lucasamarale/lucasamarale/main/assets/header-dark.svg">
  <img alt="Lucas Amaral Evangelista. I build AI systems that ship." src="https://raw.githubusercontent.com/lucasamarale/lucasamarale/main/assets/header-light.svg" width="100%">
</picture>

<p align="center">
  <a href="https://lucasamarale.dev"><img src="https://img.shields.io/badge/lucasamarale.dev-B45309?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/lucasamarale"><img src="https://img.shields.io/badge/LinkedIn-4A3B33?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:lucasamarale.dev@gmail.com"><img src="https://img.shields.io/badge/Email-4A3B33?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
</p>

I build AI systems and put them in production. Python pipelines where Claude classifies and writes, a governed knowledge base an agent edits over MCP, a support chatbot shipped in 48 hours, and the engineering around them: tests, CI, circuit breakers, an outbox, a credential vault. I work daily with Claude (API, Claude Code, Skills, MCP), Codex, the Gemini API, Groq and LLaMA, Whisper and n8n, and I write the Python, TypeScript and vanilla web code that holds it together.

I am also the Partnerships & Channels Manager at **Life Link**, a technology company in Brasília: five global vendors, IBM among them, deployed and demoed by the same person who writes the automation around them. Computer Science at UniCEUB (2025-2028), with an exchange at BCIT in Vancouver and a year of high school in New Zealand.

The person who writes the pipelines also negotiates the contracts.

## AI systems in production

| System | What it does | Stack |
| --- | --- | --- |
| **Court Docket Monitor** *(private, for a law firm)* | Tracks around 200 court cases a day: queries the DataJud API and higher courts, detects new activity by SHA-256 hash, classifies it with Claude and notifies through WhatsApp, email and Google Sheets. Circuit breakers per court, outbox pattern, credential vault, 150+ pytest cases, CI on GitHub Actions. | `Python` `Claude API` `pytest` `GitHub Actions` |
| **[nola AI](https://github.com/lucasamarale/nola-ai-chatbot)** | AI support chatbot for a restaurant-management SaaS: n8n orchestration, Groq and LLaMA inference over a CSV knowledge base, web front end. Zero to production in 48 hours. | `n8n` `Groq` `LLaMA` `Python` |
| **Lucas Brain** | Obsidian vault with a written constitution: typed frontmatter, controlled vocabulary, read-only and write zones. Claude works inside it over MCP servers with real read and write access, and custom Claude Skills turn meetings into filed notes and branded PDF minutes. | `Claude` `MCP` `Claude Skills` `Python` |
| **Meeting pipeline** | Recordings enter through a LaunchAgent, Whisper transcribes, Claude classifies and links, and the note lands in the vault typed and filed before I open it. | `Whisper` `Claude` `Python` `SQLite` |
| **[task-manager-extension](https://github.com/lucasamarale/task-manager-extension)** | Chrome extension (Manifest V3) with AI task suggestions through the Gemini API and one-click save to Google Calendar. TypeScript, tests and CI. | `TypeScript` `Gemini API` `GitHub Actions` |
| **[SUS transfer corrections](https://github.com/lucasamarale/Correcoes-repasses)** | Monetary correction of SUS transfers to hospitals: CSV in, pandas processing, PDF reports and dashboards out. | `Python` `pandas` |
| **Document generator** | Python and Playwright generate branded documents, with a pre-flight verifier that aborts the build on any violation of the visual standard. | `Python` `Playwright` |
| **SharePoint tenant** | Nine corporate sites with defined taxonomy, plus automated writes through the REST API instead of manual upkeep. | `SharePoint` `REST` |
| **[lucasamarale.dev](https://lucasamarale.dev)** | This portfolio: one vanilla HTML file with a scroll-locked 3D intro, canvas engines and a bilingual build. No frameworks, no build step, deployed on Netlify. | `HTML` `CSS` `JS` |

## Stack

**AI and agents** ![Claude](https://img.shields.io/badge/Claude-B45309?style=flat-square&logo=anthropic&logoColor=white) ![Claude Code](https://img.shields.io/badge/Claude_Code-B45309?style=flat-square&logo=anthropic&logoColor=white) ![MCP](https://img.shields.io/badge/MCP-B45309?style=flat-square&logo=modelcontextprotocol&logoColor=white) ![Codex](https://img.shields.io/badge/Codex-B45309?style=flat-square&logo=openai&logoColor=white) ![Gemini API](https://img.shields.io/badge/Gemini_API-B45309?style=flat-square&logo=googlegemini&logoColor=white) ![Groq](https://img.shields.io/badge/Groq-B45309?style=flat-square) ![LLaMA](https://img.shields.io/badge/LLaMA-B45309?style=flat-square) ![Whisper](https://img.shields.io/badge/Whisper-B45309?style=flat-square&logo=openai&logoColor=white) ![n8n](https://img.shields.io/badge/n8n-B45309?style=flat-square&logo=n8n&logoColor=white) ![Obsidian](https://img.shields.io/badge/Obsidian-B45309?style=flat-square&logo=obsidian&logoColor=white)

**Languages** ![Python](https://img.shields.io/badge/Python-4A3B33?style=flat-square&logo=python&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-4A3B33?style=flat-square&logo=typescript&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-4A3B33?style=flat-square&logo=javascript&logoColor=white) ![PHP](https://img.shields.io/badge/PHP-4A3B33?style=flat-square&logo=php&logoColor=white) ![Java](https://img.shields.io/badge/Java-4A3B33?style=flat-square&logo=openjdk&logoColor=white) ![HTML5](https://img.shields.io/badge/HTML5-4A3B33?style=flat-square&logo=html5&logoColor=white) ![CSS](https://img.shields.io/badge/CSS-4A3B33?style=flat-square&logo=css&logoColor=white)

**Engineering** ![React](https://img.shields.io/badge/React-4A3B33?style=flat-square&logo=react&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-4A3B33?style=flat-square&logo=pandas&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-4A3B33?style=flat-square&logo=sqlite&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4A3B33?style=flat-square&logo=mysql&logoColor=white) ![pytest](https://img.shields.io/badge/pytest-4A3B33?style=flat-square&logo=pytest&logoColor=white) ![Playwright](https://img.shields.io/badge/Playwright-4A3B33?style=flat-square&logo=playwright&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-4A3B33?style=flat-square&logo=githubactions&logoColor=white) ![SharePoint](https://img.shields.io/badge/SharePoint-4A3B33?style=flat-square&logo=microsoftsharepoint&logoColor=white) ![Netlify](https://img.shields.io/badge/Netlify-4A3B33?style=flat-square&logo=netlify&logoColor=white)

## The business side

At Life Link I am the single point of contact for five global technology vendors, IBM among them. I run channel enablement end to end, deploy and demo the products myself, sit between Sangfor's SOC and the client on the MDR service, analyze international channel agreements clause by clause, and handle the technical analysis of public tenders above R$ 1 million under Brazilian procurement law 14.133/2021.

## Open source and coursework

- **[fincontrol](https://github.com/lucasamarale/fincontrol)** · Personal finance app in React 18: budgets with alerts, filtered statements, CSV export. Runs fully offline in the browser.
- **[gym-management-system](https://github.com/lucasamarale/gym-management-system)** · Gym management system in PHP and SQLite: REST API over five entities, Chart.js dashboard, PDF reports with FPDF. University systems-development project.
- **[task-manager-extension](https://github.com/lucasamarale/task-manager-extension)** · Chrome extension with Gemini API suggestions, Docker and CI on GitHub Actions.
- **[CEUB](https://github.com/lucasamarale/CEUB)** · Computer Science coursework, organized by discipline and delivery.

## Activity

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=lucasamarale&hide_border=true&background=1B1410&ring=F4AC4A&fire=F4AC4A&currStreakLabel=F4AC4A&currStreakNum=F3ECE2&sideNums=F3ECE2&sideLabels=B8A899&dates=B8A899">
  <img src="https://streak-stats.demolab.com?user=lucasamarale&hide_border=true&background=FDFBF7&ring=B45309&fire=B45309&currStreakLabel=B45309&currStreakNum=4A3B33&sideNums=4A3B33&sideLabels=7A6A60&dates=7A6A60" alt="GitHub streak" height="170">
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
| Advanced English Diploma | Casa Thomas Jefferson | 2010-2019 |

<p>
  <a href="https://www.credly.com/badges/cffb9ac8-8135-4d47-a21e-4d66c181be23"><img src="https://images.credly.com/size/220x220/images/289f631b-8cce-4115-8da1-75780c54fab7/blob" width="88" alt="IBM Instana Sales Foundation"></a>
  <a href="https://www.credly.com/badges/63158500-a67c-4fb4-bc36-0b61ef22b4e1"><img src="https://images.credly.com/size/220x220/images/faf29d25-5f48-47d9-af7f-6c6427312821/blob" width="88" alt="IBM Instana Intermediate"></a>
</p>

## Contact

One email, no forms: **lucasamarale.dev@gmail.com** · [lucasamarale.dev](https://lucasamarale.dev) · [LinkedIn](https://www.linkedin.com/in/lucasamarale)
