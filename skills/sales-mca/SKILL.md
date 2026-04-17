# Merchant Cash Advance (MCA) Playbook

## Metadata
- **Title:** MCA Industry Playbook — shared context for MCA sales
- **Invocation:** auto-loaded by `/sales` commands when the product is MCA; also directly readable as reference
- **Purpose:** Single source of truth for MCA domain knowledge (product mechanics, ICP, qualification, pricing math, objections, competitors, compliance, underwriting signals)

---

## Product Primer

**Merchant Cash Advance (MCA)** is the purchase of a fixed dollar amount of a business's *future receivables* at a discount. It is **not a loan** — it is a purchase-and-sale of receivables governed by a merchant agreement (not a promissory note).

| Term | Plain English |
|------|---------------|
| Advance amount | Cash funded to the merchant today (e.g., $50,000) |
| Purchased amount / RTR | Receivables we buy — advance × factor rate (e.g., $50k × 1.35 = $67,500) |
| Factor rate (buy/sell) | Multiplier applied to the advance. Typical range **1.15 – 1.50**. Buy rate = wholesale from funder; sell rate = what's quoted to merchant |
| Term | Expected payback window, typically **3–18 months** (sweet spot 6–12) |
| Payment frequency | Daily ACH, weekly ACH, or % of card settlements (holdback) |
| Holdback % | If split-funded: 5–20% of daily card batch is diverted to repay RTR |
| Daily/weekly payment | Purchased amount ÷ number of business days/weeks in the term |
| Position | 1st, 2nd, 3rd, etc. — how many concurrent advances the merchant has |
| UCC-1 | Blanket lien filed by funder on receivables |
| PG | Personal guarantee from owner (standard) |
| COJ | Confession of Judgment (outlawed in NY since 2019 for out-of-state merchants; regulated elsewhere) |
| Reversal | Merchant blocks ACH — triggers default clauses |
| Modification | Reduced payment for hardship (not forgiveness) |
| Stacking | Taking a new advance while an existing one is outstanding |
| Consolidation / Reverse consolidation | Refi multiple positions into a single larger advance |
| Renewal / Pay-and-renew | Merchant tops up before existing advance is fully paid off |

**Funding timeline:** Application → bank statements → underwriting → approval (same day to 24 hrs) → contract → funding. Speed-to-fund: **24–72 hours** is the industry promise.

---

## ISO vs Direct Funder

This playbook assumes the seller is an **ISO / broker** placing deals with one or more funders. Where it matters, both perspectives are noted.

- **ISO:** sources merchants, packages deals, shops to funders, earns **8–15% commission** on funded amount (sometimes residual on renewals).
- **Direct funder:** underwrites with own capital, owns the receivables, collects directly.

---

## Ideal Customer Profile (ICP)

### Preferred Industries (A-tier)
Restaurants & food service · retail storefronts · auto repair & auto body · trucking & transportation · construction & general contracting · HVAC / plumbing / electrical · medical & dental practices · veterinary · salon / spa / beauty · e-commerce (US-based, processing history) · manufacturing · wholesale & distribution · landscaping · dry cleaning · gyms & fitness studios · specialty retail.

### Workable Industries (B-tier)
Hospitality / hotels · staffing agencies · non-franchise QSR · specialty food · catering · printing · signage · moving & storage · pest control · cleaning services.

### Restricted / Hard-to-Fund (confirm per funder before pitching)
Adult entertainment · cannabis / CBD (varies; only a handful of funders) · gambling & gaming · cryptocurrency · MLM · debt consolidation / settlement · law firms on contingency · real estate investment (fix-and-flip varies) · used car dealers · pawn shops · firearms dealers · travel agencies · ticket brokers · telemarketing · charities / nonprofits · trucking without DOT authority · one-off event businesses.

### Firmographic Sweet Spot

