# ShrFlow Documentation

Welcome to the official ShrFlow documentation. ShrFlow is an enterprise-grade, self-hosted email marketing platform built for teams who need full infrastructure control.

<div class="tech-stack">
  <span class="tech-pill">⚡ FastAPI</span>
  <span class="tech-pill">⚛️ Next.js 14</span>
  <span class="tech-pill">🐇 RabbitMQ</span>
  <span class="tech-pill">🐘 PostgreSQL</span>
  <span class="tech-pill">🐳 Docker</span>
  <span class="tech-pill">🛡️ Multi-tenant RLS</span>
</div>

---

## Quick Navigation

<div class="card-grid">
  <a class="card" href="#/introduction">
    <div class="card-icon">📖</div>
    <div class="card-title">Introduction</div>
    <div class="card-desc">Understand the ShrFlow architecture and core concepts.</div>
    <div class="card-arrow">Read more →</div>
  </a>
  <a class="card" href="#/screen-shots/README">
    <div class="card-icon">🖼️</div>
    <div class="card-title">Visual Tour</div>
    <div class="card-desc">See every screen of the platform — 22 annotated screenshots.</div>
    <div class="card-arrow">View tour →</div>
  </a>
  <a class="card" href="#/getting-started/quick-start">
    <div class="card-icon">🚀</div>
    <div class="card-title">Quick Start</div>
    <div class="card-desc">Get ShrFlow running locally in under 10 minutes.</div>
    <div class="card-arrow">Get started →</div>
  </a>
  <a class="card" href="#/getting-started/first-campaign">
    <div class="card-icon">📧</div>
    <div class="card-title">First Campaign</div>
    <div class="card-desc">Send your first email campaign end-to-end.</div>
    <div class="card-arrow">Learn more →</div>
  </a>
  <a class="card" href="#/advanced/deliverability-engine">
    <div class="card-icon">⚙️</div>
    <div class="card-title">Delivery Engine</div>
    <div class="card-desc">Deep-dive into the dual-path dispatch architecture.</div>
    <div class="card-arrow">Explore →</div>
  </a>
  <a class="card" href="#/api-reference/authentication">
    <div class="card-icon">📡</div>
    <div class="card-title">API Reference</div>
    <div class="card-desc">Full REST API docs for campaigns, contacts, and auth.</div>
    <div class="card-arrow">View API →</div>
  </a>
</div>

---

## Platform At a Glance

| Layer | Technology | Role |
|-------|-----------|------|
| **Frontend** | Next.js 14 (App Router) | Dashboard, campaigns, analytics |
| **Backend** | FastAPI (Python) | REST API, business logic |
| **Queue** | RabbitMQ | Async email dispatch |
| **Database** | PostgreSQL + Supabase | Multi-tenant data store |
| **Auth** | Supabase Auth | JWT-based authentication |
| **Infra** | Docker Compose | Local + production orchestration |

---

## Getting Help

<div class="callout info">
  <span class="callout-icon">💡</span>
  <div>If you are a developer taking over this codebase, start with the <a href="#/introduction">Introduction</a> and then the <a href="#/screen-shots/README">Visual Tour</a> to orient yourself before diving into code.</div>
</div>

- **Stuck?** Check [Troubleshooting →](#/troubleshooting/common-issues)
- **Architecture questions?** See [Infrastructure →](#/infrastructure/repo-structure)
- **Running locally?** See [Quick Start →](#/getting-started/quick-start)
