# Clubdrop

**In one line:** AI-assisted merch preorder campaigns for student clubs — AI drafts, organizer decides, buyers get a polished page with no account.

<p>
<img src="screenshots/01-hero-issue.png" alt="Clubdrop Issue-template buyer campaign page" width="720" />
</p>

## The decision that matters

AI is allowed to **structure** messy club notes into a draft. It is **not** allowed to publish price, deadline, payment, or pickup without a human review. Public buyer pages are **zero-LLM** and use **five fixed templates** (not generated websites).

## Problem

Clubs still run drops through a chat post + Google Form + spreadsheet + DMs. Discovery is messy, details go stale, and there is no clean public page for buyers.

## What I built

- Canonical campaign model + five fixed templates
- Organizer workspace: setup, preview/publish, preorder roster
- Buyer link: preorder without an account
- Constrained AI draft → required organizer review → publish
- Deterministic buyer/organizer flows on structured data

## Flow

`messy notes → AI structure → required human review → publish → buyer preorder → roster`

## Stack

React Router · React · TypeScript · Cloudflare Workers · Supabase · Zod · Dify · Vitest · Playwright

## Status

Demo-ready on a development Worker. Closed-beta prep in progress. **Not** a production launch or traction claim.

## Screenshots

Live `clubdrop-dev` Worker. Synthetic Keybound Club merch. Buyer pages only.

| Issue (hero) | Commons |
| --- | --- |
| Magazine layout, product photo, deadline, no-account CTA | Lifestyle lookbook |
| ![Issue](screenshots/01-hero-issue.png) | ![Commons](screenshots/02-template-commons.png) |
| **Atelier** — quiet premium split | **Signal** — high-contrast poster |
| ![Atelier](screenshots/03-template-atelier.png) | ![Signal](screenshots/04-template-signal.png) |