| Criterion | Ideal | Workable | Disqualifier |
|-----------|-------|----------|--------------|
| Monthly revenue | $50k–$500k | $15k–$50k | < $10k |
| Time in business (TIB) | 2+ years | 6–24 months | < 3 months |
| Personal FICO (owner) | 650+ | 550–649 | < 500 unless strong bank |
| Average daily balance | $5k+ | $1k–$5k | < $500 |
| Monthly deposits | 10+ | 5–9 | < 5 |
| NSFs (last 90 days) | 0 | 1–3 | 4+ |
| Negative days (last 90) | 0 | 1–5 | 6+ |
| Open positions | 0 | 1–2 | 3+ (stacking flag) |
| Entity type | LLC / Corp / Inc | Sole prop w/ EIN | No EIN, personal-name checking only |
| Geography | US lower 48 | AK / HI (some funders) | Non-US, US territories (most funders) |

### Trigger Events (why NOW)
- Slow season / cash flow gap
- Payroll shortfall
- Equipment breakdown (oven, truck, HVAC, POS)
- Inventory buy ahead of busy season
- Expansion (second location, build-out, renovation)
- Tax bill (IRS / sales tax / payroll tax)
- Vendor pay-down for discount
- Marketing push
- Buyout of partner
- Bridge to pending SBA / bank approval

### Negative ICP — do NOT pursue
Under 3 months TIB · under $10k/mo revenue · 4+ NSFs or 6+ neg days in last 90 · 3+ open positions (unless pitching consolidation) · bankruptcy discharged < 12 months · open tax lien > $25k without subordination · open judgments · restricted industry with no funder appetite · personal-name-only banking · no merchant processor and revenue is card-heavy (split funding impossible) · fraud flags (manipulated statements).

---

## Qualification Framework (MCA-specific, replaces BANT)

Use the **Five-Signal Stack** in place of generic BANT:

| Signal | Weight | What to Measure | Data Source |
|--------|-------:|-----------------|-------------|
| **Revenue** | 25 | Average monthly gross deposits over last 3 months | Business bank statements |
| **Bank Health** | 20 | ADB, deposit frequency, NSFs, negative days, ending balances | Business bank statements |
| **Time in Business** | 15 | Date entity formed / first commercial activity | Sec of State, EIN letter, bank statement earliest date |
| **Credit (Owner)** | 15 | FICO (personal), business credit if present, judgments/liens | Soft pull w/ consent |
| **Position / Stacking** | 15 | Count and balance of concurrent MCAs, daily/weekly ACH load | Bank statements (look for daily debits to known funders) |
| **Industry / Use of Funds** | 10 | Industry code fit + clear, legitimate use | Application + conversation |

### Score → Paper Grade → Funder Tier

| Score | Paper | Typical Factor Rate | Term | Funder Tier |
|-------|-------|---------------------|------|-------------|
| 90–100 | **A+ / A** | 1.15 – 1.28 | 9–18 mo | Tier-1 (Credibly, OnDeck, Forward Financing, Fora A-tier) |
| 75–89 | **B+** | 1.24 – 1.35 | 6–12 mo | Tier-1/2 (Kapitus, Rapid Finance, CFG, Libertas) |
| 60–74 | **B / B-** | 1.30 – 1.42 | 5–9 mo | Tier-2 (Everest, Kalamata, Mulligan) |
| 40–59 | **C** | 1.38 – 1.49 | 3–6 mo | Tier-3 / high-risk funders |
| 0–39 | **D** | N/A | N/A | Decline or refer to alternate products |

*Factor rates above are directional — always pull real quotes from your funder panel.*

### Required Underwriting Package

**Minimum (A/B paper):**
1. Completed 1-page application (legal name, DBA, EIN, owner SSN + DOB, address, industry, requested amount, use of funds)
2. 3 months business bank statements (all pages, PDF, not screenshots)
3. Driver's license (front)
4. Voided business check

**Additional for larger deals ($150k+) or scrutinized files:**
5. 4th month bank statement
6. YTD P&L
7. Most recent business tax return
8. Credit card processing statements (3 months) if pitching split funding
9. Property lease or deed
10. Landlord / business reference

**Additional for restricted industries or re-funds:**
11. Current payoff letters from existing funders
12. Inter-creditor agreement (for consolidation)
13. Subordination agreement (for tax liens)

---

## Pricing Math (memorize)

