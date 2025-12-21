# Writing in Public: Lead Magnet Strategy v2.0

**Document:** Paid Evergreen Funnel Strategy
**Based on:** Analiza Strategii Marketingowej Jurt.docx
**Goal:** Self-liquidating evergreen funnel with calibration levers

---

## Glossary

| Term | Definition |
|------|------------|
| **CPL** | Cost Per Lead — ad spend divided by leads captured |
| **TSR** | Thank-you page Sales Rate — % of leads who buy OTO immediately after opt-in |
| **OTO** | One-Time Offer — tripwire product shown on thank-you page |
| **RPL** | Revenue Per Lead — total revenue from OTO + Bump + Downsell per lead |
| **Bump** | Add-on offer shown as checkbox on OTO page |
| **Downsell** | Lower-priced offer shown if OTO is rejected |
| **SLO** | Self-Liquidating Offer — funnel where RPL ≥ CPL (breakeven or profit) |

---

## Part I: Funnel Strategy

### 1.1 Paid Evergreen Model (Two Paths)

**Core Concept:** All traffic is PAID. Blog chapters exist as retargeting fuel, not organic discovery.

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    PAID EVERGREEN FUNNEL (TWO PATHS)                    │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  ┌─────────────────────────────────────────────────────────────────┐    │
│  │                         VIDEO ADS                                │    │
│  │         (CTA: "Join the creation of the Yurt Handbook")         │    │
│  └─────────────────────────────┬───────────────────────────────────┘    │
│                                │                                        │
│                ┌───────────────┴───────────────┐                        │
│                │                               │                        │
│                ▼                               ▼                        │
│  ┌─────────────────────────┐     ┌─────────────────────────┐            │
│  │      PATH A: DIRECT     │     │    PATH B: WARM-UP      │            │
│  │                         │     │                         │            │
│  │   Video Ad              │     │   Video Ad              │            │
│  │       ↓                 │     │       ↓                 │            │
│  │   Squeeze Page          │     │   Blog Chapter          │            │
│  │       ↓                 │     │   (pixel visitor)       │            │
│  │   OTO                   │     │       ↓                 │            │
│  │                         │     │   RETARGET AD           │            │
│  │                         │     │       ↓                 │            │
│  │                         │     │   Squeeze Page          │            │
│  │                         │     │       ↓                 │            │
│  │                         │     │   OTO                   │            │
│  └─────────────────────────┘     └─────────────────────────┘            │
│                │                               │                        │
│                └───────────────┬───────────────┘                        │
│                                │                                        │
│                                ▼                                        │
│                    ┌───────────────────────┐                            │
│                    │  A/B TEST BOTH PATHS  │                            │
│                    │  Optimize for best    │                            │
│                    │  RPL per path         │                            │
│                    └───────────────────────┘                            │
│                                                                         │
│  PATH A: Lower CPL, colder audience, may have lower TSR                │
│  PATH B: Higher CPL (2 touches), warmer audience, likely higher TSR    │
│                                                                         │
│  GOAL: Find which path delivers better NET (RPL - CPL)                 │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

### 1.2 Complete Funnel Architecture

