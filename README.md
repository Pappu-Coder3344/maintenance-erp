
# Garments Maintenance ERP

A production-oriented full-stack project scaffold for the **Maintenance Department of a garments factory**.  
This package includes:
- full project structure
- PostgreSQL relational schema
- REST API contract
- NestJS backend scaffold
- Next.js responsive ERP UI scaffold
- sample data for machines, tickets, spare parts, PM templates, and demo users

## Repository structure

```text
garments-maintenance-erp/
├── apps/
│   ├── api/                     # NestJS backend scaffold
│   └── web/                     # Next.js frontend scaffold
├── database/
│   ├── json/                    # Sample demo data (machines, tickets, parts, PM templates)
│   └── sql/                     # DDL and reference seed
├── docs/
│   ├── solution-blueprint.md    # Full implementation blueprint
│   ├── api-reference.md         # Full API contract
│   ├── erd.md                   # Text ERD
│   ├── wireframes.md            # Page-by-page UI narrative
│   ├── user-journeys.md         # Module-wise role journeys
│   └── demo-credentials.md      # Sample login details
├── .env.example
├── docker-compose.yml
├── package.json
├── pnpm-workspace.yaml
└── tsconfig.base.json
```

## What is included

### Backend
- JWT-ready NestJS scaffold
- role / permission guard pattern
- maintenance-focused modules:
  - auth
  - dashboard
  - machines
  - preventive maintenance
  - tickets
  - work orders
  - spare parts
  - vendors
  - notifications
  - reports
  - admin
- mock service layer to support stakeholder demo

### Frontend
- responsive ERP dashboard layout
- left sidebar + topbar
- dashboard charts and KPI cards
- module pages for machines, PM, tickets, work orders, spare parts, history, vendors, reports, and admin
- modern enterprise SaaS styling approach

### Database and sample data
- SQL schema with PKs, FKs, enums, indexes, timestamps, and soft delete fields where appropriate
- reference seed file
- sample JSON data:
  - 20 machines
  - 50 spare parts
  - 30 maintenance tickets
  - 7 PM checklist templates
  - demo users and dashboard stats

## Quick start

1. Review the architecture in `docs/solution-blueprint.md`
2. Review relational design in `database/sql/schema.sql`
3. Review API contract in `docs/api-reference.md`
4. Start frontend and backend implementation from `apps/web` and `apps/api`

## Notes
- The backend controllers and services are scaffolded with representative mock logic so the structure is concrete and implementation-ready.
- Replace mock data with repository/database integration in the next implementation sprint.
- Change all demo credentials and secrets before any real deployment.
