# CLAUDE.md — ActionKeeper

## Brand Hub
**onepercentbetter.poker** — this project is listed there as `ActionKeeper`.
If it's removed from the site, it's no longer a brand asset.
Owner: Chris S. Yoon · github.com/sukminc

## What this is
Full-stack agreement & negotiation platform. Tamper-evident staking/deal agreements with dual-confirmation workflow.
Status: `building` (40% MVP)
Slug on hub: `actionkeeper` · Repo: `sukminc/action-keeper`

## Core Value
Poker context: formalize staking agreements, track action, prevent disputes.
General context: any high-stakes two-party agreement with audit trail needs.

## Stack
- Backend: FastAPI + PostgreSQL (Clean Architecture — Service/Repository layers)
- Frontend: Next.js + TypeScript
- Infrastructure: Docker, Stripe (payments)
- SHA-256 receipt hashing, full persistent audit trail

## Key Architecture
- Clean Architecture: Service layer → Repository layer → DB
- Dual-confirmation negotiation engine (Accept / Counter / Decline)
- Turn-based workflow with visual term diffs + side-by-side counter-offer comparison
- Tamper-evident hashing on every agreement record

## Commands
```bash
# Backend
cd backend && uvicorn app.main:app --reload

# Frontend
cd frontend && npm run dev
```