```
┌─────────────────────────────────────────────────────────────────────────┐
│                         FUNNEL ARCHITECTURE v2.0                        │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  PAID TRAFFIC (100% of acquisition)                                    │
│  ├── Path A: Video Ad → Squeeze Page (direct conversion)              │
│  └── Path B: Video Ad → Blog Chapter → Retarget → Squeeze Page        │
│                                                                         │
│  ─────────────────────────────────────────────────────────────────────  │
│                                                                         │
│  SQUEEZE PAGE                                                           │
│  ├── Hook: "Join the creation of Year-Round Yurt Handbook"             │
│  ├── Value: Free Chapter 1 + Table of Contents                         │
│  ├── Segment: "What's your goal?" (A/B/C radio buttons)                │
│  └── Capture: Email + First Name                                       │
│                                                                         │
│  ─────────────────────────────────────────────────────────────────────  │
│                                                                         │
│  THANK YOU PAGE (OTO)                                                   │
│  │                                                                      │
│  ├── DYNAMIC HEADLINE (based on segment)                               │
│  │   ├── A (Investor): "Before you build... know the numbers"          │
│  │   ├── B (KIT): "Before you buy materials... know real costs"        │
│  │   └── C (DIY): "Before you cut wood... know the specs"              │
│  │                                                                      │
│  ├── CORE OTO: "Investor Essentials Kit" ──────────────── 47 PLN       │
│  │   ├── ROI Calculator (Excel/Sheets)                                 │
│  │   ├── Legal Safety Pack (PDF)                                       │
│  │   ├── MPZP Checklist                                                │
│  │   └── 360° Virtual Tour Access                                      │
│  │                                                                      │
│  ├── BUMP: "Ventilation & Technical Manual" ─────────────  67 PLN      │
│  │   ├── Heat recovery system design                                   │
│  │   ├── Insulation R-value calculator                                 │
│  │   └── Climate zone requirements                                     │
│  │   (Checkbox: "Yes, add this for only 67 PLN")                       │
│  │                                                                      │
│  ├── IF REJECT OTO → DOWNSELL PAGE                                     │
│  │   └── "Quick Start Pack" ─────────────────────────────  27 PLN      │
│  │       ├── Legal Safety Pack only                                    │
│  │       └── Basic cost estimator                                      │
│  │                                                                      │
│  └── NEGATIVE OPT-OUT                                                  │
│      "No thanks, I'll risk the legal complications"                    │
│                                                                         │
│  ─────────────────────────────────────────────────────────────────────  │
│                                                                         │
│  POST-PURCHASE UPSELL (Email sequence, Day 3)                          │
│  └── Full Digital Handbook (pre-release) ────────────────  197 PLN     │
│                                                                         │
│  ─────────────────────────────────────────────────────────────────────  │
│                                                                         │
│  EMAIL NURTURE (Segment-specific)                                      │
│  ├── A: ROI case studies, legal updates, project management            │
│  ├── B: Assembly tips, material sourcing, cost breakdowns              │
│  └── C: Technical deep-dives, CAD previews, engineering details        │
│                                                                         │
│  ─────────────────────────────────────────────────────────────────────  │
│                                                                         │
│  HIGH-TICKET OFFERS (Email + Retargeting)                              │
│  ├── Manual 12k (Full SOP Package) ──────────────────────  12,000 PLN  │
│  ├── KIT (Materials + Support) ──────────────────────────  varies      │
│  └── Full Service (Turnkey Build) ───────────────────────  varies      │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

### 1.3 Pricing Architecture with Calibration Levers

**Core Principle:** Multiple price points create calibration flexibility.

```
┌─────────────────────────────────────────────────────────────────────────┐
│                      PRICING CALIBRATION MATRIX                         │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  PRODUCT              │ FLOOR │ DEFAULT │ CEILING │ LEVER              │
│  ─────────────────────┼───────┼─────────┼─────────┼────────────────     │
│  OTO (Essentials)     │ 37    │ 47      │ 197     │ Main calibration   │
│  BUMP (Technical)     │ 47    │ 67      │ 147     │ Margin boost       │
│  DOWNSELL (Quick)     │ 17    │ 27      │ 97      │ Rescue conversions │
│  POST-UPSELL (Book)   │ 147   │ 197     │ 297     │ LTV extension      │
│                                                                         │
│  CALIBRATION RULES (closed ranges):                                     │
│  ─────────────────────────────────────────────────────────────────────  │
│  CPL 0.00–15.00      → Use FLOOR prices (scale mode)                   │
│  CPL 15.01–25.00     → Use DEFAULT prices                              │
│  CPL 25.01–35.00     → Raise OTO to 97, Bump to 97, Downsell to 47     │
│  CPL 35.01–45.00     → Use CEILING prices (197/147/97)                 │
│  CPL > 45.00         → PAUSE ADS, ceiling insufficient                 │
│                                                                         │
│  TSR < 15%           → Lower OTO to 37 PLN, add scarcity               │
│  Bump Rate < 15%     → Lower Bump to 47 PLN                            │
│  Downsell < 15%      → Lower Downsell to 17 PLN                        │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Part II: Financial Model

### 2.1 Revenue Per Lead Calculation

**Assumptions (Calibrated by Scenario):**

