# Profolio

> **Your work. No noise.**

Profolio is a concept for a utility-first professional portfolio and hiring platform — envisioned as an alternative to the noise-driven model of platforms like LinkedIn. The core idea: your identity should be your work, not your posts.

> ⚠️ **This is an early-stage idea.** Everything in this repo — features, stack, architecture, monetization — is exploratory and subject to change as the project develops.

---

## The Problem

Modern professional networking has become a social media performance. Recruiters deal with broken filters and spam. Candidates have no single place to showcase work across code, design, and research. Profolio is an attempt to address that.

---

## Potential Features

- **Anti-Feed Dashboard** — A home screen built around job matches, connection suggestions, and portfolio health metrics rather than a scrollable social feed.
- **Verified Portfolio** — Embeds that pull directly from existing platforms like GitHub, Behance, and PubMed.
- **Granular Job Engine** — Filtering for true entry-level roles (0–2 years), internships, and senior positions via keyword extraction.
- **Direct-Only Networking** — Messaging limited to direct communication for hiring or networking, with no public walls or likes.
- **Recruiter Portal** — A separate view for hiring managers to filter candidates by verified skills and project types.

---

## Potential Tech Stack

These are the technologies being considered — nothing is finalized yet.

| Layer | Potential Technology |
|---|---|
| Frontend | React |
| Backend | Node.js / ASP.NET |
| Relational DB | PostgreSQL |
| Document DB | MongoDB |
| Web Server | Nginx (reverse proxy) |
| Containerization | Docker & Docker Compose |
| CI/CD | GitHub Actions |
| SSL | Certbot (Let's Encrypt) |
| Auth | OAuth 2.0 / OpenID Connect |

---

## Architecture Concept

The current thinking is an **N-Tier architecture** with separation between the UI, REST API, and database layers.

A possible **Service Layer** approach for third-party API communication:

- `GitHubService` — Repo data and language stats
- `BehanceService` — Design project galleries
- `PubMedService` — Research abstracts and publications

The idea is for the frontend to call a single endpoint that the backend uses to aggregate and return a unified response — but this is still being explored.

---

## Security Considerations

Areas being looked into, not yet designed or implemented:

- OAuth 2.0 + OpenID Connect SSO (Google, GitHub, Microsoft)
- AES-256 encryption for tokens at rest
- TLS 1.3 for all traffic in transit
- Role-Based Access Control (RBAC) for candidates vs. recruiters
- Audit logging on profile views

---

## Monetization Ideas

One possible direction is a no-subscription, no-ads model with optional one-time transactions — but this is very much up in the air:

- **Pay-per-Post** — A small fee for employers to list a job, which could also deter spam postings
- **Featured Listings** — Temporary search highlights for jobs or profiles
- **Verified Credential Badge** — Manual education and background verification
- **Corporate Partnerships** — Sponsored niche hubs (e.g., IBM Cloud Hub)
- **Portfolio Audit** — AI or expert review of a user's profile

---

## Project Status

> 🚧 **Early idea stage.** No code has been written yet. This repository will be developed throughout the capstone project.

| Phase | Status |
|---|---|
| Proposal & Research | 🔄 In Progress |
| System Design | 🔲 Not started |
| Backend Development | 🔲 Not started |
| Frontend Development | 🔲 Not started |
| Integration & Testing | 🔲 Not started |
| Deployment | 🔲 Not started |

---

## Capstone Info

- **Course:** INFO34049 — Semester 5
- **Student:** Marcus Podnar
- **Institution:** Sheridan College
- **Phase:** Year 1 Research

---

## License

This project is for academic purposes. License TBD.
