# PLAN — Discord bot & server work (option A + D)

> **Started:** 2026-10-19 · **Owner:** 13 · **Budget:** ~$20 (spend nothing until it's earned) · **Parent rails:** unconfirmed (design assumption: payment comes LAST, never first)
> Scrimline stays deployed and untouched unless explicitly asked.

## The thesis

Scrimline proved the code is easy and the **distribution is the hard part**. So this venture
sells the skill directly to people who already have the problem (server owners who need a bot),
while building an audience in public so inbound work eventually replaces outbound outreach.

Honest revenue targets — **not guaranteed**, these are the "if you actually do the outreach" numbers:

| Month | If outreach happens (30 min/day) | If it doesn't |
|---|---|---|
| 1 | $0–100 (first 1–2 small jobs) | $0 |
| 2–3 | $100–300/mo | $0 |
| 6 | $200–500/mo possible w/ repeat customers | $0 |

## Phase 0 — foundations (days 1–2)
- [ ] Offer + pricing written (`OFFER.md`) — done
- [ ] Outreach venues + templates (`OUTREACH.md`) — done
- [ ] Safety rules read and understood (`OUTREACH.md` §4) — **owner must read this**
- [ ] Portfolio: public proof of work (see below)
- [ ] Ask parent the payment question ONCE (`PAYMENTS.md` script) — don't nag

## Phase 1 — first outreach (week 1)
- [ ] Join 3–5 Discord freelance/hiring servers from `OUTREACH.md` §1
- [ ] Post service ads per each server's forum rules (read rules first!)
- [ ] 2–5 Reddit posts/DMs (check each sub's rules at posting time)
- [ ] **Goal: 1 conversation, not a sale.** Sales come from conversations.

## Phase 2 — first job (weeks 1–3)
- [ ] Scope with `OFFER.md` questions, quote a fixed price, half-upfront **only once rails exist** (see `PAYMENTS.md`)
- [ ] Deliver fast (small scope: 1 feature or a server setup), ask for a testimonial
- [ ] **Goal: 1 delivered job + 1 testimonial, even if free/cheap.** Testimonials are the product of month 1.

## Phase 3 — repeat (month 2+)
- [ ] Maintenance retainer offer to every past customer ($10–30/mo)
- [ ] Portfolio page live (free: Cloudflare) showcasing 2–3 real jobs
- [ ] Start "build in public" posts (option D) — the audience engine: `POSTS.md`

## Portfolio — proof of work (decision needed)
Scrimline is a genuinely good portfolio piece: live bot, 5 slash commands, 27-test E2E suite,
production D1/KV on Cloudflare. Options:
1. **Make `eleg007/scrimline` public** after a fresh secret scan (fastest, strongest proof)
2. Build a sanitized public showcase repo (no tokens, no owner data) — safer
3. Host a portfolio page showing screenshots + the live bot invite link

→ Ask owner to pick; default is **2 + 3** (nothing sensitive ever public).

## Metrics to track weekly (in this file)
| Week | Outreach sent | Replies | Jobs quoted | Jobs won | $ earned |
|---|---|---|---|---|---|
| 1 | | | | | |