| Metric | Pessimistic | Realistic | Optimistic |
|--------|-------------|-----------|------------|
| CPL (Cost Per Lead) | **45 PLN** | 15 PLN | 10 PLN |
| OTO Price | **197 PLN** (ceiling) | 47 PLN | 47 PLN |
| OTO Conversion (TSR) | 15% | 22% | 30% |
| Bump Price | **147 PLN** (ceiling) | 67 PLN | 67 PLN |
| Bump Take Rate | 20% | 30% | 40% |
| Downsell Price | **97 PLN** (ceiling) | 27 PLN | 27 PLN |
| Downsell Rate (of rejectors) | 15% | 20% | 25% |

**Key Insight:** Pessimistic scenario uses CEILING prices. That's the whole point of calibration levers - when CPL is extremely high (45 PLN in construction niche), you raise prices to maintain breakeven.

**Revenue Per Lead (RPL) Formula:**

```
RPL = (TSR × OTO) + (TSR × Bump Rate × Bump) + ((1-TSR) × Downsell Rate × Downsell)
```

**Calculations:**

| Scenario | OTO Rev | Bump Rev | Downsell Rev | Total RPL | CPL | Net/Lead |
|----------|---------|----------|--------------|-----------|-----|----------|
| **Pessimistic** | 29.55 | 4.41 | 12.37 | **46.33 PLN** | 45 | **≈0** |
| **Realistic** | 10.34 | 4.42 | 4.21 | **18.97 PLN** | 15 | **+3.97** |
| **Optimistic** | 14.10 | 8.04 | 4.73 | **26.87 PLN** | 10 | **+16.87** |

---

### 2.2 Breakeven Analysis

**Question:** At what conversion rates do we break even for each CPL?

| CPL | Required TSR (OTO only) | Required TSR (with Bump 30%) | Required TSR (with Bump + Downsell) |
|-----|-------------------------|------------------------------|-------------------------------------|
| 10 PLN | 21.3% | 17.5% | 14.2% |
| 15 PLN | 31.9% | 26.2% | 21.3% |
| 25 PLN | 53.2% | 43.7% | 35.5% |
| 45 PLN | 95.7% | 78.6% | **15% at ceiling prices** |

**Key Insight:** At 45 PLN CPL, default prices can't break even. But with ceiling prices (197/147/97), even 15% TSR hits breakeven. That's the power of calibration.

---

### 2.3 Calibration Decision Tree

