# Clubdrop

**In one line:** AI-assisted merch preorder campaigns for student clubs — AI drafts, organizer decides, buyers get a polished page with no account.

![Clubdrop Issue-template buyer campaign page](screenshots/01-hero-issue.png)

## Problem

Clubs still run drops through a chat post + Google Form + spreadsheet + DMs. Discovery is messy, details go stale, and there is no clean public page for buyers.

## What I built

- Canonical campaign model + **five fixed templates** (not generated websites)
- Organizer workspace: setup, preview/publish, preorder roster
- Buyer link: preorder **without an account**
- **Constrained AI:** structures messy notes into a draft; organizer must review price, deadline, payment, and pickup before save
- Public buyer pages are **zero-LLM**

## Why this shape

Clubs need occasional campaign tooling, not inventory, shipping, or a marketplace. Fixed templates stay polished; structured data keeps buyer/organizer flows deterministic. AI is optional assistance, not the source of truth.

## Flow

`messy notes → AI structure → required human review → publish → buyer preorder → roster`

## Stack

React Router · React · TypeScript · Cloudflare Workers · Supabase · Zod · Dify · Vitest · Playwright

## Status

Demo-ready on a development Worker. Closed-beta prep in progress. **Not** a production launch or traction claim.

## Screenshots

Live `clubdrop-dev` Worker. Synthetic Keybound Club merch. Buyer pages only.

| | |
| --- | --- |
| **Issue (hero)** — magazine layout, product photo, deadline, no-account CTA | **Commons** — lifestyle lookbook; templates are distinct |
| ![Issue](screenshots/01-hero-issue.png) | ![Commons](screenshots/02-template-commons.png) |
| **Atelier** — quiet premium split | **Signal** — high-contrast poster energy |
| ![Atelier](screenshots/03-template-atelier.png) | ![Signal](screenshots/04-template-signal.png) |
