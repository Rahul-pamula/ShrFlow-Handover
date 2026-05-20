# Welcome to the ShrFlow Documentation Portal

This is the interactive documentation portal for the ShrFlow Enterprise Email Engine, specifically prepared for senior engineers taking over the codebase and infrastructure.

## 📖 Recommended Reading Order

To understand the codebase quickly, explore the folders on the sidebar or follow this roadmap:

1. **[Visual Platform Tour](screen-shots/README.md):** Get an instant visual mapping of every user interface page, setting menu, and modal to their corresponding source code locations.
2. **[Introduction](introduction.md):** Read the core value proposition and general architectural introduction.
3. **[Quick Start Guide](getting-started/quick-start.md):** Get the local dockerized cluster running on your development machine in under 10 minutes.
4. **[Dispatch Engine Flow](plan/ENGINE_FLOW.md):** Understand the low-level asynchronous transactional loop of how campaigns are processed, queued, throttled, and dispatched.
5. **[Technical Infrastructure Tour](infrastructure/repo-structure.md):** Learn the exact directory structure of the repository, including the FastAPI backend (`platform/api`), backgrounds workers (`platform/worker`), and migrations.
6. **[Database & RLS Isolation](advanced/database-rls.md):** Inspect the PostgreSQL Row Level Security (RLS) configuration safeguarding the multi-tenant SaaS architecture.

---

*This portal is designed to be hosted directly on **GitHub Pages** using Docsify. To launch a local hot-reloading preview server, run:*
```bash
npx docsify-cli serve docs --port 4000
```