```
┌─────────────────────────────────────────────────────────────────────────┐
│                      CALIBRATION DECISION TREE                          │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  START: Run test campaign (500 PLN budget, ~25-50 leads)                │
│                                                                         │
│  ┌─────────────────────────────────────────────────────────────────┐    │
│  │  MEASURE: CPL, TSR, Bump Rate, Downsell Rate                    │    │
│  └─────────────────────────────────────────────────────────────────┘    │
│                              │                                          │
│                              ▼                                          │
│                    ┌─────────────────┐                                  │
│                    │  RPL ≥ CPL?     │                                  │
│                    └────────┬────────┘                                  │
│                             │                                           │
│              ┌──────────────┴──────────────┐                            │
│              ▼                             ▼                            │
│         ┌────────┐                    ┌────────┐                        │
│         │  YES   │                    │   NO   │                        │
│         └───┬────┘                    └───┬────┘                        │
│             │                             │                             │
│             ▼                             ▼                             │
│    ┌──────────────┐              ┌──────────────────────┐               │
│    │ SCALE UP     │              │ DIAGNOSE:            │               │
│    │ Increase     │              │ Which metric failing?│               │
│    │ ad spend     │              └──────────┬───────────┘               │
│    └──────────────┘                         │                           │
│                                  ┌──────────┼──────────┐                │
│                                  ▼          ▼          ▼                │
│                               ┌──────┐  ┌──────┐  ┌──────┐              │
│                               │ CPL  │  │ TSR  │  │ Bump │              │
│                               │ High │  │ Low  │  │ Low  │              │
│                               └──┬───┘  └──┬───┘  └──┬───┘              │
│                                  │         │         │                  │
│                                  ▼         ▼         ▼                  │
│                               ┌────────┐ ┌────────┐ ┌────────┐          │
│                               │RAISE   │ │Lower   │ │Lower   │          │
│                               │price   │ │OTO to  │ │Bump    │          │
│                               │tier    │ │floor   │ │price   │          │
│                               │(see    │ │(37 PLN)│ │to 47   │          │
│                               │matrix) │ │+scarcity│ │PLN    │          │
│                               └────────┘ └────────┘ └────────┘          │
│                                  │         │         │                  │
│                                  └─────────┴─────────┘                  │
│                                            │                            │
│                                            ▼                            │
│                                   ┌──────────────┐                      │
│                                   │ RETEST with  │                      │
│                                   │ new config   │                      │
│                                   └──────┬───────┘                      │
│                                          │                              │
│                                          ▼                              │
│                                 ┌─────────────────┐                     │
│                                 │  RPL ≥ CPL?     │──YES──▶ SCALE       │
│                                 └────────┬────────┘                     │
│                                          │NO                            │
│                                          ▼                              │
│                                 ┌─────────────────┐                     │
│                                 │ At ceiling      │──NO──▶ RAISE TO     │
│                                 │ prices?         │        CEILING      │
│                                 └────────┬────────┘                     │
│                                          │YES                           │
│                                          ▼                              │
│                                 ┌─────────────────┐                     │
│                                 │ PAUSE ADS       │                     │
│                                 │ Ceiling cannot  │                     │
│                                 │ cover CPL       │                     │
│                                 └─────────────────┘                     │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

### 2.4 Path A vs Path B Cost Comparison

**Two Parallel Paid Paths — A/B Test to Find Winner:**

| Metric | Path A (Direct) | Path B (Warm-Up) |
|--------|-----------------|------------------|
| **Flow** | Video Ad → Squeeze | Video Ad → Blog → Retarget → Squeeze |
| **Touches** | 1 | 2 (initial + retarget) |
| **Est. CPL** | 15–25 PLN | 25–40 PLN (higher due to 2 ad touches) |
| **Expected TSR** | 15–20% (cold) | 25–35% (warmer audience) |
| **Pixel Value** | Squeeze page only | Blog page + Squeeze page |

**Cost Model Example (1,000 PLN test budget each):**

| Path | Budget | Est. CPL | Leads | Est. TSR | OTO Sales | Revenue (47 PLN) |
|------|--------|----------|-------|----------|-----------|------------------|
| A | 1,000 | 20 PLN | 50 | 18% | 9 | 423 PLN |
| B | 1,000 | 35 PLN | 29 | 30% | 9 | 423 PLN |

**Key Insight:** Both paths can yield similar revenue, but:
- **Path A** = more leads, lower quality, bigger email list
- **Path B** = fewer leads, higher quality, better TSR, retargetable blog visitors

**Recommendation:** Run both in parallel. Measure NET per path (Revenue - Ad Spend). Scale the winner.

---

### 2.5 Ad Operations Playbook

**Purpose:** Clear actions for campaign operator based on measured metrics.

#### 2.5.1 Single Metric Triggers

| IF... | THEN... | TIMEFRAME |
|-------|---------|-----------|
| **CPL 0.00–15.00** | Scale budget +25%, test new audiences | After 50+ leads |
| **CPL 15.01–25.00** | Maintain, optimize creatives | Ongoing |
| **CPL 25.01–35.00** | Raise OTO to 97 PLN, Bump to 97 PLN | Within 24h |
| **CPL 35.01–45.00** | Raise to ceiling prices (197/147/97) | Within 24h |
| **CPL > 45.00** | Pause campaign, audit targeting | Immediate |
| **TSR > 25%** | Test raising OTO price +20 PLN | After 100+ leads |
| **TSR 15–25%** | Maintain current OTO price | Ongoing |
| **TSR 10–15%** | Lower OTO to floor (37 PLN), add urgency copy | Within 48h |
| **TSR < 10%** | A/B test completely new OTO offer | Within 48h |
| **Bump > 35%** | Test raising Bump price +30 PLN | After 50+ OTO sales |
| **Bump 20–35%** | Maintain current Bump price | Ongoing |
| **Bump < 20%** | Lower Bump to 47 PLN, reposition as "bonus" | Within 48h |
| **Downsell > 25%** | Test raising Downsell +20 PLN | After 50+ rejections |
| **Downsell < 15%** | Lower to 17 PLN, simplify offer | Within 48h |

---

#### 2.5.2 Combined Scenario Matrix

| CPL | TSR | Action Priority |
|-----|-----|-----------------|
| Low (<15) | High (>22%) | 🟢 **SCALE** - Increase budget aggressively |
| Low (<15) | Low (<15%) | 🟡 **FIX OTO** - Traffic quality good, offer weak |
| High (>25) | High (>22%) | 🟡 **RAISE PRICES** - Good conversion, need margin |
| High (>25) | Low (<15%) | 🔴 **PAUSE & AUDIT** - Both metrics failing |
| Mid (15-25) | Mid (15-22%) | 🟡 **OPTIMIZE** - A/B test both ads and OTO |

---

#### 2.5.3 Facebook/Meta Automation Rules

**Set up these automated rules in Meta Ads Manager:**

```
RULE 1: "CPL Alert High"
────────────────────────
Condition: Cost per Lead > 35 PLN (last 3 days)
Action: Send notification to operator
Frequency: Once per day

