# StackScan — RightStack v2 Prototype

A clickable prototype of RightStack repositioned as an **AI stack management** product:
*"See every AI tool your team actually uses — and what it costs."*

**Live demo:** _(add Vercel URL after deploy)_

## The thesis

The v1 catalog/recommendation product failed on ground truth: self-reported stacks go
stale, dashboards get boring, and a chat window can make recommendations for free.
v2 flips the build order — connect to sources of truth first (Google Workspace SSO,
billing feed), recommend second. The wedge is a **free shadow-AI scan**; the recurring
product is the **monthly delta** (what changed, what renews, what to cut).

## What's in the prototype

| View | What it shows |
|---|---|
| **Landing** | New positioning, how-it-works, pricing: Free scan / Monitor $149/mo / Concierge audit $750 |
| **Scan** | Mock OAuth connects (Workspace, M365, QuickBooks, card feed), paste/CSV tool-list input, sample company |
| **AI Stack Report** | Spend summary, shadow-AI count, redundancy/savings findings, renewal countdowns, full inventory, benchmark |
| **Dashboard** | The $149/mo product: monthly change events, keep/cut/switch action queue, cumulative savings vs. subscription cost |

The sample company is **Meridian Digital**, a fictional 24-person marketing agency:
14 AI tools, 5 of them shadow, $2,514/mo total spend, $405/mo in identified cuts,
and a $6,588 Jasper renewal 23 days out.

## What's real vs. mocked

**Real (runs in the browser):**
- Paste/CSV parsing matched against an embedded mini-catalog (~47 AI tools with
  categories, price estimates, and aliases)
- Redundancy detection by category overlap, with estimated savings
- Report generation from either the sample company or pasted input

**Mocked (illustrative only):**
- OAuth connections (buttons explain what they'd do)
- All sample-company data, benchmark figures, and dashboard events
- Seat/usage data, renewal dates, savings tracking

## Running it

No build, no dependencies — one static file.

- Local: open `index.html` in a browser
- Deploy: import this repo in Vercel (no framework preset needed)

## What we're looking for in feedback

1. Does the **free scan → monthly delta** wedge feel like something a 10–100 person
   company's ops lead would pay $149/mo for?
2. Is **shadow-AI discovery** the right hook, or is renewal/spend management stronger?
3. What's missing from the report that would make you say "wait, we're paying for *what*?"

---

*Prototype for review — not production. Built July 2026.*
