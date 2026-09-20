
<!-- ═══════════════════════════════════════════════════════════════════════ -->
<!--                     ENGINEERING LOG — SANJAY G. M.                    -->
<!-- ═══════════════════════════════════════════════════════════════════════ -->

<div align="center">

```
╔══════════════════════════════════════════════════════════════╗
║                                                              ║
║   SANJAY  G. M.                                              ║
║   Software Engineer  ·  SDE                                  ║
║                                                              ║
║   Building — AI systems · Backend services · Developer tools ║
║                                                              ║
╚══════════════════════════════════════════════════════════════╝
```

I build backend services, full-stack applications, and AI-powered developer tools — focused on solving practical engineering problems.

[![GitHub](https://img.shields.io/badge/GitHub-gms26-181717?style=flat&logo=github)](https://github.com/gms26)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin)](YOUR_LINKEDIN_URL)
[![LeetCode](https://img.shields.io/badge/LeetCode-500%2B_Solved-FFA116?style=flat&logo=leetcode&logoColor=white)](YOUR_LEETCODE_URL)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-4285F4?style=flat&logo=googlechrome&logoColor=white)](YOUR_PORTFOLIO_URL)

</div>

---

## ⚙️ System Status

```
 ┌─────────────────────────────────────────────────────┐
 │  [ BUILDING  ]  AI GitHub Pull Request Reviewer     │
 │  [ SOLVED   ]  500+ DSA Problems on LeetCode        │
 │  [ LEARNING ]  System Design · Cloud · DevOps       │
 │  [ EXPLORING]  Distributed Systems · AI Infra       │
 └─────────────────────────────────────────────────────┘
```

---

## 🛠️ Engineering Stack

| Layer | Technologies |
|-------|-------------|
| **Languages** | `Java` · `JavaScript` · `Python`  |
| **Backend** | `Spring Boot` · `Node.js` · `Express.js` · `REST APIs` |
| **Frontend** | `React` · `Vite` · `HTML` · `CSS` |
| **Databases** | `PostgreSQL` · `MongoDB` · `Supabase` |
| **AI / LLM** | `Google Gemini` · `LLM API Integration` · `AI App Development` |
| **Tools** | `Git` · `GitHub` · `Docker` |
| **Exploring** | `System Design` · `Cloud` · `DevOps` · `Distributed Systems` |

---

## 🏗️ Flagship System — AI GitHub Pull Request Reviewer

> An automated code review system that analyzes pull request diffs using AI and posts structured review comments directly on GitHub.

**This is not a wrapper around an AI API.** It's a complete engineering system with authentication, webhook infrastructure, external API integration, and structured response handling.

```
┌──────────────────────────────────────────────────────────────────┐
│                        SYSTEM ARCHITECTURE                       │
├──────────────────────────────────────────────────────────────────┤
│                                                                  │
│   Developer creates Pull Request                                 │
│         │                                                        │
│         ▼                                                        │
│   GitHub Webhook ──► Spring Boot Backend                         │
│                          │                                       │
│                          ├──► Webhook Signature Verification     │
│                          │        (HMAC validation)              │
│                          │                                       │
│                          ├──► GitHub API                         │
│                          │        Fetch PR Diff + Context        │
│                          │        (with pagination handling)     │
│                          │                                       │
│                          ├──► Context Builder                    │
│                          │                                       │
│                          ├──► Gemini API                         │
│                          │        Structured Review JSON         │
│                          │                                       │
│                          ├──► Parse + Validate Response          │
│                          │        (fail-safe: skip on bad parse) │
│                          │                                       │
│                          └──► GitHub API                         │
│                                  Post Review Comments on PR      │
│                                                                  │
└──────────────────────────────────────────────────────────────────┘
```

**Engineering depth:**

- **Auth:** GitHub OAuth2 authentication, repository ownership validation
- **Webhooks:** Webhook registration, HMAC signature verification, state tracking (`webhookEnabled` + `webhookId`)
- **APIs:** GitHub REST API integration with pagination, Gemini API with structured output
- **Data:** PostgreSQL persistence, Flyway migrations, Spring Data JPA
- **Resilience:** Retry mechanisms, error handling, external API resilience — if Gemini returns an unrecoverable response, the system logs and skips rather than posting garbage
- **Stack:** Java · Spring Boot · Spring Security · Actuator

<p>
  <a href="https://github.com/gms26/PR-Reviewer">
    <img src="https://img.shields.io/badge/→_View_Repository-PR--Reviewer-2ea44f?style=for-the-badge" alt="PR Reviewer Repo" />
  </a>
</p>

---

## 📦 Selected Builds

### SmartForecast AI
> **Problem:** Time-series data is hard to understand without the right forecasting model.  
> **Solution:** A dashboard that lets users upload CSV data, compare forecasting models (Moving Average, ARIMA, Holt-Winters), and get AI-generated explanations.

`React` · `Vite` · `Node.js` · `Express.js` · `Recharts` · `AI APIs`

**Key features:** CSV upload → data visualization → model comparison → forecast rendering → AI explanations

[![Repository](https://img.shields.io/badge/Repository-Forcasting-blue?style=flat&logo=github)](https://github.com/gms26/Forcasting)

---

### Smart Code Translator
> **Problem:** Developers often need to translate code across languages quickly.  
> **Solution:** An AI-powered code translation platform with Monaco Editor, Google OAuth, and real-time translation via Gemini.

`React` · `Vite` · `Node.js` · `Google Gemini` · `Google OAuth`

**Key features:** Code editor with syntax highlighting → AI-powered translation → authentication → backend API integration

[![Repository](https://img.shields.io/badge/Repository-Smart--Code--Translator-blue?style=flat&logo=github)](https://github.com/gms26/Smart-Code-Translator)

---

### CivicPulse
> **Problem:** Citizens lack a structured way to report infrastructure issues (road damage, water leakage, street-light failures).  
> **Solution:** A civic issue reporting platform with image-based reporting, issue classification, priority assignment, and authority notification.

`React` · `Node.js` · `Express.js` · `MongoDB`

**Key features:** Issue submission with photos → classification & prioritization → authority routing → issue tracking

[![Repository](https://img.shields.io/badge/Repository-CivicPulse-blue?style=flat&logo=github)](https://github.com/gms26/CivicPulse)

---

### FarmEquipConnect
> **Problem:** Farmers need accessible, affordable equipment without ownership costs.  
> **Solution:** An agricultural equipment rental platform with equipment discovery, rental workflow, and backend APIs.

**Key features:** Full-stack application → equipment catalog → rental management → database integration

[![Repository](https://img.shields.io/badge/Repository-FarmEquipConnect-blue?style=flat&logo=github)](https://github.com/gms26/FarmEquipConnect)

---

### Personal Portfolio
> A portfolio with sections for About, Skills, Projects, Achievements, Certificates, Resume, Contact — with admin functionality for content management.

`React / Next.js` · `JavaScript` · `Node.js` · `Express.js` · `MongoDB / PostgreSQL` · `Cloudinary`

[![Repository](https://img.shields.io/badge/Repository-Smart__portfolio-blue?style=flat&logo=github)](https://github.com/gms26/Smart_portfolio)

---

## 🧠 Problem Solving — 500+ LeetCode Problems

```
 ┌───────────────────────────────────────────────────────────┐
 │  TOPIC COVERAGE                                           │
 ├───────────────────────────────────────────────────────────┤
 │                                                           │
 │  Arrays ████████████  Strings █████████                   │
 │  Hashing ████████     Two Pointers ████████               │
 │  Sliding Window ████  Binary Search ███████               │
 │  Linked Lists ██████  Stack / Queue ██████                │
 │  Trees ████████████   Graphs ████████                     │
 │  Recursion ████████   Backtracking ██████                 │
 │  Dynamic Prog ██████  Greedy █████████                    │
 │                                                           │
 └───────────────────────────────────────────────────────────┘
```

Consistent daily practice. No shortcuts.

[![DSA Repository](https://img.shields.io/badge/Repository-DSA-blue?style=flat&logo=github)](https://github.com/gms26/DSA)
[![LeetCode](https://img.shields.io/badge/LeetCode-Profile-FFA116?style=flat&logo=leetcode&logoColor=white)](YOUR_LEETCODE_URL)

---

## 🔬 How I Think

```
Problem → Understand → Design → Implement → Test → Measure → Improve
                ↑                                          │
                └──────────────────────────────────────────┘
```

I start by understanding the problem deeply before writing any code. Design comes before implementation. Testing and measurement feed back into better design. Every iteration should produce something measurably better, not just different.

---

## 🧭 Engineering Philosophy

> **Build → Break → Understand → Improve**

Write it. Break it on purpose. Understand *why* it broke. Then build it better. Good engineering comes from understanding failure modes, not just the happy path.

---

## 📚 Education & Experience

**B.Tech — Information Technology**  
Dr. N.G.P. Institute of Technology, Coimbatore · CGPA: 7.74 · Class of 2027

**AI Intern — Gateway Software Solutions**  
Crop suitability prediction · AI/LLM API integration · Backend/application development

**Achievements:**
- 500+ LeetCode problems solved
- NPTEL IoT course completion
- State-level Buildathon participation
- Multiple full-stack and AI projects shipped

---

## 📡 Currently

```
 Building   →  AI GitHub Pull Request Reviewer
 Learning   →  System Design · Cloud · DevOps · Distributed Systems
 Solving    →  Data Structures & Algorithms (daily)
```

---

## 🔗 Connect

| Platform | Link |
|----------|------|
| **GitHub** | [github.com/gms26](https://github.com/gms26) |
| **LinkedIn** | [YOUR_LINKEDIN_URL](YOUR_LINKEDIN_URL) |
| **LeetCode** | [YOUR_LEETCODE_URL](YOUR_LEETCODE_URL) |
| **Portfolio** | [YOUR_PORTFOLIO_URL](YOUR_PORTFOLIO_URL) |
| **Email** | YOUR_EMAIL |

---

<div align="center">

```
└─ EOF ─ Engineering Log ─ Sanjay G. M. ─ gms26 ─┘
```

<!-- 
  This README is an engineering document, not a template.
  Every section exists because it communicates something useful.
-->

</div>