RULE 2: "CPL Kill Switch"
────────────────────────
Condition: Cost per Lead > 50 PLN (last 7 days)
Action: Turn off ad set
Frequency: Continuous

RULE 3: "Scale Winners"
────────────────────────
Condition: Cost per Lead < 12 PLN AND Leads > 10 (last 7 days)
Action: Increase daily budget by 20%
Frequency: Once per day
Cap: Max 3x original budget

RULE 4: "Kill Losers"
────────────────────────
Condition: Spend > 100 PLN AND Leads = 0 (last 3 days)
Action: Turn off ad set
Frequency: Continuous

RULE 5: "Frequency Cap"
────────────────────────
Condition: Frequency > 3.0 (last 7 days)
Action: Send notification (audience fatigue)
Frequency: Once per day
```

---

#### 2.5.4 Price Adjustment Protocol

**Step-by-step for operator when CPL rises:**

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    PRICE ADJUSTMENT PROTOCOL                            │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  STEP 1: Confirm CPL trend (minimum 30 leads data)                     │
│          └── Is this spike or trend? Check 7-day rolling average       │
│                                                                         │
│  STEP 2: Calculate current RPL                                         │
│          └── RPL = (TSR × OTO) + (TSR × Bump% × Bump)                  │
│                    + ((1-TSR) × Downsell% × Downsell)                  │
│                                                                         │
│  STEP 3: Compare RPL vs CPL                                            │
│          ├── RPL > CPL → Profitable, no action needed                  │
│          └── RPL < CPL → Proceed to Step 4                             │
│                                                                         │
│  STEP 4: Calculate required price increase                             │
│          └── Gap = CPL - RPL                                           │
│          └── New OTO = Current OTO + (Gap / TSR)                       │
│                                                                         │
│  STEP 5: Apply price tier                                              │
│          ├── If New OTO ≤ 97  → Set OTO = 97 PLN                       │
│          ├── If New OTO ≤ 147 → Set OTO = 147 PLN                      │
│          ├── If New OTO ≤ 197 → Set OTO = 197 PLN (ceiling)            │
│          └── If New OTO > 197 → PAUSE ADS, ceiling insufficient        │
│                                                                         │
│  STEP 6: Proportionally adjust Bump and Downsell                       │
│          ├── OTO 97  → Bump 97, Downsell 47                            │
│          ├── OTO 147 → Bump 127, Downsell 67                           │
│          └── OTO 197 → Bump 147, Downsell 97                           │
│                                                                         │
│  STEP 7: Update landing pages (use URL parameters or tool config)      │
│                                                                         │
│  STEP 8: Monitor for 48h, then re-evaluate                             │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

---

#### 2.5.5 Weekly Operator Checklist

```
□ MONDAY: Pull last 7 days data
  ├── CPL trend (up/down/stable?)
  ├── TSR trend
  ├── Bump rate
  ├── Downsell rate
  └── Calculate RPL vs CPL

□ TUESDAY: Creative audit
  ├── Which ads have highest CTR?
  ├── Which ads have lowest CPL?
  ├── Any ad with Frequency > 2.5?
  └── Plan 1-2 new creatives if needed

□ WEDNESDAY: Funnel audit
  ├── Check landing page load speed
  ├── Review OTO page conversion rate
  ├── Check email delivery rates
  └── Test all payment links

□ THURSDAY: Price calibration review
  ├── Are current prices optimal for CPL?
  ├── Any price adjustment needed?
  └── Update prices if required

□ FRIDAY: Reporting
  ├── Weekly summary to stakeholder
  ├── Net profit/loss calculation
  ├── Recommendations for next week
  └── Update tracking spreadsheet
