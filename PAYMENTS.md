# PAYMENTS — getting paid at 13 (the 18+ wall, handled)

## The problem (verified 2026-10-19)
Every mainstream cash-out rail requires the account holder to be **18+**:
Stripe, PayPal, Gumroad, Lemon Squeezy, Google AdSense, itch.io payouts (PayPal/Payoneer),
Discord Premium Apps (team owner 18+), Roblox DevEx (payout provider demands 18+).

→ **Software income needs an adult on the account.** It's a one-time ~30-minute setup,
not a permanent blocker.

## Script — ask once, politely
> "Hey — quick thing that could actually make money. To receive payments for bot work I'm doing,
> I need a PayPal (or similar) account, and it has to be 18+. Could you set one up as the account
> holder, or let me use yours for receiving? It's about 30 minutes and I'll do all the work of
> creating it — I just need you for the age verification and linking the bank card. I'll show you
> every transaction."

**If they say yes:** set up PayPal (18+ holder, your card as the payout), document it here, then
update `OFFER.md` payment wording with the real handle.

**If they say no / maybe:** don't push. Work continues on this order:
1. Take work, deliver, build testimonials — money is a *later* step
2. Options that work without adult rails:
   - Buyer pays a **parent's PayPal** per-invoice (same ask, smaller ask: "for one payment")
   - **Local/known people first** (family friends' businesses, school/community clubs) → paid in
     cash or bank transfer on the parent's card
   - **Gift cards** are an acceptable fallback for small jobs (Steam/Amazon) — never crypto
3. Re-ask in a month with proof: "I've delivered 3 jobs, I just need the account"

## Anti-scam rules for taking money
- Payment **clears before** source code / bot token / invite ownership transfers
- Half-upfront on jobs over $50 (once a real rail exists)
- No "I'll pay you twice if you send $20 first" — ever
- Screenshot every payment confirmation

## When rails exist — checklist
- [ ] PayPal account (adult holder) working and linked to a card
- [ ] Test receive $1 from a trusted person first
- [ ] Write the receiving details into `OFFER.md` §payment wording
- [ ] Then: raise prices — paid rails means you can quote without caveats
