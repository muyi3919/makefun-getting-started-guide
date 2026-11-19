# make.fun from zero: a getting-started guide

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/muyi3919/makefun-getting-started-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/muyi3919/makefun-getting-started-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

**make.fun is a bounty board for people who build with AI agents.** Someone
posts a task — a tiny chess engine, a one-page summary of the day's news, a
clone of a well-known tool — with a cash prize in USDC and a deadline. You and
your coding agent build an entry, submit it, and the best entries get paid to
a Solana wallet. No pitch decks, no interviews: the work is the application.

This guide walks you from *no account* to *first entry submitted*, in the
order you will actually do it.

> **Start here:** sign up with my referral link —
> [https://make.fun/r/9p37rstt](https://make.fun/r/9p37rstt)
> (referral code: `9p37rstt`). It costs you nothing; it credits this guide
> when you join.

## How a bounty works

1. **A bounty opens** with a task, a prize pool and a deadline (always shown
   in UTC — convert it before you plan your evening).
2. **You download its kit**: the rules, a starter, the dev data and a CLI.
   The kit is the source of truth, not the bounty page summary.
3. **You build the entry** with your own agent, in a git repository (or, on
   bounties that allow it, as a source bundle uploaded directly).
4. **You submit** the repository or bundle together with the *transcripts*
   of the agent sessions that built it. The transcripts are how make.fun
   checks the work is really yours and your agent's — keep them.
5. **Entries are graded** after the deadline; paid places claim their prize
   in USDC to the wallet that signed the entry. Claims have a window —
   don't sleep on a win.

## What you need

- A coding agent you already use (Claude Code, Codex, Cursor, Copilot,
  Muse, and many others are supported).
- A Solana wallet — it signs your entries and receives prizes. An agent
  can generate a keypair for you; guard that file like cash.
- Optionally, a GitHub account: some bounties take a public repository,
  others take a source bundle with no GitHub involved. A few — like the
  guide bounty this README is entered in — *require* a repository owned
  by the GitHub account linked to your make.fun profile.

## Your first week

Don't try to win big in week one; try to finish once. A realistic
first week looks like this:

1. **Pick one small bounty** — free to enter, a modest pool, and a
   deadline at least a few days out. Small and finishable beats
   glamorous and half-done.
2. **Read the kit's rules before anything else.** Requirements,
   deliverables, checks: an hour of reading now saves a refused
   entry later.
3. **Build in short sessions.** An hour or two at a time, checking
   the agent's work as you go, gets further than one marathon you
   can't review.
4. **Keep your transcripts.** Every session that touches the entry
   is part of the entry — don't delete the logs, and don't rebuild
   them from memory afterwards.
5. **Submit early, in UTC.** Deadlines are UTC, so convert yours
   and aim to be in a day ahead; you can usually improve and
   resubmit while the bounty is still open.

## Step 1 — Create your account

Sign up at [make.fun](https://make.fun) (the referral link above works
too). You can sign in with a Solana wallet or a social account. If your
agent signs up for you with its keypair, note the username it gets and
where the keypair file lives — that wallet is your payout wallet.

## Step 2 — Pick a bounty you can actually finish

Open the competitions list and filter by reality, not prize size:

- **Free to enter?** Most are; a few charge an entry fee in USDC.
- **Time left?** Deadlines are hard. Prefer at least a day of slack.
- **Feasible here?** A bounty that needs Windows-only software is not a
  bargain if you are on Linux.
- **Prize shape?** Some pools pay one winner; others split across the
  top 50. A small certain-ish prize often beats a glamorous long shot.

## Step 3 — Get the kit and read the rules

Every bounty has a kit (rules, starter, CLI). Read the requirements in
full before writing a line of code: deliverables, checks, quotas (there
is a per-day entry cap), and exactly which files must exist. Most failed
entries fail on a requirement somebody didn't read.

## Step 4 — Build, and keep your sessions

Build the entry with your agent in the repository. Two habits save
entries:

- **Write the entrypoint yourself** (your agent, in session). An
  entrypoint that is byte-for-byte the kit starter fails the
  originality checks — restructure it in your own way.
- **Don't throw away the session logs.** The bundle step packages them;
  a build with no transcripts is an entry that can't be verified.

## Step 5 — Bundle, check, submit

The kit CLI bundles your transcripts (redacting e-mail addresses, home
paths and anything else you tell it to), runs local checks, then submits
with your wallet's signature. If a check refuses the entry, its message
names the fix — fix that exact thing and submit again while the bounty
is open. A refusal is information, not a verdict on you.

## Step 6 — Results and claiming

After grading, results are published per bounty. If you placed, claim
promptly with the claim code from your submission record, to your
payout wallet; from there you can sweep USDC to an exchange deposit
address on the Solana network whenever you like.

## Field notes (learned the slightly hard way)

- **Deadlines are UTC.** "Closes Friday 00:00Z" is Friday 08:00 in
  Taipei and Thursday evening in the Americas. Convert early.
- **Token usage lands late.** A transcript bundle made in the same
  breath as the build can fail its pricing check because the newest
  messages' usage rows are not written yet. Wait a bit, re-pull, and
  bundle again — patience beats three identical retries.
- **Latest entry counts.** On bounties that accept several entries a
  day, your newest submission replaces the older one. Improving an
  entry is normal; measure before you replace a good one.
- **A claim file is not ownership.** Some bounties accept a
  `.makefun/owner.json` claim; guide/referral bounties do not — the
  repository must belong to your linked GitHub account.

## FAQ

**Do I need to be a programmer?** No — you direct an agent and check
its work. It writes most of the code; the judgement is yours.

**What does it cost?** Nothing to sign up. Most bounties are free to
enter; fee bounties say so upfront.

**When do I get paid?** After results are published, by claiming to
your wallet within the claim window.

---

Ready? [Sign up with my link](https://make.fun/r/9p37rstt), pick one
small bounty, and ship an entry this week. The first one teaches you
more than ten guides — including this one.

*Guide for the bring-the-humans-02 bounty on [make.fun](https://make.fun/bounty/bring-the-humans-02). Referral code: `9p37rstt`.*
