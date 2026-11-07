# Azib Iqbal

<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=600&size=22&pause=1200&color=E6EDF3&center=true&vCenter=true&random=false&width=640&lines=Software+Engineer+%C2%B7+Integrations+%26+Backend;FastAPI+%C2%B7+Postgres+%C2%B7+Redis+%C2%B7+Celery;ERP+sync+that+survives+retries;Building+things+that+(hopefully)+work." alt="Typing SVG" />
</div>

## About

Software engineer at **MindHive Asia**, working on **MAIA**, an ERP built on Frappe / ERPNext.

Most of my time goes into **MAIA Sync Spine**: a standalone sync service that keeps MAIA and clients'
accounting systems in agreement, in both directions, without double-posting an invoice when a network
call times out halfway.

- Outbox / inbox pipeline on Postgres, claimed with `FOR UPDATE SKIP LOCKED`, drained by Celery workers
- Idempotency keys and per-entity partitions, so retries are safe and ordering holds within a document
- Plug-in adapters for **AutoCount**, **SQL Accounting**, **SQL Cloud**, **SAP Business One** and **Epicor**
- Dependency graph between doctypes, conflict handling, DLQ and redrive tooling, reconciliation jobs
- Live client onboarding and migrations: backfills, drift checks, stock and AR reconciliation

The rule I work by: near-real-time wrong data is worse than five-minutes-late correct data.

## Stack

### Backend and data

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" />
  <img src="https://img.shields.io/badge/Celery-37814A?style=for-the-badge&logo=celery&logoColor=white" alt="Celery" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" />
  <img src="https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=sqlalchemy&logoColor=white" alt="SQLAlchemy" />
  <img src="https://img.shields.io/badge/Frappe_/_ERPNext-0089FF?style=for-the-badge&logo=frappe&logoColor=white" alt="Frappe / ERPNext" />
  <img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="MariaDB" />
</p>

### Frontend

<p align="left">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS" />
</p>

### Infrastructure and tools

<p align="left">
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="AWS" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Vercel" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions" />
  <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" alt="Postman" />
  <img src="https://img.shields.io/badge/Claude_Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude Code" />
</p>

### AI and ML

<p align="left">
  <img src="https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white" alt="Gemini" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="scikit-learn" />
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Streamlit" />
</p>

## Selected projects

| Project | What it is |
|---|---|
| [ResumeRankr](https://github.com/azibbrrrrr/ResumeRankr) | Streamlit app that scores a resume against a job description with Gemini: ATS-style matching, skill gaps, likely interview questions |
| [MyCEO AI Tools](https://github.com/azibbrrrrr/MyCEO-AI-Tools) | Entrepreneurship platform for students aged 9 to 13: product ideas, branding, booth setup and profit maths, AI-assisted |
| [fastapi-rag-chatbot](https://github.com/azibbrrrrr/fastapi-rag-chatbot) | Retrieval-augmented chatbot behind a FastAPI service |
| [hex-mcts-ai-agent](https://github.com/azibbrrrrr/hex-mcts-ai-agent) | Hex-playing agent built on Monte Carlo tree search |
| [swishfit](https://github.com/azibbrrrrr/swishfit) | Full-stack e-commerce on Next.js, Node.js and PostgreSQL with SSR, admin dashboard and checkout |
| [maia-retro-tech-academy](https://github.com/azibbrrrrr/maia-retro-tech-academy) | An original, playable Malaysian retro-school campus |

## GitHub stats

<div align="center">
  <img src="./metrics.stats.svg" alt="GitHub stats across personal and organisation repos" />
</div>

## Currently

- Rolling clients onto Sync Spine one book at a time, with reconciliation before go-live
- Two-way document lifecycle: drafts, amends, cancels and payments that stay consistent across systems
- Making failures self-explaining: every DLQ row should say what broke and what fixes it

## Connect

<p align="center">
  <a href="https://azibiqbal.vercel.app/" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Portfolio" />
  </a>
  <a href="https://github.com/azibbrrrrr" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
  <!-- Add LinkedIn and email badges here once you choose which to make public. -->
</p>

<div align="center">
  <img src="https://komarev.com/ghpvc/?username=azibbrrrrr&style=flat-square&color=555555" alt="Profile views" />
</div>
