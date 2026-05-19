# Platform Automation & Utility Scripts

This folder contains utility scripts for database setup, deployment, data seeding, and platform monitoring. Always run these from the **project root** directory.

## Core Database & Setup Scripts

| Script | Purpose | How to Run |
|---|---|---|
| `apply_all_migrations.py` | Connects to PostgreSQL via `DATABASE_URL` and applies all schema migrations sequentially. Uses `schema.sql` first. | `python3 scripts/apply_all_migrations.py` |
| `apply_rls.py` | Connects via `DATABASE_URL` and applies all Row Level Security (RLS) policies for multi-tenant isolation. | `python3 scripts/apply_rls.py` |
| `seed_templates.py` | Seeds default high-fidelity MJML campaign templates into the database. | `python3 scripts/seed_templates.py` |
| `seed_dev_data.py` | Seeds mock development tenants, users, and tasks for local testing. | `python3 scripts/seed_dev_data.py` |
| `schema.sql` | Base schema snapshot used by `apply_all_migrations.py`. Reference only. | View only |

## Infrastructure & Monitoring Scripts

| Script | Purpose | How to Run |
|---|---|---|
| `e2e_readiness_check.py` | Validates end-to-end local platform readiness by testing S3, RabbitMQ, and DB connections. | `python3 scripts/e2e_readiness_check.py` |
| `region_monitor.py` | ESP-grade active-region health check and coordinator/lease manager for high-availability multi-region setups. | `python3 scripts/region_monitor.py` |

## VPS Deployment Utilities (Optional)

| Script | Purpose | How to Run |
|---|---|---|
| `install_vps.sh` | One-shot script to set up Nginx, SSH gateway ports, and Certbot/SSL certificates on Ubuntu VPS. | `sudo bash scripts/install_vps.sh <domain> <email>` |
| `start_tunnel.sh` | Sets up a persistent, auto-reconnecting SSH reverse tunnel from local environment to VPS. | `./scripts/start_tunnel.sh <user>@<domain>` |

> **Note:** Ensure your `.env` file at the project root contains a valid `DATABASE_URL` before running any database or setup scripts.