```

---

#### 2.5.6 Escalation Matrix

| Situation | Operator Action | Escalate to Owner If... |
|-----------|-----------------|-------------------------|
| CPL spike (1 day) | Monitor, don't react | Spike lasts 3+ days |
| CPL > 45 PLN sustained | Apply ceiling prices | Still losing after 48h |
| TSR < 10% | A/B test new OTO | No improvement after 3 tests |
| Zero leads (24h) | Check pixel, landing page | Technical issue confirmed |
| Negative comments on ads | Hide, don't delete | Pattern of complaints |
| Budget depleted early | Reduce daily cap | Happening weekly |
| Competitor copying ads | Document, notify owner | Immediate |

---

#### 2.5.7 Quick Reference Card (Print This)

```
╔═══════════════════════════════════════════════════════════════════════╗
║                    ENKLAVA AD OPERATIONS CHEAT SHEET                  ║
╠═══════════════════════════════════════════════════════════════════════╣
║                                                                       ║
║  PRICE TIERS:                                                         ║
║  ┌─────────┬────────┬─────────┬─────────┐                            ║
║  │ Tier    │ OTO    │ Bump    │ Downsell│                            ║
║  ├─────────┼────────┼─────────┼─────────┤                            ║
║  │ Floor   │ 37     │ 47      │ 17      │                            ║
║  │ Default │ 47     │ 67      │ 27      │                            ║
║  │ Mid     │ 97     │ 97      │ 47      │                            ║
║  │ High    │ 147    │ 127     │ 67      │                            ║
║  │ Ceiling │ 197    │ 147     │ 97      │                            ║
║  └─────────┴────────┴─────────┴─────────┘                            ║
║                                                                       ║
║  CPL RESPONSE:                                                        ║
║  < 15 PLN  → Scale (+25% budget)                                     ║
║  15-25 PLN → Optimize (test creatives)                               ║
║  25-35 PLN → Raise to Mid tier                                       ║
║  35-45 PLN → Raise to Ceiling tier                                   ║
║  > 45 PLN  → PAUSE & ESCALATE                                        ║
║                                                                       ║
║  BREAKEVEN FORMULA:                                                   ║
║  RPL = (TSR × OTO) + (TSR × Bump% × Bump) + ((1-TSR) × DS% × DS)     ║
║  IF RPL ≥ CPL → Profitable ✓                                         ║
║  IF RPL < CPL → Raise prices or pause                                ║
║                                                                       ║
║  TARGETS:          RED FLAGS:                                         ║
║  CPL < 15          CPL > 45                                          ║
║  TSR > 22%         TSR < 10%                                         ║
║  Bump > 25%        Bump < 15%                                        ║
║  Downsell > 20%    Downsell < 10%                                    ║
║                                                                       ║
║  EMERGENCY CONTACTS:                                                  ║
║  Owner: [phone]    Tech: [phone]    Payments: [phone]                ║
║                                                                       ║
╚═══════════════════════════════════════════════════════════════════════╝
```

---

## Part III: Blog as Retargeting Fuel

### 3.1 How Blog Powers Path B

**Primary Purpose:** Warm up cold traffic before squeeze page.

```
┌─────────────────────────────────────────────────────────────────────────┐
│                    PATH B: BLOG RETARGETING FLOW                        │
├─────────────────────────────────────────────────────────────────────────┤
│                                                                         │
│  STEP 1: Video Ad (CTA: "Read how we build yurts year-round")          │
│          └── Drives to: Blog chapter (e.g., "Surviving January")       │
│                                                                         │
│  STEP 2: Blog Chapter                                                   │
│          ├── Visitor reads valuable content                            │
│          ├── Facebook Pixel fires → visitor added to custom audience   │
│          └── Soft CTA at end: "Want to join the handbook creation?"    │
│                                                                         │
│  STEP 3: Retarget Ad (shown 1-7 days later)                            │
│          ├── "You read about winter yurts. Here's what's next..."      │
│          └── CTA: Direct to squeeze page                               │
│                                                                         │
│  STEP 4: Squeeze Page → OTO → Bump → Downsell                          │
│          └── Warmer lead = higher TSR expected                         │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

**Why This Works:**
- First touch = value (blog), not ask (squeeze)
- Pixel builds retargetable audience automatically
- Second touch = familiar brand, warmer reception
- Blog readers self-qualify by topic interest

---

### 3.2 Blog Chapters for Path B

**8 Chapters = 8 Warm-Up Landing Pages**

