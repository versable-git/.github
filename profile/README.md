<div align="center">
  <img src="./banner.svg" alt="Versable — AI-Powered Data Enhancement for the Automotive Aftermarket" width="100%"/>
</div>

<br/>

<div align="center">

[![Website](https://img.shields.io/badge/versable.ai-2563EB?style=for-the-badge&logo=googlechrome&logoColor=white)](https://versableai.com)
[![App](https://img.shields.io/badge/app.versable.ai-4F46E5?style=for-the-badge&logo=vercel&logoColor=white)](https://app.versable.ai)
[![Y Combinator](https://img.shields.io/badge/Y%20Combinator-F26522?style=for-the-badge&logo=ycombinator&logoColor=white)](https://ycombinator.com)

</div>

---

## What We Build

Versable is an **AI-powered data enhancement platform** built specifically for the automotive aftermarket parts industry. We transform incomplete, inaccurate, and non-compliant product listings into market-ready content — eliminating the manual work that costs sellers time and revenue.

> **"Supercharge your product data to help you sell"**

Versable is trained on millions of auto parts data points and employs programmatic guardrails to ensure zero AI hallucinations — accuracy is non-negotiable in the parts business.

---

## Core Products

| Feature                | Description                                                           |
| ---------------------- | --------------------------------------------------------------------- |
| **Data Normalization** | Merges supplier spreadsheets into fully ACES/PIES-compliant catalogs  |
| **AI Extraction**      | Adaptive scraper that auto-completes product catalogs from any source |
| **Content Generation** | SEO-optimized, platform-ready product descriptions at scale           |
| **Image Enhancement**  | Resize, enhance, or generate new product images from the database     |

**Supported formats:** PIES XML · JSON · Excel · Unstructured spreadsheets

---

## Who We Serve

- **Manufacturers** — audit data gaps and avoid costly partner rejections
- **Retailers & Distributors** — streamline supplier onboarding
- **Marketplaces & Buying Groups** — enforce catalog compliance at ingestion

---

## Infrastructure

```
╔═══════════════════════════════════════════════════════════════╗
║  Versable Infrastructure                                      ║
╚═══════════════════════════════════════════════════════════════╝

╭───────────╮
│  Browser  │
╰───────────╯
     │  HTTPS
     ▼
╔══════════════════════════════════════════════════════════╗
║  Vercel  (app.versable.ai)                               ║
║  ╭────────────╮  ╭─────────────────────╮  ╭──────────╮  ║
║  │ Next.js 16 │  │ /api/engine/* proxy │  │ NextAuth │  ║
║  ╰────────────╯  ╰─────────────────────╯  ╰──────────╯  ║
╚══════════════════════════════════════════════════════════╝
              │  /api/engine/* rewrite
              ▼
╔══════════════════════════════════════════════════════════╗
║  Render  (backend API)                                   ║
║  ╭──────────────────╮  ╭───────────────╮                 ║
║  │ FastAPI (Python) │  │ Credit Worker │                 ║
║  ╰──────────────────╯  ╰───────────────╯                 ║
╚══════════════════════════════════════════════════════════╝

  ┌──────────────── Shared Data Layer ─────────────────┐
  │  ┌────────────┐    ┌───────┐    ┌────────┐         │
  │  │ PostgreSQL │    │ Redis │    │ AWS S3 │         │
  │  └────────────┘    └───────┘    └────────┘         │
  └────────────────────────────────────────────────────┘

  ┌──────────────── External Services ─────────────────┐
  │  ┌─────────┐    ┌────────┐    ┌──────────┐        │
  │  │ AWS SES │    │ Stripe │    │ Sentry * │        │
  │  └─────────┘    └────────┘    └──────────┘        │
  └────────────────────────────────────────────────────┘
  * Sentry: production branch only
```

**Stack:** Next.js 16 · React 19 · FastAPI · PostgreSQL · Redis · AWS S3 · Stripe · Vercel · Render

---

## Repositories

| Repo                                                                         | Description                                         |
| ---------------------------------------------------------------------------- | --------------------------------------------------- |
| [`enhancement-product`](https://github.com/versable-git/enhancement-product) | Enhancement Product v2 — core Next.js + FastAPI app |
| [`logger-crab`](https://github.com/versable-git/logger-crab)                 | Centralized logging — Rust + axum + SQLite + S3     |
| [`organization-state`](https://github.com/versable-git/organization-state)   | Company status and internal happenings              |
| [`vcdb-check`](https://github.com/versable-git/vcdb-check)                   | Scripts to validate data against VCDB               |
| [`data-quality-trial`](https://github.com/versable-git/data-quality-trial)   | Public data quality tooling                         |

---

## Recognition

Featured by **Y Combinator** · **AutoCare Association** · **Forbes** · **USA Today** · **LA Weekly**

---

<div align="center">
  <sub>Built with precision for the automotive aftermarket &nbsp;·&nbsp; <a href="https://versableai.com">versableai.com</a></sub>
</div>
