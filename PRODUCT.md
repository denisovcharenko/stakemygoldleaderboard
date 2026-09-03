# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Static single-file HTML/CSS/JS SPA (`index.html`). No build step, no framework. Served as a static file. Git repo: `https://github.com/denisovcharenko/stakemygoldleaderboard.git`.

## Users

Crypto/DeFi participants in the StakeMyGold ecosystem — holders who stake assets and compete for rankings. They visit to check their rank, track XP accumulation, discover squads, and share referral links. Secondary audience: potential participants evaluating whether to join (landing/persuasion mode when no wallet is connected).

## Product Purpose

A seasonal staking leaderboard for the StakeMyGold platform. Participants earn XP by staking assets; the leaderboard ranks them individually and by squad. The product makes on-chain staking participation legible, social, and competitive. Success means a participant can immediately locate their rank, understand the gap to the next tier, and feel the season's momentum.

## Positioning

The product's differentiating bet is theatrical presentation: a vault-themed prestige aesthetic ("The Gilded Vault") that makes crypto staking feel like a high-stakes private club rather than a generic DeFi dashboard. The brand signals exclusivity and craft in a category dominated by functional but visually undistinguished leaderboards.

## Operating Context

- Accessed on desktop (primary) and mobile (secondary), no native wrapper
- Seasons are discrete periods with a `state` of `live`, `upcoming`, or `ended`
- Data is embedded as JS objects in the HTML (`SEASONS` array, participant/squad arrays)
- Wallet connection is simulated (no live Web3 integration in this version)
- Dark mode supported via `[data-theme="dark"]` on `<html>`

## Capabilities and Constraints

- SPA routing via `body[data-page]` attribute and `navigate(page, opts)` function
- Pages: home (leaderboard), profile, squad-detail, how-it-works
- Four typefaces: Archivo Black (wordmark), Playfair Display (editorial/numbers), IBM Plex Mono (data labels), Figtree (body/UI)
- Design tokens: `--navy:#0E1729`, `--gold:#F0BD5E`, `--gold-dp:#9A6A0A`, `--paper:#FFFFFF`, `--cream:#F8F6F2`, `--bg:#FDFCFA`
- Halftone canvas background, cursor-glow radial gradient, IntersectionObserver scroll animations, count-up XP animations
- `prefers-reduced-motion` respected throughout

## Brand Commitments

- Brand name: **StakeMyGold**
- Creative north star: **"The Gilded Vault"** — a private financial institution with centuries-old prestige, gold-leaf registers, and vault architecture
- Primary palette: navy (`#0E1729`) and gold (`#F0BD5E`)
- Wordmark rendered in Archivo Black
- Copy voice: confident, aspirational, slightly old-world prestige — not hype, not generic DeFi

## Evidence on Hand

- `index.html` — full SPA implementation
- `DESIGN.md` — visual system and design token documentation
- `.impeccable/design.json` — machine-readable design system sidecar
- `assets/partners/certik.svg` — security audit partner logo

## Product Principles

1. **Rank is theatre.** Every participant should feel the weight of their position — not a row number but a vault entry. Make rank visible, contextual, and emotionally resonant.
2. **Season drives urgency.** The leaderboard is never static; live seasons tick, approaching deadlines create action. Design should amplify time-sensitivity without anxiety.
3. **Craft signals trust.** In DeFi, visual quality is a trust signal. Impeccable typography, precise spacing, and tasteful animation communicate legitimacy before any copy does.
4. **Social is the mechanic.** Squads and referrals are not features — they are the compounding loop. Design should make sharing and squad membership feel like status, not utility.
5. **Mobile is real.** Participants check rankings from phones mid-session; the leaderboard must be as usable at 390px as at 1440px.

## Accessibility & Inclusion

WCAG 2.1 AA target. Skip-link to `#main` implemented. All interactive elements keyboard-accessible. `aria-hidden` on decorative canvas and glow elements. `prefers-reduced-motion` disables animations and count-up effects.
