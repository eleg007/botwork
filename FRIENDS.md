# SMP Launch Kit

Server: **built, running, backed up**. The only missing piece: port 25565 open in the Oracle Cloud console (steps already given).

## Connection details

```
Address: 132.145.204.4:25565
Version: any Java Edition 1.21.11 or newer
```

- ViaVersion is installed → friends on **newer** clients (26.x) join a 1.21.11 server fine.
- Friends on **older** clients than 1.21.11 cannot join (ViaBackwards deliberately not installed — keeps it lean).
- Bedrock/phone players **cannot** join (Java server only).

## How a friend joins (send this as-is)

1. Open Minecraft Java Edition
2. Multiplayer → **Direct Connection**
3. Type `132.145.204.4` → Join Server
4. Done — they spawn at world spawn, free to play

Troubleshooting:
- "Timed out" → server is down or restarting (rare; auto-restarts). Ask again in a minute.
- "Outdated client" → update Minecraft launcher version.
- "You are not whitelisted" → shouldn't happen (whitelist off), report it.

## House rules (enforced by CoreProtect — everything is logged and reversible)

- No griefing, no stealing — CoreProtect logs every block change by name; rollbacks are one command
- Be nice in chat; I can mute/kick/ban from console
- No hacked clients (server is `online-mode=true`, vanilla expected)

## Draft announcement — needs owner approval before sending

> **Discord / group chat version:**
> hey — I set up a Minecraft survival server for us, it's free and always on 🟩
> join: Multiplayer → Direct Connection → `132.145.204.4`
> any version 1.21.11+ works. feel free to bring friends, the more the merrier. if anything breaks or looks griefed, tell me — everything's logged and I can roll it back

> **Short version (for a status/story):**
> made a minecraft server for the group, always on, free. DM me for the address 🟩

Notes for the owner:
- These are drafts — nothing gets sent without your OK.
- The address is the "invite" — anyone who has it can join. That's intended for the friend-growth model. If strangers ever show up, we can flip the whitelist on (one command).
- Suggested moment to send: right after I confirm the port is open, so nobody gets a "timed out" and gives up.

## Store (later, parent's Tebex)

Rank groups already exist server-side:
- `vip` — `[VIP]` prefix, 4 homes
- `mvp` — `[MVP]` prefix, 8 homes (inherits vip)
Store launch = one `/lp user <name> parent add vip` per purchase.