```
Advance           × Factor Rate        = Purchased Amount (RTR)
$50,000           × 1.35               = $67,500

Purchased Amount  ÷ Term in days       = Daily Payment
$67,500           ÷ 126 business days  = $535.71/business day

Purchased Amount  ÷ Term in weeks      = Weekly Payment
$67,500           ÷ 26 weeks           = $2,596.15/week

Daily Payment     × 21 business days   = Approx monthly debit
$535.71           × 21                 = $11,250/mo
```

**Quick gut-check:** Monthly debit should not exceed **~9% of average monthly deposits** on a first position. Higher = stacking risk.

**APR calculation (for comparison only — never lead with APR):**
```
APR ≈ ((Factor Rate − 1) × 2 × (12 / Term in months)) × 100
1.35 factor, 6-month term ≈ ((0.35) × 2 × 2) × 100 = 140% APR
```
This is why we **do not** position MCA against APR-priced products. We position on **speed, access, and capital velocity**.

---

## Use-of-Funds ROI Framing

Always convert the conversation from "cost of capital" to "what this capital earns":

| Use of Funds | ROI Framing |
|--------------|-------------|
| Inventory buy at vendor discount | Discount captured vs factor cost |
| Equipment (oven, truck, AC) | Days of lost revenue avoided |
| Marketing / ad spend | CAC × LTV multiple |
| Payroll gap | Jobs kept × billable revenue retained |
| Expansion / second location | Projected monthly revenue lift |
| Tax payoff | Penalty + interest avoided |
| Emergency repair | Shutdown days avoided |

**Scripted pivot:** *"Forget the factor rate for a second — tell me what the $50k does for you. If that inventory buy puts $120k in your register at your normal margin, the math is obvious."*

---

## The 10 MCA Objections (use alongside `sales-objections` universal list)

1. **"The factor rate is too expensive."** → Speed, no collateral, approves when banks won't, pricing reflects risk. Pivot to ROI on use-of-funds.
2. **"Daily ACH will kill my cash flow."** → Payment is calibrated to your revenue (<9% of deposits). Weekly option available. Compare to a lump-sum bank payment.
3. **"I'll go to my bank / SBA."** → 20% approval rate, 45–90 days, collateral + 680+ FICO required. Offer to fund now + refi into SBA later.
4. **"I'm already stacked."** → Consolidation / reverse consolidation — one payment, lower daily, sometimes net cash out.
5. **"This isn't a real loan / I've heard it's predatory."** → It's a receivables purchase, governed by a merchant agreement. Terms are disclosed upfront. Walk through the agreement page by page.
6. **"I want to shop multiple offers."** → "I *am* your shop — I place your file with 40+ funders so you don't hit your credit 40 times." One hard pull, best offer wins.
7. **"I need to talk to my accountant."** → Encourage it. Offer to get on a three-way. Real question: is the accountant a decision blocker or a shield?
8. **"Payback is too much — I'm paying $67k to borrow $50k."** → Reframe as capital cost per week/day and tie to revenue generated.
9. **"I don't want ACH touching my account daily."** → Explain the mechanics. Offer weekly. Explain reserve account option.
10. **"I've been turned down before."** → Different funders, different appetites, different programs today vs 6 months ago. Let's re-submit.

Each of these is expanded into full FFR + ABC scripts in the `/sales objections mca` output.

---

## Competitive Landscape

### Funders / Direct Lenders
**A-paper term lenders:** OnDeck (term loans + LOC), Credibly, Bluevine (LOC), Fundbox (LOC), Headway Capital (LOC), Kapitus (term + MCA).

**B/C-paper MCA funders:** Forward Financing, Fora Financial, Rapid Finance, Libertas Funding, CFG Merchant Solutions, Kalamata, Everest Business Funding, Mulligan Funding, Reliant Funding, Expansion Capital Group, Unique Funding Solutions, Yellowstone Capital / Delta Bridge.

**Platform lenders:** Stripe Capital, Square Capital, Shopify Capital, PayPal Working Capital, Amazon Lending — **embedded**, underwrite from processor data, hardest to displace.