| Chapter | Topic | Best For Avatar | Retarget Message |
|---------|-------|-----------------|------------------|
| 0.1 The Itch | Why year-round yurts | All | "Ready to take the first step?" |
| 0.2 Surviving January | Winter insulation | B, C | "Get the full insulation specs" |
| 1.1 Paper Jungle | Legal & permits | A, B | "Avoid the legal traps we discovered" |
| 2.1 Circle and Parts | Yurt anatomy | B, C | "See the full construction breakdown" |
| 4.1 First Cut | Workshop basics | C | "Access the technical manual" |
| 7.1 Before Anyone Lifts | Assembly safety | B, C | "Don't lift without this checklist" |
| 9.1 Four Seasons | Maintenance | A, B | "Protect your investment year-round" |
| 10.1 Joining Network | Franchise model | A | "Join our builder network" |

---

### 3.3 Retargeting Audience Setup (Meta Ads)

**Custom Audiences to Create:**

| Audience Name | Source | Retention | Use For |
|---------------|--------|-----------|---------|
| Blog_All_Visitors | All blog pages | 30 days | Broad retarget |
| Blog_Legal_Readers | Ch 1.1 page | 14 days | Avatar A retarget |
| Blog_Technical_Readers | Ch 2.1, 4.1, 7.1 | 14 days | Avatar C retarget |
| Blog_Winter_Readers | Ch 0.2 | 14 days | Insulation-focused retarget |
| Squeeze_Visitors_NoConvert | Squeeze page, no thank-you | 7 days | Abandonment retarget |

**Lookalike Audiences (after 500+ conversions):**
- 1% Lookalike of OTO Buyers
- 1% Lookalike of Blog_Technical_Readers

---

### 3.4 Blog SEO Bonus (Long-Term)

**Secondary benefit:** Blog posts index in Google over time.

| Chapter | Target Keyword | Est. Monthly Search (PL) |
|---------|----------------|--------------------------|
| 0.1 The Itch | "jurta całoroczna" | 500 |
| 0.2 Surviving January | "jurta zimą" | 200 |
| 1.1 Paper Jungle | "jurta pozwolenie na budowę" | 300 |
| 2.1 Circle and Parts | "budowa jurty" | 400 |

**Note:** SEO is a bonus, not the strategy. Primary acquisition remains paid ads. Any organic traffic is free bonus leads that enter the same funnel.

---

## Part IV: Implementation Roadmap

### 4.1 Phase 1: Calibration (Weeks 1-4)

**Goal:** Find profitable configuration

| Week | Action | Budget | KPIs |
|------|--------|--------|------|
| 1 | Build funnel (Squeeze + OTO + Bump + Downsell) | 0 | Funnel live |
| 2 | Launch test ads (3 creatives, 2 audiences) | 500 PLN | CPL < 20 |
| 3 | Measure conversions, first calibration | 500 PLN | TSR, Bump%, Downsell% |
| 4 | Optimize prices based on data | 500 PLN | RPL > CPL |

**Total calibration budget:** 1,500 PLN
**Expected leads:** 75-150

---

### 4.2 Phase 2: Stabilization (Weeks 5-12)

**Goal:** Consistent profitable acquisition

| Month | Paid Budget | Expected Leads | Target RPL | Target Net |
|-------|-------------|----------------|------------|------------|
| 2 | 2,000 PLN | 130-150 | 19+ PLN | +450 PLN |
| 3 | 3,000 PLN | 200-230 | 19+ PLN | +700 PLN |

**Parallel:** Launch first 2 public blog posts for SEO

---

### 4.3 Phase 3: Evergreen (Month 4+)

**Goal:** Reduce paid dependency, increase organic

| Quarter | Paid Budget | Organic Leads | Blended CPL | Net Margin |
|---------|-------------|---------------|-------------|------------|
| Q2 | 6,000 PLN | 50/month | 10 PLN | Positive |
| Q3 | 4,500 PLN | 100/month | 7 PLN | Very positive |
| Q4 | 3,000 PLN | 150/month | 5 PLN | Highly profitable |

---

## Part V: Risk Mitigation

### 5.1 Scenario Planning

