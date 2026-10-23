# OPTION MC — self-hosted Minecraft server

> Researched 2026-10-19 at owner request. Presented as a standing option alongside A (bot work) + D (posting).

## 1. Feasibility on YOUR machine — verified ✅

| Requirement | Reality on this box | Verdict |
|---|---|---|
| Bandwidth | 6 GB/mo outbound vs **10 TB** cap (0.06%) | ✅ non-issue |
| CPU | 2× Neoverse-N1 (ARM server cores) | ✅ fine for 10–20 players (Paper runs well on ARM) |
| RAM | 7.7 GB total, **4.5 GB available** | ✅ 2–3 GB heap for a small server + headroom |
| Java | OpenJDK **21** already installed | ✅ current Paper/Velocity target |
| Disk | 46 GB, **12 GB free (74% used)** | ⚠️ tightest resource — world + backups need monitoring |
| Cost to run | $0 (existing VM, electricity/hosting already paid) | ✅ |
| Setup labor | **I can do 100% of it**: install Paper, configure, plugins, backups, Discord bridge, autorestart, firewall | ✅ |

**Setup work I'd automate end-to-end:** Paper server + `server.properties` tuning, EssentialsX/LuckPerms,
anti-cheat + chat filter, Discord chat bridge (your Scrimline Discord experience transfers), automated
world backups with rotation, systemd autorestart, status page, vote-reward plugin (Votifier).

## 2. How players actually arrive (the honest part)

- Players find servers via **lists**: minecraft-server-list.com, minecraft-mp.com, Planet Minecraft, TopG, DISBOARD (MC tag). Listing is free, and this is genuinely **inbound** — no pitching.
- **But lists rank by daily votes.** A server with no votes sits on page 40. A server with steady votes climbs to page 1 → joins.
- Vote loop options: (a) players vote for rewards (needs players first), (b) you vote daily per list — ~5–10 min/day **your** time, (c) in-game vote parties to make it fun.
- Bootstrap reality check (from hosting-industry stats): **~95% of new servers die in month 1** — from zero traffic, not from technical failure.
- Secondary channels: your own Discord (reusing the Scrimline community angle), TikTok/YouTube shorts of builds, Reddit server threads.

## 3. Monetization — same 18+ wall, verified

| Path | Rule found | Works for you? |
|---|---|---|
| **Tebex** (the standard MC store — Mojang-endorsed) | "You must have full legal capacity (**usually 18+**). Otherwise, a parent/guardian must register" + Onfido **ID verification** | Only with a parent |
| CraftingStore / similar | Same age class | Only with a parent |
| Ko-fi / PayPal donations | 18+ | Only with a parent |
| **BuiltByBit** (sell setups/plugins — see §5) | ToS: **"at least 13 years of age"**, minors need parent permission | ✅ **Yes, at 13** |

EULA rules (Mojang): you **may** sell cosmetics, ranks, convenience, queue priority — you may **not**
sell gameplay advantages (pay-to-win). Cosmetic-only stores are the norm and are compliant.

## 4. Revenue & time — realistic, no hype

| Stage | Money | Your screen time |
|---|---|---|
| Month 1 (0 → first players) | **$0** | High: list submissions, daily votes, being present in-game/Discord |
| Month 2–3 (5–20 regulars, store live w/ parent) | **$0–50/mo** typical; most servers stay $0 | Medium: events, moderation (I automate ~70% of it) |
| Month 6 (if it actually retains) | **$20–150/mo** possible, not guaranteed | Medium — communities decay without a human present |

**The honest ledger:** bandwidth/CPU/money ✅ solved. The one scarce resource you flagged is
**screen time** — and a Minecraft community is the *most* human-hungry option of everything on the
table. Moderation, events, welcoming new players: I can automate plugins and moderation, but I cannot
be a host. If a server sits empty, no vote grind fixes that.

## 5. The variant that fits your constraints better

**Sell server products instead of running one.** BuiltByBit (13+ ✅) has active paid categories for
**pre-built server setups, plugins, configs, builds**. Buyers come to the marketplace (fully inbound),
I build the products with AI, you approve listings and spend ~30 min/week. Payouts: Tebex wallet →
PayPal (**parent**, one-time).
- A **live server you already run** becomes your demo/showroom — so MC-1 and MC-2 reinforce each other
- Same effort spent, but the product persists and sells while you sleep; a community doesn't

## 6. Owner's proposed model (researched 2026-10-19) — tiers + friend-join

**"Tiers and items in-game, grown by players joining like a friend's world."**

### In-game store — what Mojang actually allows ✅/⚠️
The rule (Commercial Usage Guidelines): **paying players may get NO gameplay advantage.**

