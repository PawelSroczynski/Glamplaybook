# Writing in Public Strategy v3.0

**Status:** Master Strategy Document
**Updated:** December 2025
**Architect:** Paweł Sroczyński

---

## Executive Summary

This document defines a **self-liquidating evergreen funnel** built on the "writing in public" philosophy. The yurt handbook serves as the entry point to the larger **Enklava vision** — a path from consumer dependency to sovereign living.

### North Star Story

> "From renting your life to owning it — one system at a time."

The yurt is not the product. **Enklava is the story. Yurt is Chapter 1.**

---

## Table of Contents

1. [The Enklava Path](#1-the-enklava-path)
2. [Avatar Segmentation](#2-avatar-segmentation)
3. [Video Ad Scripts](#3-video-ad-scripts)
4. [Funnel Architecture](#4-funnel-architecture)
5. [Squeeze Page](#5-squeeze-page)
6. [Product Stack & Pricing](#6-product-stack--pricing)
7. [Email Sequences](#7-email-sequences)
8. [Book Series](#8-book-series)
9. [Tagging System](#9-tagging-system)
10. [Price Adjustment Protocol](#10-price-adjustment-protocol)
11. [Campaign Calibration Manual](#11-campaign-calibration-manual)
12. [Weekly Operator Checklist](#12-weekly-operator-checklist)
13. [Revenue Modeling](#13-revenue-modeling)
14. [Tech Stack](#14-tech-stack)

---

## 1. The Enklava Path

### The Vision

Enklava is a **Civilization Protocol** — an incremental transition from dependent consumerism to sovereign, off-grid resilience.

```
┌─────────────────────────────────────────────────────────────────┐
│                    THE ENKLAVA STORY                            │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   THE PROBLEM (Civilization-level)                              │
│   You rent your life from utility companies.                    │
│   Grid power. City water. Supermarket food. Bank mortgage.      │
│   One disruption and you're exposed.                            │
│                                                                 │
│   THE VISION                                                    │
│   Sovereign households. Networked communities.                  │
│   You produce what you need. You share what you have.           │
│   Resilient by design.                                          │
│                                                                 │
│   THE PATH (One system at a time)                               │
│   1. Shelter — a roof that's yours                              │
│   2. Energy — power you generate                                │
│   3. Water — supply you control                                 │
│   4. Food — land that feeds you                                 │
│   5. Knowledge — tools to keep learning                         │
│   6. Community — network that multiplies everything             │
│                                                                 │
│   THE INVITATION                                                │
│   You don't have to do it all at once.                          │
│   You start with shelter. The rest follows.                     │
│   This is Enklava.                                              │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### The Enklava Path Visual

```
    ┌─────────┐
    │ SHELTER │  ← You are here (Yurt)
    └────┬────┘
         ↓
    ┌─────────┐
    │ ENERGY  │  ← Solar, batteries, gasifier
    └────┬────┘
         ↓
    ┌─────────┐
    │  WATER  │  ← Collection, filtration, greywater
    └────┬────┘
         ↓
    ┌─────────┐
    │  FOOD   │  ← Garden, greenhouse, systems
    └────┬────┘
         ↓
    ┌─────────┐
    │KNOWLEDGE│  ← Local AI, skills, documentation
    └────┬────┘
         ↓
    ┌─────────┐
    │COMMUNITY│  ← Toloka, network, nodes
    └────┬────┘
         ↓
    ╔═════════╗
    ║ ENKLAVA ║  ← Sovereign life
    ╚═════════╝
```

### Taglines

| Option | Vibe |
|--------|------|
| "From renting your life to owning it." | Aspirational |
| "Shelter first. Sovereignty follows." | Sequential |
| "One system at a time." | Practical |
| "Build your Enklava." | Action-oriented |
| "The path to sovereign living." | Journey |

---

## 2. Avatar Segmentation

### The Four Avatars

| Avatar | Who | Goal | Yurt Role | Vision Alignment |
|--------|-----|------|-----------|------------------|
| **A** | Glamping Investor | ROI, scale business | Multiple units | Low |
| **B** | Self-Builder | DIY, live on own land | Personal dwelling | Medium |
| **C** | Special-Use Client | One yurt for specific purpose | Studio, therapy, etc. | Low |
| **D** | Enklava Builder | Full sovereign homestead + income | Everything | **High** |

### Avatar A: Glamping Investor

**Profile:** Business-minded, wants passive income, thinks in ROI

**Primary Interest:** Multiple yurts, hospitality business, franchise

**Buying Signals:** Purchases ROI Calculator, asks about occupancy rates

**Tag:** `avatar-a-investor`

**Upsell Path:** ROI Calculator → Manual 12k → Franchise

### Avatar B: Self-Builder

**Profile:** DIY mindset, wants independence, resourceful

**Primary Interest:** Build own home, live on land, off-grid systems

**Buying Signals:** Purchases Offgrid Guide, asks about materials

**Tag:** `avatar-b-builder`

**Upsell Path:** Offgrid Guide → KIT → Builder's Circle → Toloka

### Avatar C: Special-Use Client

**Profile:** Professional needing dedicated space, not interested in living off-grid

**Primary Interest:** One yurt for specific purpose

**Sub-Worlds:**

| Sub-World | Use Case | Tag |
|-----------|----------|-----|
| Wellness | Yoga studio, meditation, retreat | `avatar-c-wellness` |
| Therapy | Psychologist, counseling, coaching | `avatar-c-therapy` |
| Bodywork | Massage, physio, osteopath | `avatar-c-bodywork` |
| Creative | Art studio, music, writing | `avatar-c-creative` |
| Hospitality | Guest room, small Airbnb | `avatar-c-hospitality` |
| Coaching | Business coaching, consulting | `avatar-c-coaching` |

**Upsell Path:** Turnkey service, Design consultation

### Avatar D: Enklava Builder (Vision Carrier)

**Profile:** Wants complete sovereign homestead with income stream

**Primary Interest:** Live on land + earn from it + build all systems

**What They're Building:**

```
┌─────────────────────────────────────────────────────────────────┐
│                    AVATAR D: "MY ENKLAVA"                       │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   DWELLING                                                      │
│   └── Yurt → Climate Fortress (incremental)                     │
│                                                                 │
│   HOSPITALITY                                                   │
│   └── 1-4 guest yurts (glamping income)                         │
│                                                                 │
│   SPECIAL USE (optional)                                        │
│   └── Workshop / studio / therapy space                         │
│                                                                 │
│   UBS SYSTEMS                                                   │
│   └── Solar, water, food production, composting                 │
│                                                                 │
│   COMMUNITY CONNECTION                                          │
│   └── Toloka host, skill sharing, network node                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Their Timeline:**

| Phase | What They Build | Timeframe |
|-------|-----------------|-----------|
| 1 | First yurt (live in it) | Year 1 |
| 2 | Offgrid systems (solar, water) | Year 1-2 |
| 3 | 1-2 guest yurts (income starts) | Year 2 |
| 4 | Food systems (garden, greenhouse) | Year 2-3 |
| 5 | Climate Fortress (permanent home) | Year 3-4 |
| 6 | Scale hospitality (3-4 units) | Year 4+ |
| 7 | Special use space | When ready |

**Tag:** `avatar-d-enklava`

**Upsell Path:** Full book series → Manual 12k → KIT → Franchise / Node partnership

---

## 3. Video Ad Scripts

### Main Ad (North Star Version)

| Section | Timing | Script |
|---------|--------|--------|
| **Hook** | 0-3s | "Start living comfortably on your land fast, with only 60k in your pocket. Built in weeks, not years." |
| **Problem** | 3-15s | "But where do you even start? YouTube has a thousand videos. Forums contradict each other. You spend months lost in details — permits, insulation, stoves — and you're still not sure if it'll survive January. The information is everywhere and nowhere." |
| **Solution** | 15-35s | "I built a year-round yurt on my land in Poland. Handles -20°C winters. Legal. Under 60k in materials. A bunch of friends and a few weekends. Done. But here's the thing — the yurt was just step one." |
| **Bridge** | 35-45s | "Shelter first. Then energy. Then water. Then food. One system at a time, until your land sustains you — and maybe earns for you too. This is what I call Enklava." |
| **Offer** | 45-65s | "I'm writing down everything I've learned building 17 yurts since 2020. Three chapters are ready — free. Why this works when permits fail. Surviving your first winter. The real costs. The rest of the guide? I'm writing it now, with people building their own Enklavas." |
| **CTA** | 65-75s | "Link below. Free guide. Start your Enklava." |

### Avatar C Variations

#### Yoga / Wellness

| Section | Script |
|---------|--------|
| **Hook** | "Your yoga practice deserves more than a rented room with fluorescent lights." |
| **Problem** | "You share walls with spin classes. You negotiate time slots. You set up and tear down every session. The space doesn't match the energy you bring — and your students feel it." |
| **Solution** | "Imagine a yurt in your garden. A wooden circle. Natural light through the crown. Warm in winter, cool in summer. Your students arrive to birdsong, not elevator music. No rent. No scheduling. Your practice, your space, your terms." |
| **Offer** | "I've built 17 yurts since 2020. Three chapters are ready — free. How to get one on your land legally. What it actually costs. How it survives Polish winters. This is step one of Enklava — shelter first, then the systems that make it sovereign." |
| **CTA** | "Link below. Free guide. Build your practice space." |

**Tag:** `avatar-c-wellness`

#### Therapy / Counseling

| Section | Script |
|---------|--------|
| **Hook** | "A private practice that actually feels private." |
| **Problem** | "You rent an office in a building. Thin walls. Your clients hear the dentist next door. The waiting room is shared. Is this really where healing happens?" |
| **Solution** | "A yurt in your garden. Separate entrance — clients never enter your home. Sound-dampened walls. Nature outside the window. Thirty seconds from your kitchen. Your practice, rooted where you live." |
| **Offer** | "I've helped therapists, coaches, and counselors build exactly this. Three free chapters: legal setup, real costs, winter-proof design. The rest of the guide? I'm writing it now — with questions from people like you." |
| **CTA** | "Link below. Free guide. Your practice, your land." |

**Tag:** `avatar-c-therapy`

#### Massage / Bodywork

| Section | Script |
|---------|--------|
| **Hook** | "Stop commuting to your own business." |
| **Problem** | "You rent a room by the hour. You carry your table across town. You pay for space you use twenty hours a week. The overhead eats your margins, and the commute eats your energy." |
| **Solution** | "A yurt in your garden. Heated floor. Ambient lighting. Your table stays set up. Clients park on your driveway and walk into calm — not a strip mall. Zero commute. Full control. You keep what you earn." |
| **Offer** | "I built this for myself. Now I'm writing the complete guide. Three chapters are free: permits, costs, winter heating. If you've got land or a big garden, this could be your clinic by next season." |
| **CTA** | "Link below. Free guide. Build your treatment room." |

**Tag:** `avatar-c-bodywork`

#### Creative Studio

| Section | Script |
|---------|--------|
| **Hook** | "Your art deserves a room of its own." |
| **Problem** | "You paint in the garage. You write at the kitchen table. Your studio is wherever the kids aren't. The creative space you dream of stays a dream — because building one feels impossible." |
| **Solution** | "A yurt is 28 square meters of yours. Natural light from above. Wood walls. Silence. A space your brain recognizes as 'work happens here.' You walk across the garden and you're in the zone. No commute. No coworking. No compromise." |
| **Offer** | "I've built 17 yurts. Three chapters are ready — free. What it costs, how it's legal, how it stays warm. This could be your studio before next winter." |
| **CTA** | "Link below. Free guide. Build your creative space." |

**Tag:** `avatar-c-creative`

#### Guest Accommodation / Small Airbnb

| Section | Script |
|---------|--------|
| **Hook** | "Turn your garden into a guest suite — without a construction crew." |
| **Problem** | "Your in-laws sleep on the couch. Your Airbnb idea stays an idea. Building an extension costs a fortune, takes a year, and needs permits you'll never get." |
| **Solution** | "A yurt goes up in a weekend. Sleeps two. Heated. Cozy. Legal under Polish recreation rules. Your guests get privacy. You get your house back. Or you list it and let it pay for itself." |
| **Offer** | "I've built 17 of these. The free guide covers: legal setup, real costs, year-round comfort. Three chapters. Yours now." |
| **CTA** | "Link below. Free guide. Add a guest room this year." |

**Tag:** `avatar-c-hospitality`

#### Coaching / Consulting

| Section | Script |
|---------|--------|
| **Hook** | "Coach from a space that matches your message." |
| **Problem** | "You talk about transformation on Zoom calls from your bedroom. You preach presence while sitting in front of a bookshelf backdrop. Your space says 'working from home' — not 'this is where change happens.'" |
| **Solution** | "A yurt is a circle. No corners. Natural materials. A space your clients feel the moment they see it on camera — or step into it in person. A place that says: this work matters." |
| **Offer** | "Three free chapters: how it's legal, what it costs, how it handles winter. I'm building this guide in public — your questions shape the next chapters." |
| **CTA** | "Link below. Free guide. Build your coaching space." |

**Tag:** `avatar-c-coaching`

#### Avatar D: Enklava Builder

| Section | Script |
|---------|--------|
| **Hook** | "What if your land paid for itself — while you lived on it?" |
| **Problem** | "You dream of homesteading, but the math doesn't work. Land costs money. Building costs money. And you're supposed to wait years before any income? Most people give up before they start." |
| **Solution** | "I built a yurt, moved onto my land, then added two more for guests. Within 18 months, the glamping income covered my costs. Now I'm building the permanent house — funded by the land itself. Solar, water, food systems — all incremental. No massive loan. No waiting." |
| **Offer** | "I wrote down the whole sequence. Three chapters free: how to start legal, what it really costs, how to survive the first winter. The rest? I'm writing it with people who are building their own Enklavas right now. This is the framework — shelter, energy, water, food, income. One system at a time." |
| **CTA** | "Link below. Free guide. Start your Enklava." |

**Tag:** `avatar-d-enklava`

---

## 4. Funnel Architecture

### Complete Flow — All YES/NO Paths

```
┌─────────────────────────────────────────────────────────────────┐
│                         VIDEO AD                                │
│                      (60-75 seconds)                            │
└────────────────────────────┬────────────────────────────────────┘
                             ↓
┌─────────────────────────────────────────────────────────────────┐
│                       SQUEEZE PAGE                              │
│                                                                 │
│  "Year-Round Yurt Handbook"                                     │
│   3 free chapters + join the Enklava path                       │
│                                                                 │
│                       PRICE: FREE                               │
│                  Target: 100% of clicks                         │
│                                                                 │
│  [Email] → [START YOUR ENKLAVA]                                 │
│                                                                 │
│  Tag: `lead-new`                                                │
└────────────────────────────┬────────────────────────────────────┘
                             ↓
┌─────────────────────────────────────────────────────────────────┐
│                          OTO PAGE                               │
│                                                                 │
│  "Glamping ROI Calculator + Investor Kit"                       │
│                                                                 │
│  • ROI modeling spreadsheet                                     │
│  • Occupancy & pricing scenarios                                │
│  • Breakeven calculator                                         │
│  • Legal safety checklist                                       │
│                                                                 │
│                      PRICE: 47 PLN                              │
│                    Target: 15-22%                               │
│                                                                 │
│         [YES - 47 PLN]              [NO THANKS]                 │
│              │                           │                      │
│    Tag: `buyer-oto`              Tag: `lead-cold`               │
│    Tag: `avatar-a-investor`                                     │
└────────────────┬───────────────────────────┬────────────────────┘
                 ↓                           ↓
┌────────────────────────────────┐ ┌─────────────────────────────────┐
│         UPSELL #1              │ │         DOWNSELL #1             │
│                                │ │                                 │
│  "Offgrid Systems Guide"       │ │  "Just the Legal Guide"         │
│                                │ │                                 │
│  • Solar sizing basics         │ │  • The 70m² loophole            │
│  • Water collection & filter   │ │  • Permit vs notification       │
│  • Heating (wood stove)        │ │  • Zoning classification        │
│  • Composting sanitation       │ │  • Risk mitigation checklist    │
│  • Ventilation essentials      │ │                                 │
│                                │ │                                 │
│      PRICE: 67 PLN             │ │      PRICE: 27 PLN              │
│   Target: 25-30% of OTO        │ │   Target: 15-20% of rejecters   │
│                                │ │                                 │
│  Tag: `buyer-offgrid`          │ │  Tag: `buyer-legal`             │
│  Tag: `avatar-b-diy`           │ │  Tag: `needs-legal`             │
│                                │ │                                 │
│     [YES]          [NO]        │ │       [YES]          [NO]       │
└────────┬────────────┬──────────┘ └──────────┬────────────┬─────────┘
         ↓            ↓                       ↓            ↓
┌─────────────────┐ ┌─────────────────┐ ┌─────────────────┐ ┌─────────┐
│   UPSELL #2     │ │  DOWNSELL #1B   │ │   UPSELL #2     │ │ THANK   │
│                 │ │                 │ │                 │ │  YOU    │
│ "Builder's      │ │ "Offgrid Mini"  │ │ "Builder's      │ │         │
│  Circle"        │ │                 │ │  Circle"        │ │ Free    │
│                 │ │ • Solar basics  │ │                 │ │ only    │
│ • Priority Q&A  │ │ • Water basics  │ │ • Priority Q&A  │ │         │
│ • Your Qs →     │ │ • Heating quick │ │ • Your Qs →     │ │  END    │
│   chapters      │ │                 │ │   chapters      │ │         │
│ • Monthly call  │ │ PRICE: 37 PLN   │ │ • Monthly call  │ │ Tag:    │
│ • Early access  │ │                 │ │ • Early access  │ │`lead-   │
│ • Toloka access │ │ Tag: `avatar-b- │ │ • Toloka access │ │ cold`   │
│                 │ │       budget`   │ │                 │ │         │
│ PRICE: 47 PLN   │ │                 │ │ PRICE: 47 PLN   │ └─────────┘
│ (first month)   │ │ Target: 20-25%  │ │ (first month)   │
│ then 67 PLN/mo  │ │                 │ │ then 67 PLN/mo  │
│                 │ │                 │ │                 │
│ Tag: `community-│ │ [YES]    [NO]   │ │ Target: 10-15%  │
│       member`   │ └───┬────────┬────┘ │                 │
│                 │     ↓        ↓      │ [YES]    [NO]   │
│ Target: 10-15%  │     │        │      └──┬─────────┬────┘
│                 │     │        │         ↓         ↓
│ [YES]    [NO]   │     │        │     ┌──────┐  ┌──────┐
└──┬─────────┬────┘     │        │     │THANK │  │THANK │
   ↓         ↓          │        │     │ YOU  │  │ YOU  │
┌──────┐ ┌──────────┐   │        │     │      │  │      │
│THANK │ │DOWNSELL  │   │        │     │ END  │  │ END  │
│ YOU  │ │   #2     │   │        │     └──────┘  └──────┘
│      │ │          │   │        │
│ END  │ │"Community│   │        │
│      │ │  Trial"  │   │        │
│ Tag: │ │          │   │        │
│`avatar│ │ • 7-day  │   │        │
│-c-   │ │   access │   │        │
│engin-│ │ • 1 live │   │        │
│eer`* │ │   Q&A    │   │        │
│      │ │          │   │        │
└──────┘ │ PRICE:   │   │        │
         │ 17 PLN   │   │        │
         │          │   │        │
         │ Target:  │   │        │
         │ 15-20%   │   │        │
         │          │   │        │
         │[YES][NO] │   │        │
         └─┬────┬───┘   │        │
           ↓    ↓       │        │
       ┌──────┐┌──────┐ │        │
       │THANK ││THANK │ │        │
       │ YOU  ││ YOU  │ │        │
       │ END  ││ END  │ │        │
       └──────┘└──────┘ │        │
                        ↓        ↓
                ┌─────────────────┐    ┌──────────┐
                │   UPSELL #2     │    │  THANK   │
                │ "Builder's      │    │   YOU    │
                │  Circle"        │    │   END    │
                │ PRICE: 47 PLN   │    └──────────┘
                │                 │
                │ [YES]    [NO]   │
                └──┬─────────┬────┘
                   ↓         ↓
               ┌──────┐  ┌──────┐
               │THANK │  │THANK │
               │ YOU  │  │ YOU  │
               │ END  │  │ END  │
               └──────┘  └──────┘
```

*If bought OTO + Offgrid + Community → upgrade to `avatar-c-engineer` or `avatar-d-enklava`

### Thank You Page

```
┌─────────────────────────────────────────────────────────────────┐
│                       THANK YOU PAGE                            │
│                      (All paths end here)                       │
│                                                                 │
│  "Check your email for your downloads"                          │
│                                                                 │
│  SURVEY: "What's your goal?"                                    │
│                                                                 │
│  ○ Run a glamping business → `avatar-a`                         │
│  ○ Build my own home on land → `avatar-b`                       │
│  ○ One yurt for specific use → `avatar-c`                       │
│  ○ Live on land + earn + build all systems → `avatar-d`         │
│                                                                 │
│  QUESTION: "What's your #1 question about building on land?"    │
│                                                                 │
│  → Answers feed "writing in public" process                     │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## 5. Squeeze Page

### North Star Version

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│                         ENKLAVA                                 │
│          "From renting your life to owning it."                 │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   It starts with shelter.                                       │
│                                                                 │
│   A year-round yurt. 60,000 PLN. Built in weeks.                │
│   Legal. Warm in winter. Yours.                                 │
│                                                                 │
│   Three chapters. Free.                                         │
│                                                                 │
│   ☑ Why this works when permits fail                            │
│   ☑ Surviving your first Polish winter                          │
│   ☑ The real costs — no bullshit                                │
│                                                                 │
│   This is step one of the Enklava path.                         │
│   Shelter → Energy → Water → Food → Sovereignty.                │
│                                                                 │
│   [Email]                                                       │
│   [START YOUR ENKLAVA]                                          │
│                                                                 │
│   "Join 147 people building their Enklavas right now."          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## 6. Product Stack & Pricing

### Funnel Products

| Step | Product | Price (PLN) | Price (€) | Target Conv. |
|------|---------|-------------|-----------|--------------|
| Lead Magnet | 3 Free Chapters | 0 | 0 | 100% |
| OTO | ROI Calculator + Investor Kit | 47 | ~11 | 15-22% |
| Upsell #1 | Offgrid Systems Guide | 67 | ~15 | 25-30% of OTO |
| Downsell #1 | Legal Mini Guide | 27 | ~6 | 15-20% of rejecters |
| Downsell #1B | Offgrid Mini | 37 | ~8 | 20-25% of Upsell #1 rejecters |
| Upsell #2 | Builder's Circle (1st month) | 47 | ~11 | 10-15% |
| Downsell #2 | Community Trial (7 days) | 17 | ~4 | 15-20% of Upsell #2 rejecters |

### Backend Products

| Product | Price (PLN) | Price (€) | Timeline |
|---------|-------------|-----------|----------|
| Full Book (Digital) | 150-200 | ~35-45 | Week 3-4 |
| Full Book (Physical) | 150 | ~35 | Presale Month 2 |
| Builder's Circle (ongoing) | 67/month | ~15/mo | Ongoing |
| Manual 12k (Full SOPs) | 12,000 | ~2,700 | Month 2-3 |
| KIT (Materials + Guide) | 25,000-40,000 | ~5,700-9,000 | Month 3+ |
| Turnkey Service | 60,000+ | ~13,500+ | On request |
| Franchise License | 50,000+ | ~11,000+ | Month 6+ |

---

## 7. Email Sequences

### Story Arc Across Touchpoints

| Touchpoint | Story Beat |
|------------|------------|
| **Ad** | "There's a path. It starts with shelter." |
| **Squeeze Page** | "This is Enklava. Shelter first." |
| **OTO Page** | "Know your numbers before you build." |
| **Email Day 1** | "Welcome to the path." |
| **Email Day 7** | "What comes after shelter? Energy." |
| **Email Day 14** | "The full Enklava framework." |
| **Builder's Circle** | "Build with others on the same path." |
| **Toloka** | "The community that builds together." |
| **Book Series** | Each book = one system on the path |
| **Franchise** | "Become an Enklava node." |

### Avatar A: Glamping Investor

| Day | Subject | Content |
|-----|---------|---------|
| 0 | "Your ROI Calculator is ready" | Deliver + quick win tutorial |
| 2 | "How Marek hit 78% occupancy in year 1" | Case study |
| 5 | "The legal setup that protects your asset" | Legal framework |
| 8 | "What a 4-yurt glamping site actually costs" | Full P&L breakdown |
| 12 | "Ready to scale? Franchise options" | High-ticket intro |
| 20 | "Manual 12k: Everything for your builder" | Upsell SOPs |

### Avatar B: Self-Builder

| Day | Subject | Content |
|-----|---------|---------|
| 0 | "Your Offgrid Guide is ready" | Deliver + first steps |
| 2 | "How Ania built her yurt with 3 friends" | Story + photos |
| 5 | "The tools you actually need (skip the rest)" | Practical list |
| 8 | "Where to source materials in Poland" | Supplier guide |
| 12 | "Join a build — Toloka community projects" | Toloka invite |
| 20 | "KIT option: We prep, you build" | Upsell KIT |

### Avatar C: Special-Use

| Day | Subject | Content |
|-----|---------|---------|
| 0 | "Your guide is ready" | Deliver + use-case tips |
| 3 | "How [therapist/yoga teacher] built their space" | Case study from their world |
| 7 | "Permits for commercial use — what you need" | Practical legal |
| 14 | "Need it done for you?" | Turnkey service intro |
| 21 | "The bigger picture (if you're curious)" | Soft Enklava intro |

### Avatar D: Enklava Builder

| Day | Subject | Content |
|-----|---------|---------|
| 0 | "Your first step on the Enklava path" | Deliver + roadmap |
| 3 | "How I funded my homestead with glamping" | Your story |
| 7 | "The 18-month plan: live + earn from land" | Phase breakdown |
| 12 | "What system are you building first?" | Engagement |
| 18 | "Builder's Circle: build with others doing this" | Community pitch |
| 25 | "Toloka: find help, offer skills" | Platform intro |
| 35 | "The Enklava framework: where this is going" | Full vision |
| 50 | "KIT options: we prep, you build" | High-ticket |
| 90 | "Franchise: become an Enklava node" | Top of ladder |

### Cold Leads (No Purchase)

| Day | Subject | Content |
|-----|---------|---------|
| 0 | "Your 3 chapters are ready" | Deliver lead magnet |
| 3 | "Most people get stuck here..." | Address objections |
| 7 | "Still thinking about land life?" | Re-engagement |
| 14 | "Last chance: ROI Calculator (24h)" | Scarcity re-offer |
| 21 | "What's YOUR biggest question?" | Engagement ask |
| 30 | "This is why people wait too long" | Story-based nudge |

---

## 8. Book Series

### The Enklava Path — Book by Book

| Book | Title | Story Role | Focus |
|------|-------|------------|-------|
| 1 | **Year-Round Yurt** | Chapter 1: Shelter | Entry point, yurt construction |
| 2 | **Offgrid Systems** | Chapter 2: Energy + Water | Solar, batteries, water systems |
| 3 | **Land & Food** | Chapter 3: Cultivation | Garden, greenhouse, food production |
| 4 | **Climate Fortress** | Chapter 4: Permanent Home | Prefab strawbale, thermal mass |
| 5 | **The Enklava Protocol** | Chapter 5: Full Stack | Community, network, sovereignty |

### Writing in Public Model

**Time-Lag Protocol:**

- **Real-Time (Paid):** Builder's Circle members get immediate access to drafts, CAD, BOMs
- **12-Month Delay (Free):** Version 1.0 released to public as open content

**Community Input:**

- Questions from readers shape upcoming chapters
- Most common questions become priority content
- Contributors acknowledged in book

---

## 9. Tagging System

### Purchase-Based Tags

| Purchase Combination | Tags Applied |
|---------------------|--------------|
| Nothing | `lead-cold` |
| Legal Mini only | `lead-cold`, `needs-legal`, `buyer-legal` |
| OTO only | `buyer-oto`, `avatar-a-investor` |
| OTO + Offgrid | `buyer-oto`, `buyer-offgrid`, `avatar-b-diy` |
| OTO + Community | `buyer-oto`, `community-member`, `avatar-a-investor` |
| OTO + Offgrid + Community | `buyer-oto`, `buyer-offgrid`, `community-member`, `avatar-d-enklava` |
| OTO + Offgrid Mini | `buyer-oto`, `avatar-b-budget` |
| Downsell + Community | `buyer-legal`, `community-member`, `needs-legal` |

### Survey-Based Tags

| Survey Response | Tag |
|-----------------|-----|
| "Run a glamping business" | `avatar-a-investor` |
| "Build my own home on land" | `avatar-b-builder` |
| "One yurt for specific use" | `avatar-c-special` |
| "Live + earn + build all systems" | `avatar-d-enklava` |

### Avatar C Sub-Tags

| Use Case | Tag |
|----------|-----|
| Yoga / meditation / retreat | `avatar-c-wellness` |
| Therapy / counseling / coaching | `avatar-c-therapy` |
| Massage / bodywork | `avatar-c-bodywork` |
| Art / music / creative | `avatar-c-creative` |
| Guest accommodation / Airbnb | `avatar-c-hospitality` |
| Business coaching | `avatar-c-coaching` |

---

## 10. Price Adjustment Protocol

### Calibration Tiers by CPL

| CPL Range | OTO | Upsell #1 | Downsell #1 | Downsell #1B | Upsell #2 | Downsell #2 |
|-----------|-----|-----------|-------------|--------------|-----------|-------------|
| 0-15 PLN | 47 | 67 | 27 | 37 | 47 | 17 |
| 15-25 PLN | 67 | 97 | 37 | 47 | 67 | 27 |
| 25-35 PLN | 97 | 127 | 47 | 67 | 97 | 37 |
| 35-45 PLN | 147 | 167 | 67 | 97 | 127 | 47 |
| >45 PLN | **PAUSE** | — | — | — | — | — |

### Conversion-Based Adjustments

| Metric | Threshold | Action |
|--------|-----------|--------|
| TSR (OTO) < 10% | Too low | Lower OTO to 37 PLN floor, test copy |
| TSR (OTO) > 30% | Very high | Test raising to next tier |
| Bump rate < 15% | Too low | Lower bump price, reposition as bonus |
| Downsell < 10% | Too low | Lower to floor price, test urgency |

### Decision Tree

```
CPL Check (7-day average)
    │
    ├── < 15 PLN → Scale budget +25%
    │
    ├── 15-25 PLN → Maintain, optimize creatives
    │
    ├── 25-35 PLN → Raise prices one tier
    │
    ├── 35-45 PLN → Apply ceiling prices
    │
    └── > 45 PLN → PAUSE campaigns, diagnose
```

---

## 11. Campaign Calibration Manual

### Automated Rules (Meta Ads Manager)

| Rule | Trigger | Action |
|------|---------|--------|
| CPL Alert | CPL > 35 PLN (3-day avg) | Notify operator |
| Kill Switch | CPL > 50 PLN (7-day avg) | Auto-pause campaign |
| Scale Winners | CPL < 12 PLN (7-day avg) | Increase budget +20% (max 3x) |
| Kill Losers | Spent > 100 PLN, 0 leads | Auto-pause ad set |
| Frequency Cap | Frequency > 3.0 | Alert: audience fatigue |

### A/B Testing Protocol

**Always test:**
1. Hook variations (first 3 seconds)
2. Thumbnail images
3. CTA text
4. Audience segments

**Test duration:** Minimum 100 impressions per variant before decisions

**Winner criteria:** Statistical significance or 20%+ difference in CPL

### Audience Strategy

**Cold Audiences:**

| Audience | Description |
|----------|-------------|
| Dreamers | Homesteading, off-grid, tiny houses, permaculture |
| Investors | Glamping, Airbnb hosts, passive income, rural tourism |
| Special-Use | Yoga teachers, therapists, massage therapists, coaches |

**Retargeting:**

| Audience | Window | Use |
|----------|--------|-----|
| Blog visitors | 1-7 days | Path B warm-up |
| Squeeze visitors (no signup) | 1-14 days | Re-engagement |
| OTO rejectors | 1-30 days | Downsell campaigns |

---

## 12. Weekly Operator Checklist

### Monday: Metrics Review

- [ ] Pull 7-day CPL average
- [ ] Check TSR (OTO conversion rate)
- [ ] Review Bump and Downsell rates
- [ ] Calculate RPL (Revenue Per Lead)
- [ ] Check overall ROAS

### Tuesday: Creative Audit

- [ ] Review CTR by ad creative
- [ ] Check frequency scores
- [ ] Identify fatigued creatives (frequency > 3)
- [ ] Queue new creatives if needed

### Wednesday: Funnel Audit

- [ ] Check page load speeds
- [ ] Review squeeze → OTO conversion
- [ ] Check email deliverability
- [ ] Monitor cart abandonment

### Thursday: Price Calibration

- [ ] Compare CPL to calibration tiers
- [ ] Adjust prices if threshold crossed
- [ ] Document any changes

### Friday: Reporting & Planning

- [ ] Weekly summary report
- [ ] Compare to previous week
- [ ] Plan next week's tests
- [ ] Update content calendar (writing in public)

### Monthly: Strategic Review

- [ ] Avatar distribution analysis
- [ ] High-ticket pipeline check
- [ ] Community growth (Builder's Circle)
- [ ] Content production progress (book chapters)

---

## 13. Revenue Modeling

### Revenue Per 100 Leads (Conservative)

| Scenario | Path | Buyers | Revenue (PLN) |
|----------|------|--------|---------------|
| Full stack | OTO + Offgrid + Community | 3 | 483 |
| OTO + Offgrid | OTO + Upsell #1 | 4 | 456 |
| OTO + Community | OTO + Upsell #2 | 2 | 188 |
| OTO + Offgrid + Trial | OTO + Upsell #1 + Downsell #2 | 2 | 262 |
| OTO only | OTO | 5 | 235 |
| OTO + Mini + Community | OTO + Downsell #1B + Upsell #2 | 1 | 131 |
| OTO + Mini | OTO + Downsell #1B | 1 | 84 |
| Downsell + Community | Downsell #1 + Upsell #2 | 2 | 148 |
| Downsell only | Downsell #1 | 3 | 81 |
| Free only | — | 77 | 0 |
| **TOTAL** | | **100** | **~2,068 PLN** |

**RPL (Revenue Per Lead): ~20.68 PLN**

### Break-Even Analysis

| CPL | RPL Required | Status |
|-----|--------------|--------|
| 15 PLN | 15 PLN | Profitable at 20.68 RPL ✓ |
| 20 PLN | 20 PLN | Profitable at 20.68 RPL ✓ |
| 25 PLN | 25 PLN | Need price tier increase |
| 30 PLN | 30 PLN | Need ceiling prices |

### Lifetime Value by Avatar

| Avatar | Immediate | 90-day | 1-year | 3-year |
|--------|-----------|--------|--------|--------|
| A (Investor) | 47-114 PLN | 200-500 PLN | 12,000+ PLN | 50,000+ PLN |
| B (Builder) | 47-114 PLN | 200-800 PLN | 25,000+ PLN | 40,000+ PLN |
| C (Special) | 27-114 PLN | 100-200 PLN | 200 PLN | 200 PLN |
| D (Enklava) | 114-161 PLN | 500-2,000 PLN | 40,000+ PLN | 100,000+ PLN |

---

## 14. Tech Stack

### Minimum Viable Stack

| Tool | Purpose | Cost |
|------|---------|------|
| Carrd / Webflow | Squeeze + OTO pages | 0-20 USD/mo |
| MailerLite / ConvertKit | Email sequences + tagging | 0-30 USD/mo |
| Stripe / TPay | Payment processing | 2.9% + 0.30 |
| Meta Ads Manager | Traffic | Variable |
| Plausible / GA4 | Analytics | 0-10 USD/mo |
| **Total fixed** | | **~50-100 PLN/mo + 3%** |

### Recommended Upgrades

| Tool | Purpose | When |
|------|---------|------|
| Skool / Circle | Community platform | When Builder's Circle launches |
| Notion / Airtable | Product delivery | When digital products scale |
| Zapier | Automation | When volume increases |
| Hotjar | Funnel optimization | When testing at scale |

---

## Implementation Roadmap

### Phase 1: Calibration (Weeks 1-4)

- [ ] Build squeeze page
- [ ] Create lead magnet (3 chapters PDF)
- [ ] Build OTO page + ROI Calculator
- [ ] Set up email sequence (cold leads)
- [ ] Create first video ad
- [ ] Launch with 1,500 PLN budget
- [ ] Target: Find profitable configuration

### Phase 2: Stabilization (Month 2-3)

- [ ] Scale to 2,000-3,000 PLN/month
- [ ] Add Upsell/Downsell pages
- [ ] Segment email sequences by avatar
- [ ] Publish first 3 blog chapters (SEO)
- [ ] Launch Builder's Circle
- [ ] Target: 200+ leads/month, positive ROI

### Phase 3: Evergreen (Month 4+)

- [ ] Organic traffic growing
- [ ] Blended CPL dropping
- [ ] Community active
- [ ] First high-ticket sales
- [ ] Avatar C variations live
- [ ] Target: 500+ leads/month, sustainable growth

---

## Appendix: All Possible Buyer Journeys

| # | Path | Products | Total Revenue |
|---|------|----------|---------------|
| 1 | YES → YES → YES | OTO + Offgrid + Community | 161 PLN |
| 2 | YES → YES → NO → YES | OTO + Offgrid + Trial | 131 PLN |
| 3 | YES → YES → NO → NO | OTO + Offgrid | 114 PLN |
| 4 | YES → NO → YES → YES | OTO + Mini + Community | 131 PLN |
| 5 | YES → NO → YES → NO → YES | OTO + Mini + Trial | 101 PLN |
| 6 | YES → NO → YES → NO → NO | OTO + Mini | 84 PLN |
| 7 | YES → NO → NO → YES | OTO + Community | 94 PLN |
| 8 | YES → NO → NO → NO → YES | OTO + Trial | 64 PLN |
| 9 | YES → NO → NO → NO → NO | OTO only | 47 PLN |
| 10 | NO → YES → YES | Downsell + Community | 74 PLN |
| 11 | NO → YES → NO → YES | Downsell + Trial | 44 PLN |
| 12 | NO → YES → NO → NO | Downsell only | 27 PLN |
| 13 | NO → NO | Free only | 0 PLN |

---

**Document Version:** 3.0
**Last Updated:** December 2025
**Next Review:** After Phase 1 completion