**SBA / bank alternatives:** Live Oak Bank, Huntington, Chase, Wells Fargo SBA desks, Lendio (aggregator), Fundera (aggregator), Biz2Credit.

**Factoring / AR:** altLINE, Triumph, RTS Financial, apex capital (trucking-focused).

**Equipment financing:** Balboa Capital, Crest Capital, National Funding, Taycor.

### Competitive Positioning (as an ISO)

| If they're talking to... | Lead with... |
|--------------------------|--------------|
| A bank / SBA | Speed + approval odds |
| Another ISO | Our funder panel size, one-pull promise, renewal terms |
| OnDeck / Credibly direct | Direct is one offer; we shop 40+ |
| Square / Stripe / Shopify Capital | Platform lenders cap your advance at <10% of GMV — we go higher, and you own the receivables mix |
| Factoring | Factoring ties up invoices + notifies customers; MCA is invisible |
| LOC | LOC needs 680+ FICO and 2+ years audited financials |

---

## Compliance & Regulatory Notes

**Do's**
- Always use a signed merchant agreement; never fund on a term sheet alone.
- Disclose factor rate, purchased amount, daily/weekly payment, term in writing.
- Honor state disclosure rules: **CA SB 1235** (since 2022), **NY Commercial Finance Disclosure Law** (2024), **VA, UT** similar — they require APR-style disclosures for commercial financing.
- Respect NY COJ ban (2019) for out-of-state merchants.
- Keep PII encrypted; bank statements are highly sensitive.
- Verify ownership (25%+ owners must sign).

**Don'ts**
- Never call MCA a "loan" or quote an "interest rate" — this is a receivables purchase.
- Never inflate bank statements, alter PDFs, or coach merchants to hide positions. This is fraud and increasingly prosecuted.
- Never promise funding before underwriting approves.
- Never stack a merchant without explicit disclosure of the new position to existing funder if an inter-creditor exists.
- Never fund a restricted industry without confirming funder appetite.

---

## Data Sources for Prospecting

| Source | Use |
|--------|-----|
| Reference USA / Data Axle | Business lists by industry + revenue |
| Yelp, Google Maps | Local SMB targeting |
| UCC-1 filings | Merchants with prior MCA history (renewal candidates) — state SOS search |
| Industry associations (NRA for restaurants, ATA for trucking) | Warm audiences |
| Processor portals (if ISO has partnership) | Merchants with card volume |
| Google Ads "business loan", "working capital", "cash advance" | Inbound intent |
| Facebook / Instagram leads (SMB owners) | Geo + interest targeting |
| LinkedIn (less effective — SMB owners underrepresented) | Larger deals / $250k+ |

---

## Renewal / Retention Signals

Watch for **renewal windows** at ~50–60% paid down. These are the highest-margin deals (lower CAC, pre-qualified). Signal stack:
- Deposit trend steady or up
- No new NSFs since funding
- Clean on-time pay history
- Communicates well
- Implied use of funds went well (ask!)

---

## Glossary Quick Ref

`RTR` Right To Receive (purchased amount) · `PG` Personal Guarantee · `UCC-1` Financing statement lien · `ADB` Average Daily Balance · `NSF` Non-Sufficient Funds · `TIB` Time In Business · `ACH` Automated Clearing House · `SOS` Secretary of State · `COJ` Confession of Judgment · `MCA` Merchant Cash Advance · `LOC` Line of Credit · `MID` Merchant ID (processor) · `Splits` % of card batch held back · `Lockbox` Third-party receivables account.

---

## How This Playbook Is Used

Every `/sales` command operating in MCA context should:

1. Load this file as domain context before research or generation.
2. Replace generic "SaaS / services / e-commerce" framing with **MCA funding product** framing.
3. Use the **Five-Signal Stack** in place of BANT for `/sales qualify`.
4. Default `/sales icp` output to SMB owner-operators in A-tier industries with $50k+/mo revenue.
5. Default `/sales objections` output to the 10 MCA objections above before generic objections.
6. Use MCA-tailored outreach and proposal templates in `templates/`.

When a user invokes `/sales <cmd>` without a product description, assume MCA. When they provide a non-MCA description, fall back to generic behavior.