| Sell this | Status |
|---|---|
| Rank tiers (VIP/MVP tags, chat colors, cosmetics, particle trails, pets, emotes, extra homes, queue priority, name changes) | ✅ **EULA-safe** — the standard model; cosmetic monetization is what the most successful 2026 servers run on |
| Crate keys / gacha cosmetics | ✅ allowed (keep rewards cosmetic) |
| **Items: gear, weapons, armor, tools, resources** | ❌ **pay-to-win = against the guidelines** — this is the line Mojang draws sharply; getting your domain blocked by Mojang is the enforcement stick |
| "Convenience" that is purely comfort (homes, warps, kits of beginner starter gear, XP boosts in casual servers) | ⚠️ gray zone — common in practice, technically an advantage; safest to keep minimal or cosmetic |

**→ Tiers: yes, profitable and legal. Items: only cosmetic/convenience items — no competitive gear.**
Store platform = **Tebex** (Mojang-endorsed) → **18+ with ID verification, parent must register**.
Sequencing: **launch free first**, open the store the day a parent completes Tebex (~30 min).

### "Join as a friend" growth ✅ — this is now real, and new
- **Mojang shipped an official Friends List to Java Edition** (snapshot 26.2-7, May 12, 2026) — for the first time in Java's history, no address-typing needed.
- **OpenFriend** (SpigotMC plugin, server-side) **bridges that official Friends List to any server** → your friends click your name and join, exactly like a Bedrock/Realms world. **I install this.**
- This **kills the daily vote grind** as the growth engine: growth = your friends → their friends, in-game, zero promotion spend. Server lists stay as an *optional* later layer, not a chore.
- Honest caveat: friend-of-friend growth is slower than lists but compounds and costs **zero screen time** — it's the best fit found yet for "limited screen time".

### Suggested phase order
1. **Launch free** (friends join via Friends List; I build everything: Paper + OpenFriend + Discord bridge + backups + moderation)
2. **Store live** the moment a parent does Tebex (rank tiers only, cosmetic)
3. **Lists later, optional** — only if friend growth stalls and you have 20 min to spare

## 7. Build state (live since 2026-10-19)

**Server is built and running** on the box. Full inventory:

| Component | Detail |
|---|---|
| Server | Paper **1.21.11** build 132 (SHA-256 verified against Paper API) |
| RAM / disk | -Xms1G -Xmx3G (uses ~1.4G live); world currently ~2.3M, disk headroom 12G |
| Port | 25565 (ufw allowed) |
| Public address | `132.145.204.4:25565` |
| Plugins | ViaVersion 5.12.1 (lets newer clients join), EssentialsX 2.22.0 (homes/kits), LuckPerms 5.5.71 (ranks), Vault 1.7.3, CoreProtect 24.1 (grief rollback /audit) |
| Rank groups | `vip`, `mvp` created with prefixes + extra homes — **store-ready** |
| Service | `systemd` unit `mcserver` — autostart on boot, graceful stop, auto-restart on crash |
| Backups | Daily 04:00 via `mcserver-backup.timer` (save-all flush → tar.gz → last 5 kept) |
| Admin channel | RCON on localhost:25575 (password `~/.mc-rcon-password`, blocked externally by ufw) |
| Management | `systemctl status/restart mcserver`, logs at `~/mcserver/logs/latest.log` |

**Version choice rationale:** server = 1.21.11 (most common current client line, OpenFriend-compatible) + ViaVersion so friends on newer 26.x clients can still join.

### Port 25565 — OPENED & VERIFIED (2026-10-19)
Owner added the Oracle Cloud ingress rule; external ping confirmed `online: true`, correct MOTD, 0/20 players, `eula_blocked: false`. **Server is publicly joinable at `132.145.204.4:25565`.**

### Still optional (owner decision)
- **OpenFriend** (friend-list joining): third-party jar that runs a companion process with a Microsoft login — flagged for supply-chain risk; default = NOT installed until owner approves. Plain address join works without it.
- **Discord chat bridge**: EssentialsXDiscord module available from same release; needs a bot token + channel choice.
- **Tebex store**: ranks only (cosmetic), parent 18+ registration day one is available.

## 8. Verdict

| | Fits "no outreach"? | Fits "limited screen time"? | $0? | Money realistic? |
|---|---|---|---|---|
| **MC-1: run a server** | Mostly (lists = inbound) | ❌ weakest — needs daily human presence | ✅ | $0–150/mo, most servers $0 |
| **MC-2: sell setups on BuiltByBit** | ✅ fully inbound | ✅ ~30 min/week, I do the rest | ✅ | Small but real once listed |
| A (bot commissions) | ❌ outreach needed | ⚠️ moderate | ✅ | $50–300/mo fastest |
| D (build in public) | ✅ | ✅ you approve, I draft | ✅ | $0 for months |

**Recommendation:** MC-2 (sell setups) as the Minecraft play, optionally running MC-1 as a
low-effort showroom/community you'd enjoy anyway — treat the server as a **hobby with a shop attached**,
not as the income. MC-1 alone does not solve your screen-time problem.
