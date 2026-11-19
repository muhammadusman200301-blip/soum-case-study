# Soum · Case Study

> **Source code is private under client NDA.** This repo documents the product, the architecture and my role. Happy to walk through it on a call: [book 30 min](https://calendly.com/muhammadusman200301/30min).

**Soum** is a Saudi marketplace for buying and selling, including live auctions, on web and mobile.

| | |
|---|---|
| **My role** | Full Stack Lead Engineer (Aug 2023 – Present) |
| **Team** | I lead 5 developers |
| **Platforms** | Web, iOS, Android |
| **Scale** | 1M+ downloads on Google Play |
| **Live** | [Web](https://soum.sa/en) · [App Store](https://apps.apple.com/us/app/soum/id1580930409) · [Google Play](https://play.google.com/store/apps/details?id=com.soum.sa) |

## Tech stack
React · Next.js · React Native · TypeScript · Node.js · PostgreSQL · Redis · AWS · Docker · GitHub Actions

## What I work on
- Own features end to end, from technical design and APIs to web and mobile screens, release and production support
- Design REST APIs and PostgreSQL schemas for listings, bidding, orders and payments
- Build iOS and Android features in React Native and manage App Store and Google Play releases
- Add AI features on LLM APIs, with structured outputs, retries and fallbacks
- Lead the team: sprint planning in Jira, code review on every pull request, weekly releases

## Architecture (simplified)

```
React Native app ─┐
                  ├──► Node.js REST APIs ──► PostgreSQL
Next.js web app ──┘          │         └──► Redis (cache)
                             ├──► Payment / SMS / push providers
                             └──► LLM APIs (AI features)
        CI/CD: GitHub Actions ──► Docker ──► AWS
```

## Challenges and how I handled them
- **Slow endpoints on busy screens** – traced the slowest queries, added indexes and caching, and cut response times on the busiest endpoints by about 30%.
- **Shipping often without breaking things** – moved the team to weekly releases with CI/CD, automated tests and code review on every change.
- **Mobile and web staying in sync** – shared API contracts and TypeScript types between the React Native and web apps.

---
More of my work: [Portfolio](https://muhammadusman-portfolio10.netlify.app) · [LinkedIn](https://www.linkedin.com/in/muhammad-usman-987852388/)