| Risk | Probability | Impact | Mitigation |
|------|-------------|--------|------------|
| CPL 25-35 PLN | Medium | Medium | Raise OTO to 97-147 PLN |
| CPL 35-45 PLN | Low | High | Use ceiling prices (197/147/97) |
| CPL > 45 PLN | Very Low | Critical | Pause paid, pivot to organic only |
| TSR < 15% | Low | High | A/B test OTO copy, lower price to 37 |
| Bump < 15% | Medium | Medium | Reposition as "limited offer", lower to 47 |
| Organic slow to build | Medium | Medium | Increase paid, guest post for backlinks |
| Competition copies | Low | Low | Brand authority, community moat |

---

### 5.2 Kill Criteria

**Stop paid campaigns if after 4 weeks:**
- CPL > 45 PLN consistently (ceiling prices already in use)
- TSR < 10% after 3 A/B tests
- Combined (OTO + Bump + Downsell) < 50% of CPL at ceiling prices

**If kill criteria met:**
- Pause all paid campaigns
- Audit offer positioning, pricing, and creative
- Consider market timing (seasonality, competition)
- Resume testing with new hypothesis after 30 days

---

## Part VI: Metrics Dashboard

### 6.1 Weekly Tracking

| Metric | Target | Red Flag |
|--------|--------|----------|
| CPL | < 15 PLN | > 45 PLN |
| TSR (OTO) | > 22% | < 15% |
| Bump Rate | > 25% | < 15% |
| Downsell Rate | > 20% | < 10% |
| RPL | > 19 PLN | < CPL |
| Net per Lead | > 4 PLN | < 0 PLN (at ceiling) |

---

### 6.2 Monthly Tracking

| Metric | Target | Red Flag |
|--------|--------|----------|
| Total Leads | Growth +20% | Decline |
| Organic % | Increasing | Flat at < 10% |
| Email Open Rate | > 35% | < 20% |
| Unsubscribe Rate | < 1% | > 3% |
| High-ticket conversions | > 0 | None after 90 days |

---

## Part VII: Product Requirements

### 7.1 Assets to Create

| Asset | Priority | Est. Effort | Deadline |
|-------|----------|-------------|----------|
| Squeeze Page | P0 | 4h | Week 1 |
| OTO Page (dynamic) | P0 | 8h | Week 1 |
| Bump Page Section | P0 | 2h | Week 1 |
| Downsell Page | P0 | 4h | Week 1 |
| ROI Calculator (Sheets) | P0 | 8h | Week 1 |
| Legal Pack (PDF) | P0 | 16h | Week 1 |
| Technical Manual (Bump) | P1 | 24h | Week 2 |
| 3 Ad Creatives | P0 | 8h | Week 1 |
| Email Welcome Sequence (5) | P0 | 8h | Week 1 |
| Segment Nurture Sequences (3x5) | P1 | 24h | Week 3 |

---

### 7.2 Tech Stack

| Function | Tool | Cost |
|----------|------|------|
| Landing Pages | Carrd / Webflow | 0-20 USD/mo |
| Email | MailerLite / ConvertKit | 0-30 USD/mo |
| Payments | Stripe / TPay | 2.9% + 0.30 |
| Analytics | Plausible / GA4 | 0-10 USD/mo |
| Ads | Meta Business Suite | Variable |
| CRM Tagging | Email tool native | Included |

**Fixed monthly cost:** ~50-100 PLN
**Variable cost:** Payment processing (~3%)

---

## Summary: Key Changes from Original Strategy

| Aspect | Original | Improved |
|--------|----------|----------|
| OTO Price | Fixed 37 PLN | Flexible 37-67 PLN |
| Bump | Mentioned as idea | Core component (67 PLN) |
| Downsell | Missing | Added (27 PLN) |
| Organic layer | Not addressed | 8 public chapters SEO |
| Calibration | None | Decision tree + price matrix |
| Evergreen | Not designed | Blended CPL model |
| Risk model | Optimistic CPL | Conservative 45 PLN CPL |
| Breakeven | 27% TSR (no help) | **0 net at 45 PLN CPL** (ceiling prices) |

---

## Action Items

1. **Immediate:** Build funnel pages (Week 1)
2. **Week 2:** Launch calibration campaign (500 PLN)
3. **Week 3:** First optimization round
4. **Week 4:** Price calibration based on data
5. **Month 2:** Publish first 2 public SEO chapters
6. **Month 3:** Scale if profitable, pivot if not

---

*Document Version: 2.0*
*Created: December 2025*
*Strategy: Writing in Public as Self-Liquidating Evergreen Funnel*
