# OFFER — services, pricing, scoping

## Service menu

| Tier | What | Price | Turnaround |
|---|---|---|---|
| **Starter** | Server setup: channels, roles, verification gate, welcome flow, bot config | $15–30 | 1–2 days |
| **Custom bot — small** | One focused feature (ticket system, leveling, form applications, giveaway, stats) | $30–60 | 3–5 days |
| **Custom bot — medium** | Multi-feature bot (moderation suite, LFG/matchmaking, applications + review) | $75–150 | 1–2 weeks |
| **Fix / urgent** | Debug or modify an existing bot | $15–40 | same/next day |
| **Maintenance** | Hosting upkeep, tweaks, uptime watch | $10–30/mo | ongoing |

**Pricing rules:**
- Never go below Starter price "for exposure" — exposure doesn't pay. Discount only for testimonials from *real, active* servers.
- Quote a **fixed price after scoping**, never hourly (hourly punishes you for being fast).
- First job may be discounted 25–50% **if** you get a public testimonial + permission to show the work.

## Tech you can honestly claim
- HTTP-interaction Discord bots on Cloudflare Workers (Scrimline: Ed25519 verification, slash commands,
  buttons, D1, KV, cron-ready) — **no 24/7 hosting bill for the customer, ever**. This is a real selling point:
  most competitors charge for a VPS.
- TypeScript, automated tests (27-assertion E2E), CI-ready deploys.
- 100k requests/day free tier covers essentially any small/medium server.

**Delivery promise you can keep:** "hosted free on Cloudflare — you'll never get a hosting invoice."

## Scoping questions (send these before quoting)
1. What should it **do**? (one sentence)
2. Who uses it — how big is the server? (members / daily online)
3. Do you have a bot already? What's wrong with it?
4. Do you want it in **your** bot account or a new one? (never ask for their token — see safety rules)
5. Any deadline?
6. Slash commands / buttons / web dashboard — which matter?

## What to say when they ask about you
> "I build Discord bots that run on Cloudflare Workers, so there's no hosting cost and no downtime.
> My live bot (Scrimline) handles teams, LFG and scrims with slash commands and has an automated test
> suite. I can show you a demo invite."

**Age:** be honest if asked — "I'm 13, I've been building bots with automated tests and shipping them
to production." Never pretend to be older; it only creates problems later, and being young + shipping
real production software is a better story anyway (see `POSTS.md`).

## Payment wording (use when quoting)
> "Payment via PayPal — [family account / details] once we agree on the scope."
> (Fill `PAYMENTS.md` first — do NOT invent payment details you don't have.)
