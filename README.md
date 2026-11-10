<div align="center">

# Krishal Karna

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=1000&color=70A5FD&center=true&vCenter=true&width=620&lines=Backend+%2B+applied+ML+Engineer;Django+%C2%B7+DRF+%C2%B7+FastAPI+%C2%B7+PostgreSQL;scikit-learn+%C2%B7+LangGraph+%C2%B7+Gemini;Ships+the+frontend+too%2C+when+it+needs+shipping" alt="Backend + applied ML Engineer" />

**I build the backend and the model. Then I build the UI so people can actually use it.**

[Portfolio](https://krishalkarna.com.np) ·
[LinkedIn](https://www.linkedin.com/in/krishalkarna) ·
[Blog](https://completesql.hashnode.dev/series/learn-mysql) ·
[LeetCode](https://leetcode.com/u/kreeshal17/) ·
[karnakreeshal@gmail.com](mailto:karnakreeshal@gmail.com)

</div>

---

## About

Final-year CS student at Jain University, Bangalore — CGPA 9.5/10, graduating June 2027. Backend and applied ML is where I live. Frontend is a tool I picked up because a model sitting in a notebook helps nobody.

Most of what I build follows the same shape:

```mermaid
flowchart LR
    A["Real data<br/>CSV, uploads, user input"] --> B["Django + DRF<br/>ingest, validate, persist"]
    B --> C["ML pipeline<br/>scikit-learn"]
    C --> D["LangGraph + Gemini<br/>structured reasoning"]
    D --> E["REST API<br/>stable contracts"]
    E --> F["Next.js UI"]
    F --> G["Docker + Gunicorn<br/>EC2 · Vercel · Railway"]
```

- **Backend first** — Django + DRF, JWT auth, schema design, API contracts that don't change every week
- **Applied ML, not toy ML** — anomaly detection, imputation, similarity search, inside real request/response cycles
- **LLM systems** — LangGraph agents and Gemini pipelines that return structured output, not vibes
- **Deployment is part of the job** — Docker, Gunicorn, AWS EC2, Vercel, Railway

---

## Featured Work

| Project | What it does | Stack |
| :-- | :-- | :-- |
| **[DataLens AI](https://github.com/kreeshal17/Datalens-AI)** | Upload a CSV, get back a real data-quality verdict — profiled, scored, diagnosed and explained | DRF · Next.js · Postgres · scikit-learn · LangGraph · Docker · EC2 |
| **[Luma AI Studio](https://github.com/kreeshal17/LUMA-AI-STUDIO)** | Coding agent that generates *and incrementally edits* live React components from prompts | Next.js · TS · FastAPI · Postgres · Sandpack |
| **[BookMandu](https://bookmandu.vercel.app)** | Multi-vendor book marketplace with delivery-gated reviews, so only real buyers can review | Next.js · Prisma · Postgres · Tailwind |

<details>
<summary><b>DataLens AI — what's actually under the hood</b></summary>

<br/>

The interesting part isn't the upload form, it's what runs after it.

**1 · Profiling.** Row- and column-level statistics — type inference, null density, cardinality, distribution shape — rolled into a single quality score you can track across uploads.

**2 · The scikit-learn pass.** Three models, each answering a different question:

| Model | Question it answers |
| :-- | :-- |
| Isolation Forest | Which rows don't belong? |
| KNN imputation | What should the missing values have been? |
| TF-IDF + cosine similarity | Which rows are near-duplicates of each other? |

**3 · Root cause.** A LangGraph + Gemini layer takes those raw findings and turns them into plain-language explanations plus *structured* fix recommendations — enforced schema, so the frontend can render them instead of parsing prose.

**4 · Shipping it.** Backend containerized with Docker + Gunicorn on EC2, managed Postgres, frontend on Vercel. The ML runs inside the request cycle, so latency budgets were a design constraint, not an afterthought.

</details>

<details>
<summary><b>Luma AI Studio — the incremental-edit problem</b></summary>

<br/>

Generating a component from scratch is the easy half. The hard half is the second prompt: *"now make the sidebar collapsible"* — without regenerating and breaking everything else.

Solved with a component-driven architecture where each generation is a diff against persisted session state rather than a fresh render. Live preview through Sandpack, session history in Postgres, GitHub OAuth so the result can be pushed straight to a repo. Vercel + Railway.

</details>

---

## Stack

| | |
| :-- | :-- |
| **Languages** | Python · TypeScript · JavaScript · SQL · Java |
| **Backend** | Django · Django REST Framework · FastAPI · JWT auth · REST API design |
| **ML & LLM** | scikit-learn · pandas · NumPy · LangChain · LangGraph · Google Gemini |
| **Databases** | PostgreSQL · MySQL · Prisma |
| **Frontend** | Next.js · React · Tailwind CSS |
| **Infra** | Docker · AWS EC2 · Gunicorn · Vercel · Railway · Git · Power BI |

---


## Experience

**Backend Developer Intern** — Neosophical Labs Pvt. Ltd. · *Sep 2026 – Present*  
Developing and maintaining Django-based backend systems, building REST APIs, and contributing to production features across multiple application modules. Working on PostgreSQL-backed data models, authentication, business logic, and API integrations. Contributing to AI-powered features involving LLM integrations, voice processing, scoring pipelines, and asynchronous task handling. Also working on analytics APIs, notification systems, performance optimization, debugging, and backend reliability.

**Full Stack Developer Intern** — Mahalaxmi Tech Group Pvt. Ltd. (Remote) · *Jan 2026 – Mar 2026*  
Developed responsive Next.js pages and reusable UI components integrated with Django REST APIs. Worked across frontend and backend workflows, implementing API integrations, debugging application issues, and improving feature functionality. Followed PR-based GitHub workflows involving code reviews, collaborative development, and iterative improvements.

**Technical Team Lead** — Enigma Club, Jain University · *Oct 2025 – Apr 2026*  
Led a technical team across university events and technical initiatives. Organized coding workshops, mentored junior members on programming fundamentals and Git workflows, coordinated technical activities, and contributed to team planning and execution.

---



## How I Got Here

```text
Java + DSA + Spring Boot  →  scikit-learn & applied ML  →  FastAPI model serving  →  Django + DRF
        (year 1)                    (year 2)                     (year 3)              (now)
```

Started backend-heavy in Java, got pulled into ML in second year, learned to serve models as APIs with FastAPI, then moved to Django + DRF for the systems I actually want to build — production apps where the model is one component of a real product, not the whole demo.

**Going deeper right now:** multi-agent LangGraph workflows · RAG and retrieval pipelines · model serving at scale · Django internals and query optimization

---

## LeetCode

<div align="center">

<a href="https://leetcode.com/u/kreeshal17/">
  <img src="https://leetcard.jacoblin.cool/kreeshal17?theme=nord&font=Fira%20Code&border=0&radius=10&animation=false&ext=heatmap" alt="LeetCode stats" />
</a>

</div>



## Beyond the Code

- 🎓 **EdCIL COMPEX Scholar** — merit-based Government of India scholarship covering full undergraduate tuition
- 🧩 **275+ DSA problems** on [LeetCode](https://leetcode.com/u/kreeshal17/) — arrays, graphs, DP, SQL
- ✍️ **[Learn MySQL series](https://completesql.hashnode.dev/series/learn-mysql)** on Hashnode — SQL from fundamentals to query design
- 📜 HackerRank Advanced SQL · Google Cloud Generative AI · IBM Applied AI · IBM SkillsBuild Data Fundamentals

---

<div align="center">

### Open to backend, ML and AI engineering roles — 2027 batch

Talk to me about Django architecture, getting models out of notebooks, or LangGraph agents that behave.

**[karnakreeshal@gmail.com](mailto:karnakreeshal@gmail.com)** · **[krishalkarna.com.np](https://krishalkarna.com.np)**

</div>
