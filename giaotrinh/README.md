# GiaoTrinh

GiaoTrinh is a Vietnam-only student exchange for lawful textbooks and study resources. Classmates browse and search without an account, then reveal the seller's contact after an explicit safety step and meet in person — no checkout, shipping, or in-app chat.

The source repository remains private. This folder is a public presentation layer with portfolio-safe screenshots and a concise case study.

![GiaoTrinh search discovery for a Casio listing](screenshots/02-discovery.png)

## Highlights

- Next.js `16.3.3` App Router + SSR with Appwrite (Auth, TablesDB, Storage, Functions)
- Anonymous browse/search/detail; `.edu.vn` domain-suffix eligibility for sellers
- Contact kept off public DTOs and revealed per listing after a safety acknowledgement
- Read-amplification hardening: school-catalog cache, batched projection, request dedupe, and HMAC image tokens with zero database reads
- Default-deny mutations and an ownership-aware private image proxy

## Portfolio status

**Feature-complete with caveats.** The product is feature-complete and deployment-ready on `main`; public production verification is pending an Appwrite database-read quota reset. Screenshots are from local fixture mode with synthetic `QA Seller` demo data. No live-user, traction, or launch claim is made.

See [case-study.md](./case-study.md) for the concise public case study and full screenshot set.
