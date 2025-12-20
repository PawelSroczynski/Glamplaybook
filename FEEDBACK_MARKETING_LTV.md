# GlampModeler Ultimate — Constructive Feedback

## Marketing, LTV & Business Performance Enhancement Review

> **Review Date:** 2025-12-19
> **Scope:** Business Monitoring, Marketing Integration, Customer Lifetime Value

---

## Executive Summary

The current GlampModeler specification excels at **CapEx modeling** and **financial projections** but has significant gaps in:

| Gap Area | Current State | Impact |
|----------|---------------|--------|
| **Marketing Attribution** | Not addressed | Can't measure ROI on marketing spend |
| **Customer Acquisition** | Basic CAC mention only | No channel-level tracking |
| **LTV/Loyalty** | Single line mention | No retention modeling |
| **Discount Strategy** | Sankey shows 3% | No management system |
| **Word of Mouth** | Not addressed | Missing referral tracking |
| **Content Performance** | Not addressed | Blind content investment |

---

## PART 1: GAPS IN CURRENT SPECIFICATION

### 1.1 What's Missing — The Marketing Blindspot

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                     CURRENT vs NEEDED VISIBILITY                                │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   CURRENT STATE                          NEEDED STATE                           │
│   ══════════════                         ════════════                           │
│                                                                                 │
│   ┌─────────────┐                        ┌─────────────┐                        │
│   │   REVENUE   │                        │   REVENUE   │                        │
│   │   €18,250   │                        │   €18,250   │                        │
│   └──────┬──────┘                        └──────┬──────┘                        │
│          │                                      │                               │
│          ▼                                      ▼                               │
│   ┌─────────────┐                        ┌─────────────────────────────────┐    │
│   │  ? ? ? ? ?  │                        │  WHERE DID THEY COME FROM?      │    │
│   │  BLACK BOX  │                        │  ├── Google Ads:     €4,200     │    │
│   │             │                        │  ├── Instagram:      €3,100     │    │
│   │  "Guests    │                        │  ├── Booking.com:    €5,400     │    │
│   │   appeared" │                        │  ├── Referrals:      €2,800     │    │
│   │             │                        │  ├── Direct/Repeat:  €1,950     │    │
│   └─────────────┘                        │  └── Influencer:       €800     │    │
│                                          └─────────────────────────────────┘    │
│                                                                                 │
│   You know WHAT you earned              You know WHY you earned it              │
│   but not WHY or HOW                    and can optimize channels               │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

### 1.2 Missing Metrics in Current KPI Dashboard

**Currently tracked:**
- Occupancy, ADR, RevPAR, EBITDA, GOP, DSCR
- CAC mentioned but not operationalized

**NOT tracked (critical gaps):**

| Metric | Why It Matters |
|--------|----------------|
| **ROAS** (Return on Ad Spend) | Is your €500/month on Google Ads profitable? |
| **Channel Attribution** | Which platform brings best guests? |
| **LTV:CAC Ratio** | Is acquisition sustainable? (Target: >3:1) |
| **Referral Rate** | What % of guests come via word-of-mouth? |
| **Repeat Guest Rate** | Loyalty health indicator |
| **Content Conversion Rate** | Is organic content working? |
| **Discount Impact** | Revenue lost vs. occupancy gained |
| **Influencer ROI** | Did that free stay generate bookings? |

---

## PART 2: RECOMMENDED NEW MODULE — MARKETING COMMAND CENTER

### 2.1 Proposed Architecture Addition

```
╔═══════════════════════════════════════════════════════════════════════════════╗
║                                                                               ║
║   EXISTING THREE-LAYER MODEL                                                  ║
║   ══════════════════════════                                                  ║
║                                                                               ║
║   ┌─────────────────────────────────────────────────────────────────────┐     ║
║   │  LAYER 1: PLANNING      │  LAYER 2: OPERATIONS  │  LAYER 3: ANALYSIS│     ║
║   │  (CapEx, 10-Year)       │  (Daily KPIs)         │  (Sankey, Compare)│     ║
║   └─────────────────────────────────────────────────────────────────────┘     ║
║                                      │                                        ║
║                                      ▼                                        ║
║   ┌─────────────────────────────────────────────────────────────────────┐     ║
║   │                                                                     │     ║
║   │                    ⚡ NEW: LAYER 4 — GROWTH ENGINE                  │     ║
║   │                                                                     │     ║
║   │   ┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐        │     ║
║   │   │ Channel  │──▶│ Customer │──▶│ Loyalty  │──▶│ Referral │        │     ║
║   │   │ Tracker  │   │   LTV    │   │ Program  │   │  Engine  │        │     ║
║   │   └──────────┘   └──────────┘   └──────────┘   └──────────┘        │     ║
║   │                                                                     │     ║
║   │   Output: Attribution, ROAS, LTV:CAC, Referral Rate, Cohort Value  │     ║
║   └─────────────────────────────────────────────────────────────────────┘     ║
║                                                                               ║
╚═══════════════════════════════════════════════════════════════════════════════╝
```

---

### 2.2 Marketing Channel Tracker

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                         CHANNEL PERFORMANCE DASHBOARD                           │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   PERIOD: [This Month ▾]    COMPARE: [Last Month ▾]    CURRENCY: [EUR ▾]       │
│                                                                                 │
│   ┌─ CHANNEL MIX ───────────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   CHANNEL           BOOKINGS    REVENUE     SPEND      ROAS    TREND   │   │
│   │   ════════════════════════════════════════════════════════════════════ │   │
│   │                                                                         │   │
│   │   🔍 Google Ads        12       €4,200      €380      11.1x    ▲ +2.3  │   │
│   │      ████████████████████████████████░░░░░░░░░░                        │   │
│   │                                                                         │   │
│   │   📸 Meta (IG/FB)       8       €3,100      €290      10.7x    ▲ +1.1  │   │
│   │      ████████████████████████░░░░░░░░░░░░░░░░                          │   │
│   │                                                                         │   │
│   │   🏨 Booking.com       15       €5,400      €810       6.7x    ─  0.0  │   │
│   │      ██████████████████████████████████████████░░░░░                   │   │
│   │                                                                         │   │
│   │   🏠 Airbnb             9       €3,200      €480       6.7x    ▼ -0.8  │   │
│   │      █████████████████████████░░░░░░░░░░░░░░░░░                        │   │
│   │                                                                         │   │
│   │   👥 Referrals          7       €2,800       €0         ∞      ▲ +3    │   │
│   │      █████████████████████░░░░░░░░░░░░░░░░░░░░░   (program cost: €140) │   │
│   │                                                                         │   │
│   │   🔄 Direct/Repeat      5       €1,950       €0         ∞      ▲ +1    │   │
│   │      ██████████████░░░░░░░░░░░░░░░░░░░░░░░░░░░░                        │   │
│   │                                                                         │   │
│   │   🎬 Influencer         2        €800      €450       1.8x    NEW      │   │
│   │      ██████░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░                       │   │
│   │                                                                         │   │
│   │   🌐 Organic/SEO        4       €1,400       €0         ∞      ▲ +2    │   │
│   │      ██████████░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░                       │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ INSIGHTS ──────────────────────────────────────────────────────────────┐   │
│   │  💡 Google Ads ROAS improved 26% — consider increasing budget           │   │
│   │  ⚠️  Influencer campaign underperforming — review content strategy      │   │
│   │  🎯 Referrals growing — activate loyalty program promotion              │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

#### Channel Data Model

```typescript
interface BookingAttribution {
  bookingId: string;

  // First-touch attribution
  firstTouchChannel: Channel;
  firstTouchDate: Date;
  firstTouchCampaign?: string;

  // Last-touch attribution
  lastTouchChannel: Channel;
  lastTouchDate: Date;
  lastTouchCampaign?: string;

  // UTM tracking
  utmSource?: string;
  utmMedium?: string;
  utmCampaign?: string;
  utmContent?: string;

  // Referral tracking
  referredBy?: string; // guest ID if referral
  referralCode?: string;

  // Revenue attribution
  revenue: number;
  commission: number;
  netRevenue: number;
}

type Channel =
  | 'google_ads'
  | 'meta_ads'
  | 'booking_com'
  | 'airbnb'
  | 'direct'
  | 'referral'
  | 'influencer'
  | 'organic_search'
  | 'organic_social'
  | 'email'
  | 'other';

interface ChannelMetrics {
  channel: Channel;
  period: DateRange;

  // Volume
  impressions?: number;
  clicks?: number;
  bookings: number;
  guests: number;

  // Revenue
  grossRevenue: number;
  commission: number;
  netRevenue: number;

  // Cost
  adSpend: number;
  platformFees: number;
  totalCost: number;

  // Efficiency
  cpc?: number;           // Cost per click
  cpa: number;            // Cost per acquisition
  roas: number;           // Return on ad spend
  conversionRate: number; // Bookings / Clicks

  // Quality
  avgStayLength: number;
  avgReviewScore: number;
  repeatRate: number;
}
```

---

### 2.3 Paid Advertising Module

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                            PAID ADS COMMAND CENTER                              │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   ┌─ BUDGET ALLOCATION ─────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   MONTHLY BUDGET: €1,500                     SPENT: €1,180 (79%)       │   │
│   │   ████████████████████████████████████████░░░░░░░░░░                   │   │
│   │                                                                         │   │
│   │   PLATFORM        BUDGET    SPENT     ROAS    STATUS                   │   │
│   │   ────────────────────────────────────────────────────                 │   │
│   │   Google Ads      €600      €520     11.1x    🟢 Profitable            │   │
│   │   Meta Ads        €500      €380     10.7x    🟢 Profitable            │   │
│   │   TikTok Ads      €200      €180      3.2x    🟡 Testing               │   │
│   │   Pinterest       €200      €100      2.1x    🔴 Pause recommended     │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ CAMPAIGN PERFORMANCE ──────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   GOOGLE ADS                                                            │   │
│   │   ├── "Glamping Poland" (Search)      ROAS: 14.2x  ▲  [Scale Up]       │   │
│   │   ├── "Luxury Yurt" (Search)          ROAS:  9.8x  ─  [Maintain]       │   │
│   │   ├── "Weekend Getaway" (Display)     ROAS:  4.1x  ▼  [Optimize]       │   │
│   │   └── "Retargeting" (Display)         ROAS: 18.3x  ▲  [Scale Up]       │   │
│   │                                                                         │   │
│   │   META ADS                                                              │   │
│   │   ├── "Nature Escape" (IG Stories)    ROAS: 12.4x  ▲  [Scale Up]       │   │
│   │   ├── "Couple Retreat" (FB Feed)      ROAS:  8.2x  ─  [Maintain]       │   │
│   │   └── "Lookalike Audience"            ROAS: 11.1x  ▲  [Scale Up]       │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ SEASONALITY INSIGHTS ──────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   AD SPEND vs BOOKINGS (12-month view)                                  │   │
│   │                                                                         │   │
│   │   €800│           Spend                                                 │   │
│   │       │            ╭─╮                                                  │   │
│   │   €600│        ╭───╯ ╰───╮                    ╭───╮                     │   │
│   │       │    ╭───╯         ╰───╮          ╭────╯   │                     │   │
│   │   €400│────╯                 ╰────╮ ╭───╯        ╰────                 │   │
│   │       │                           ╰─╯                                   │   │
│   │   €200│                                                                 │   │
│   │       └────┬────┬────┬────┬────┬────┬────┬────┬────┬────┬────┬────     │   │
│   │           Jan  Feb  Mar  Apr  May  Jun  Jul  Aug  Sep  Oct  Nov  Dec   │   │
│   │                                                                         │   │
│   │   💡 INSIGHT: Reduce spend Jun-Aug (organic demand high)               │   │
│   │              Increase spend Mar-May (shoulder season boost)            │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

### 2.4 Organic Content Performance Module

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                         ORGANIC CONTENT DASHBOARD                               │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   ┌─ CONTENT FUNNEL ────────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   IMPRESSIONS          ENGAGEMENT          CLICKS           BOOKINGS   │   │
│   │      45,200      ──▶      3,800      ──▶     890      ──▶      12      │   │
│   │                   8.4%              23.4%             1.3%              │   │
│   │                                                                         │   │
│   │   ████████████████████████████████████████████████████████░░░░░░░░░░   │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ PLATFORM BREAKDOWN ────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   PLATFORM       FOLLOWERS    REACH     ENGAGE    CLICKS    BOOK       │   │
│   │   ═══════════════════════════════════════════════════════════════════  │   │
│   │                                                                         │   │
│   │   📸 Instagram     2,450     18,200     1,820      420       5         │   │
│   │      Best: Reels (3x engagement vs posts)                              │   │
│   │                                                                         │   │
│   │   📘 Facebook      1,890     12,400       680      180       3         │   │
│   │      Best: Guest story shares                                          │   │
│   │                                                                         │   │
│   │   🎬 TikTok          890      8,600       950      180       2         │   │
│   │      Best: "Day in the life" format                                    │   │
│   │                                                                         │   │
│   │   🌐 Blog/SEO         —       6,000       350      110       2         │   │
│   │      Best: "Best glamping Poland" (rank #3)                            │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ TOP PERFORMING CONTENT ────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   #   CONTENT                      TYPE      REACH    BOOK   €/BOOK    │   │
│   │   ─────────────────────────────────────────────────────────────────    │   │
│   │   1   "Sunrise from the yurt"      Reel      8,400     3     €0        │   │
│   │   2   "Winter morning routine"     TikTok    6,200     2     €0        │   │
│   │   3   "Guest review montage"       Reel      4,100     2     €0        │   │
│   │   4   "Building our yurt" story    Blog      2,800     2     €0        │   │
│   │   5   "Hot tub under stars"        Post      3,200     1     €0        │   │
│   │                                                                         │   │
│   │   💡 Content ROI: 12 bookings × €150 ADR × 2.3 nights = €4,140         │   │
│   │      Time invested: ~20 hrs/month = €207/hr effective rate             │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ CONTENT CALENDAR ──────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   MON      TUE      WED      THU      FRI      SAT      SUN            │   │
│   │   ═══════════════════════════════════════════════════════════          │   │
│   │   📸       🎬       📘       📸       🎬       📸       📘             │   │
│   │   IG Post  TikTok   Blog     IG Reel  TikTok   IG Story  FB Post       │   │
│   │                                                                         │   │
│   │   [ + Schedule Post ]  [ Content Ideas ]  [ Analytics Deep Dive ]      │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

### 2.5 Influencer Campaign Tracker

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                        INFLUENCER CAMPAIGN MANAGEMENT                           │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   ┌─ ACTIVE CAMPAIGNS ──────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   INFLUENCER         FOLLOWERS   DEAL         STATUS      ROI          │   │
│   │   ══════════════════════════════════════════════════════════════════   │   │
│   │                                                                         │   │
│   │   @nature.escapes      45K      Free stay     ✅ Posted    4.2x        │   │
│   │   ├── Posts: 3/3 delivered                                             │   │
│   │   ├── Stories: 8/5 delivered (+3 bonus)                                │   │
│   │   ├── Reach: 38,400                                                    │   │
│   │   ├── Bookings (tracked): 4                                            │   │
│   │   └── Revenue: €1,890 vs Cost: €450 (stay value)                       │   │
│   │                                                                         │   │
│   │   @travel.couple.pl    28K      €300 + stay   🔄 In progress  TBD      │   │
│   │   ├── Posts: 1/2 delivered                                             │   │
│   │   ├── Stories: 3/4 delivered                                           │   │
│   │   └── Tracking code: TRAVELCOUPLE15                                    │   │
│   │                                                                         │   │
│   │   @minimalist.living   12K      Free stay     📅 Scheduled   —         │   │
│   │   └── Visit date: Jan 15-17                                            │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ CAMPAIGN RESULTS (Last 12 Months) ─────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   Total Campaigns:        8                                             │   │
│   │   Total Investment:       €3,200 (stays + fees)                         │   │
│   │   Tracked Bookings:       18                                            │   │
│   │   Attributed Revenue:     €7,650                                        │   │
│   │   ─────────────────────────────────────                                 │   │
│   │   Overall ROAS:           2.4x                                          │   │
│   │   Avg. Cost per Booking:  €178                                          │   │
│   │                                                                         │   │
│   │   ⚠️  Below target ROAS of 3.0x                                         │   │
│   │   💡 Best performer: Micro-influencers (5-20K) avg 4.1x ROAS           │   │
│   │   💡 Worst: Macro-influencers (100K+) avg 1.2x ROAS                    │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ INFLUENCER SCORING ────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   Before partnering, evaluate:                                          │   │
│   │                                                                         │   │
│   │   ┌────────────────┐  ┌────────────────┐  ┌────────────────┐            │   │
│   │   │  RELEVANCE     │  │  ENGAGEMENT    │  │  AUTHENTICITY  │            │   │
│   │   │  ───────────   │  │  ───────────   │  │  ───────────   │            │   │
│   │   │  Travel niche? │  │  >3% rate?     │  │  Real comments?│            │   │
│   │   │  Nature focus? │  │  Active reply? │  │  No fake vibe? │            │   │
│   │   │  Similar demo? │  │  Story views?  │  │  Past collabs? │            │   │
│   │   │                │  │                │  │                │            │   │
│   │   │  Score: __/10  │  │  Score: __/10  │  │  Score: __/10  │            │   │
│   │   └────────────────┘  └────────────────┘  └────────────────┘            │   │
│   │                                                                         │   │
│   │   PARTNER IF: Total Score > 21/30                                       │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

### 2.6 Word of Mouth & Referral Engine

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                          REFERRAL PROGRAM DASHBOARD                             │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   ┌─ PROGRAM OVERVIEW ──────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   REFERRAL PROGRAM: "Share the Magic"                                   │   │
│   │                                                                         │   │
│   │   ┌─────────────────────────────────────────────────────────────────┐   │   │
│   │   │                                                                 │   │   │
│   │   │   REFERRER                              FRIEND                  │   │   │
│   │   │   ═════════                             ══════                  │   │   │
│   │   │                                                                 │   │   │
│   │   │   Gets: €50 credit                      Gets: 10% off           │   │   │
│   │   │   on next stay                          first booking           │   │   │
│   │   │                                                                 │   │   │
│   │   │              ────────▶  BOOKS  ◀────────                       │   │   │
│   │   │                                                                 │   │   │
│   │   │   Trigger: When friend completes stay (not just books)         │   │   │
│   │   │                                                                 │   │   │
│   │   └─────────────────────────────────────────────────────────────────┘   │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ REFERRAL METRICS ──────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   THIS MONTH                           ALL TIME                         │   │
│   │   ══════════                           ════════                         │   │
│   │                                                                         │   │
│   │   Referral codes sent:    45           Total codes sent:      312       │   │
│   │   Codes used:              7           Total codes used:       48       │   │
│   │   Conversion rate:      15.6%          Overall rate:        15.4%       │   │
│   │                                                                         │   │
│   │   Revenue generated:  €2,800           Total revenue:     €18,400       │   │
│   │   Credits issued:       €350           Total credits:      €2,400       │   │
│   │   NET contribution:   €2,450           NET contribution:  €16,000       │   │
│   │                                                                         │   │
│   │   ─────────────────────────────────────────────────────────────────    │   │
│   │   Cost per Referral Booking: €50 (credit only, vs €180 paid CAC)       │   │
│   │   Referral CAC is 72% cheaper than paid acquisition                    │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ TOP REFERRERS (Ambassadors) ───────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   #   GUEST              REFERRALS    REVENUE     STATUS                │   │
│   │   ─────────────────────────────────────────────────────────────────    │   │
│   │   1   Anna K.               8         €3,200      🏆 VIP Ambassador     │   │
│   │   2   Michał W.             5         €1,890      ⭐ Ambassador         │   │
│   │   3   Julia & Tom           4         €1,650      ⭐ Ambassador         │   │
│   │   4   Ewa P.                3         €1,100      Rising Star           │   │
│   │   5   Group: "Yoga Tribe"   3         €2,400      Community Leader      │   │
│   │                                                                         │   │
│   │   💡 Consider: Ambassador tier with enhanced benefits (free upgrades)  │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ WORD OF MOUTH TRACKING ────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   "How did you hear about us?" (Post-booking survey)                    │   │
│   │                                                                         │   │
│   │   Friend recommendation     ████████████████████████████  34%           │   │
│   │   Google search             █████████████████████  26%                  │   │
│   │   Instagram                 ██████████████  17%                         │   │
│   │   Booking.com               █████████  11%                              │   │
│   │   Blog/Article              █████  6%                                   │   │
│   │   Other                     ████  5%                                    │   │
│   │                                                                         │   │
│   │   NPS Score: 72 (Excellent)  │  Would Recommend: 94%                   │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

### 2.7 Discount & Promotion Management

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                        DISCOUNT & PROMOTION ENGINE                              │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   ┌─ ACTIVE PROMOTIONS ─────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   CODE            TYPE          VALUE     USAGE    EXPIRES   REVENUE   │   │
│   │   ═══════════════════════════════════════════════════════════════════  │   │
│   │                                                                         │   │
│   │   WINTER25       Seasonal       25%       18/50    Jan 31    €4,200    │   │
│   │   ████████████████████████████████████░░░░░░░░░░░░░░░░░░░░░            │   │
│   │   Status: 🟢 Active, performing above target                           │   │
│   │                                                                         │   │
│   │   LASTMINUTE     Dynamic        15%       8/∞      Ongoing   €1,100    │   │
│   │   Auto-applies to bookings <48hrs before check-in                      │   │
│   │   Status: 🟢 Filling gaps effectively                                  │   │
│   │                                                                         │   │
│   │   LONGSTAY7      Length-based   10%       4/20     Mar 31    €2,800    │   │
│   │   For stays ≥7 nights                                                  │   │
│   │   Status: 🟡 Moderate uptake                                           │   │
│   │                                                                         │   │
│   │   INFLUENCER_X   Partnership    Free      1/1      One-time    €0      │   │
│   │   Status: 🔵 Campaign code                                             │   │
│   │                                                                         │   │
│   │   [ + Create Promotion ]                                                │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ DISCOUNT IMPACT ANALYSIS ──────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   MONTH: December 2024                                                  │   │
│   │                                                                         │   │
│   │   Gross Bookings Value:        €24,500                                  │   │
│   │   Total Discounts Given:       -€1,840  (7.5%)                          │   │
│   │   ─────────────────────────────────────                                 │   │
│   │   Net Revenue:                 €22,660                                  │   │
│   │                                                                         │   │
│   │   DISCOUNT BREAKDOWN:                                                   │   │
│   │   ├── Seasonal promos:         €980   (53%)                            │   │
│   │   ├── Last-minute fills:       €420   (23%)                            │   │
│   │   ├── Referral discounts:      €280   (15%)                            │   │
│   │   └── Loyalty rewards:         €160   (9%)                             │   │
│   │                                                                         │   │
│   │   ⚠️  ANALYSIS:                                                         │   │
│   │   Without discounts: Est. 12 fewer bookings (-€3,600 gross)            │   │
│   │   With discounts: Kept 12 bookings, lost €1,840                        │   │
│   │   NET GAIN from discounting: +€1,760                                   │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ DYNAMIC PRICING RULES ─────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   RULE                           TRIGGER              ADJUSTMENT        │   │
│   │   ═══════════════════════════════════════════════════════════════════  │   │
│   │                                                                         │   │
│   │   🔴 Last-minute fill            <48hrs, unit empty    -15%            │   │
│   │   🟠 Low demand period           Occ <40% next 14d     -10%            │   │
│   │   🟢 High demand surge           Occ >85% next 7d      +20%            │   │
│   │   🔵 Extended stay bonus         Stay ≥5 nights        -8%             │   │
│   │   🟣 Repeat guest loyalty        2nd+ booking          -5%             │   │
│   │   ⚪ Early bird                  >60 days advance      -10%            │   │
│   │                                                                         │   │
│   │   [ Edit Rules ]  [ View Impact Simulation ]                           │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

## PART 3: CUSTOMER LIFETIME VALUE (LTV) & LOYALTY

### 3.1 LTV Calculation Engine

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                        CUSTOMER LIFETIME VALUE ENGINE                           │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   ┌─ LTV FORMULA ───────────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │                     Avg. Booking    Bookings     Gross        Customer  │   │
│   │         LTV    =      Value      ×  per Year  ×  Margin   ×   Lifespan  │   │
│   │                                                                         │   │
│   │                        €320      ×    0.8     ×   65%     ×    3.2 yrs  │   │
│   │                                                                         │   │
│   │                   ═══════════════════════════════════════════════       │   │
│   │                                  LTV = €534                             │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ KEY LTV METRICS ───────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   METRIC                    VALUE        BENCHMARK      STATUS          │   │
│   │   ══════════════════════════════════════════════════════════════════   │   │
│   │                                                                         │   │
│   │   Average LTV               €534         €400-600       🟢 Good        │   │
│   │   Average CAC               €145         €100-200       🟢 Good        │   │
│   │   LTV:CAC Ratio             3.7:1        >3:1           🟢 Healthy     │   │
│   │                                                                         │   │
│   │   Repeat Booking Rate       22%          15-25%         🟢 Good        │   │
│   │   Avg. Time to Return       8.4 months   6-12 months    🟢 Normal      │   │
│   │   Churn Rate (annual)       31%          25-35%         🟡 Average     │   │
│   │                                                                         │   │
│   │   ─────────────────────────────────────────────────────────────────    │   │
│   │   💡 Insight: LTV:CAC of 3.7 means every €1 spent on acquisition       │   │
│   │      returns €3.70 over the customer lifetime. Sustainable!            │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ LTV BY SEGMENT ────────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   SEGMENT              LTV      CAC     RATIO    % OF BASE   PRIORITY  │   │
│   │   ══════════════════════════════════════════════════════════════════   │   │
│   │                                                                         │   │
│   │   VIP Repeaters       €1,890    €85    22.2x       8%        ⭐⭐⭐     │   │
│   │   (4+ stays)                                                           │   │
│   │                                                                         │   │
│   │   Loyal Returners      €720    €120     6.0x      14%        ⭐⭐⭐     │   │
│   │   (2-3 stays)                                                          │   │
│   │                                                                         │   │
│   │   Direct Bookers       €480    €45     10.7x      18%        ⭐⭐       │   │
│   │   (no OTA, 1 stay)                                                     │   │
│   │                                                                         │   │
│   │   Referral Guests      €520    €50     10.4x      15%        ⭐⭐       │   │
│   │                                                                         │   │
│   │   OTA First-timers     €310    €185     1.7x      45%        ⭐         │   │
│   │   (Booking.com/Airbnb)                                                 │   │
│   │                                                                         │   │
│   │   ⚠️  45% of guests are OTA first-timers with lowest LTV:CAC          │   │
│   │   💡 Strategy: Convert OTA guests to direct bookers (save commission)  │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

### 3.2 Loyalty Program Design

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                            LOYALTY PROGRAM TIERS                                │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│                                                                                 │
│        EXPLORER              ADVENTURER            PIONEER             LEGEND   │
│        (1 stay)              (2-3 stays)           (4-6 stays)        (7+ stays)│
│                                                                                 │
│        ┌──────┐              ┌──────┐              ┌──────┐           ┌──────┐  │
│        │  🌱  │      ──▶     │  🌿  │      ──▶     │  🌲  │    ──▶    │  🏔️  │  │
│        └──────┘              └──────┘              └──────┘           └──────┘  │
│                                                                                 │
│        Benefits:             Benefits:             Benefits:          Benefits: │
│        • Welcome             • 5% off              • 10% off          • 15% off │
│          email                 direct               direct             direct   │
│        • Referral            • Early               • Free             • Free    │
│          code                  check-in             upgrade            upgrade  │
│                               (when avail)          (guaranteed)       (always) │
│                              • Birthday            • Hot tub          • VIP     │
│                                surprise              included           hotline │
│                                                    • Priority         • Free    │
│                                                      booking           night/yr │
│                                                                                 │
│        42% of               35% of                15% of              8% of     │
│        guests               guests                guests              guests    │
│                                                                                 │
│   ═══════════════════════════════════════════════════════════════════════════  │
│                                                                                 │
│   PROGRAM ECONOMICS:                                                            │
│   ├── Cost of rewards:        ~€4,200/year                                     │
│   ├── Incremental revenue:    ~€18,400/year (from increased repeat rate)       │
│   └── NET ROI:                4.4x                                             │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

### 3.3 Guest Journey & Touchpoints

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                         GUEST LIFECYCLE AUTOMATION                              │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   STAGE           TOUCHPOINT              CHANNEL        GOAL                   │
│   ═══════════════════════════════════════════════════════════════════════════  │
│                                                                                 │
│   🔍 AWARENESS                                                                  │
│   │                                                                             │
│   │   ├── Social content              Instagram       Build desire             │
│   │   ├── Google Ads                  Search          Capture intent           │
│   │   └── Blog/SEO                    Organic         Educate                  │
│   │                                                                             │
│   ▼                                                                             │
│   📋 CONSIDERATION                                                              │
│   │                                                                             │
│   │   ├── Retargeting ads             Meta/Google     Stay top-of-mind         │
│   │   ├── Email: "Still thinking?"    Email           Nudge decision           │
│   │   └── Virtual tour                Website         Reduce uncertainty       │
│   │                                                                             │
│   ▼                                                                             │
│   💳 BOOKING                                                                    │
│   │                                                                             │
│   │   ├── Confirmation email          Email           Set expectations         │
│   │   ├── "Preparing for you"         Email (D-7)     Build excitement         │
│   │   └── Check-in instructions       Email (D-1)     Reduce friction          │
│   │                                                                             │
│   ▼                                                                             │
│   🏕️ STAY                                                                       │
│   │                                                                             │
│   │   ├── Welcome message             SMS/WhatsApp    Personal touch           │
│   │   ├── Mid-stay check              SMS (if 3+ d)   Address issues           │
│   │   └── Photo opportunity           On-site         Generate UGC             │
│   │                                                                             │
│   ▼                                                                             │
│   📝 POST-STAY                                                                  │
│   │                                                                             │
│   │   ├── Thank you + review ask      Email (D+1)     Get reviews              │
│   │   ├── Photo share request         Email (D+3)     Get UGC                  │
│   │   └── Referral code               Email (D+7)     Activate WOM             │
│   │                                                                             │
│   ▼                                                                             │
│   🔄 RETENTION                                                                  │
│   │                                                                             │
│   │   ├── Season announcement         Email (90d)     Re-engage               │
│   │   ├── "We miss you" offer         Email (180d)    Win back                │
│   │   ├── Birthday/Anniversary        Email           Delight                 │
│   │   └── Loyalty status update       Email           Recognize               │
│   │                                                                             │
│   └────────────────────────────────────────────────────────────────────────────│
│                                                                                 │
│   AUTOMATION STATUS:  ⬜ Not built  🔄 In progress  ✅ Active                   │
│                                                                                 │
│   ⬜ Awareness       ⬜ Consideration    ✅ Booking                             │
│   ⬜ Stay            ⬜ Post-Stay        ⬜ Retention                           │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

## PART 4: ENHANCED BUSINESS MONITORING

### 4.1 Marketing Performance Dashboard

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                     MARKETING PERFORMANCE COMMAND CENTER                        │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   ┌─ ACQUISITION FUNNEL ────────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   IMPRESSIONS     CLICKS       LEADS        BOOKINGS      GUESTS       │   │
│   │     124,500        8,420        1,890          62           148         │   │
│   │        │            │            │             │             │          │   │
│   │        └────6.8%────┘────22.4%───┘────3.3%────┘────2.4pax───┘          │   │
│   │                                                                         │   │
│   │   ████████████████████████████████████████████████░░░░░░░░░░░░░░░░░░   │   │
│   │                                                                         │   │
│   │   Funnel Health: 🟢 Good  │  vs Last Month: ▲ +8% bookings             │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ CHANNEL MIX (Revenue Attribution) ─────────────────────────────────────┐   │
│   │                                                                         │   │
│   │        OTA          PAID         DIRECT       REFERRAL      ORGANIC    │   │
│   │       32%           28%           18%           12%           10%       │   │
│   │                                                                         │   │
│   │   ░░░░░░░░░░░░  ████████████  ████████░░░░  ██████░░░░░░  █████░░░░░   │   │
│   │   HIGH COST     SCALABLE      BEST MARGIN   CHEAPEST      FREE         │   │
│   │                                                                         │   │
│   │   Target Mix:   25%           30%           25%           15%    5%    │   │
│   │   Gap:          -7%           +2%           +7%           +3%    -5%   │   │
│   │                                                                         │   │
│   │   💡 Action: Increase direct booking incentives to shift from OTA      │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
│   ┌─ MARKETING ROI SUMMARY ─────────────────────────────────────────────────┐   │
│   │                                                                         │   │
│   │   Total Marketing Spend:       €2,180                                   │   │
│   │   Attributed Revenue:          €18,400                                  │   │
│   │   ─────────────────────────────────────                                 │   │
│   │   Blended ROAS:                8.4x                                     │   │
│   │   Cost per Booking:            €35                                      │   │
│   │   Cost per Guest Night:        €12                                      │   │
│   │                                                                         │   │
│   │   vs Target:                   ROAS 8.4x > 5.0x target  🟢             │   │
│   │                                                                         │   │
│   └─────────────────────────────────────────────────────────────────────────┘   │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

### 4.2 Customer Health Sankey (NEW)

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                        CUSTOMER HEALTH FLOW (Sankey)                            │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   NEW GUESTS                                                                    │
│   This Year: 180                                                                │
│        │                                                                        │
│        │                                                                        │
│        ├─────────────────────────────────────────────────▶ ONE-TIME            │
│        │ ████████████████████████████████████████████████   140 (78%)          │
│        │                                                                        │
│        │                                                                        │
│        └───────────────────────▶ RETURNED                                       │
│                                  40 (22%)                                       │
│                                    │                                            │
│                                    │                                            │
│                                    ├─────────────────────▶ 2ND STAY ONLY       │
│                                    │ █████████████████████  28 (70%)           │
│                                    │                                            │
│                                    │                                            │
│                                    └─────────────▶ BECAME LOYAL                 │
│                                                    12 (30%)                     │
│                                                      │                          │
│                                                      │                          │
│                                                      ├────────▶ 3-4 STAYS       │
│                                                      │ ████████  8 (67%)        │
│                                                      │                          │
│                                                      └────▶ 5+ STAYS (VIP)      │
│                                                        ████  4 (33%)            │
│                                                                                 │
│   ═══════════════════════════════════════════════════════════════════════════  │
│                                                                                 │
│   INSIGHT: 78% never return. Focus on post-stay engagement to improve.         │
│   TARGET: Reduce one-time to 65%, increase returned to 35%                     │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

## PART 5: DATA MODEL ADDITIONS

### 5.1 Marketing & LTV TypeScript Models

```typescript
// ═══════════════════════════════════════════════════════════════
// MARKETING & LTV DATA MODELS
// ═══════════════════════════════════════════════════════════════

// Guest & LTV
interface Guest {
  id: string;
  email: string;
  phone?: string;
  firstName: string;
  lastName: string;

  // Acquisition
  firstBookingDate: Date;
  acquisitionChannel: Channel;
  acquisitionCampaign?: string;
  referredBy?: string;

  // Loyalty
  loyaltyTier: 'explorer' | 'adventurer' | 'pioneer' | 'legend';
  totalStays: number;
  totalRevenue: number;
  totalNights: number;

  // LTV Calculation
  ltv: number;
  predictedNextBooking?: Date;
  churnRisk: 'low' | 'medium' | 'high';

  // Engagement
  lastStayDate: Date;
  avgReviewScore?: number;
  referralsMade: number;
  referralCode: string;

  // Communication
  emailOptIn: boolean;
  smsOptIn: boolean;
  preferredLanguage: string;
}

interface LTVMetrics {
  period: DateRange;

  // Cohort analysis
  newGuests: number;
  returningGuests: number;
  repeatRate: number;

  // Value metrics
  avgBookingValue: number;
  avgBookingsPerYear: number;
  avgGrossMargin: number;
  avgLifespanYears: number;
  calculatedLTV: number;

  // Acquisition efficiency
  totalCAC: number;
  avgCAC: number;
  ltvCacRatio: number;

  // Churn
  churnedGuests: number;
  churnRate: number;
  avgTimeToChurn: number;
}

// Referral Program
interface ReferralProgram {
  referrerReward: {
    type: 'credit' | 'discount' | 'free_night';
    value: number;
    trigger: 'on_booking' | 'on_completion';
  };

  refereeReward: {
    type: 'discount' | 'upgrade' | 'amenity';
    value: number;
  };

  metrics: {
    totalCodesSent: number;
    totalCodesUsed: number;
    conversionRate: number;
    totalRevenueGenerated: number;
    totalRewardsCost: number;
    netContribution: number;
    costPerReferralBooking: number;
  };
}

// Discount Management
interface Promotion {
  id: string;
  code: string;
  name: string;

  // Type
  type: 'percentage' | 'fixed' | 'free_night' | 'upgrade';
  value: number;

  // Conditions
  conditions: {
    minNights?: number;
    minValue?: number;
    validUnits?: string[];
    validDates?: DateRange;
    maxUses?: number;
    maxUsesPerGuest?: number;
    newGuestsOnly?: boolean;
    channels?: Channel[];
  };

  // Tracking
  status: 'active' | 'paused' | 'expired';
  usageCount: number;
  revenueGenerated: number;
  discountGiven: number;

  // Attribution
  campaign?: string;
  influencer?: string;
}

interface DynamicPricingRule {
  id: string;
  name: string;
  priority: number;

  trigger: {
    type: 'occupancy' | 'lead_time' | 'stay_length' | 'day_of_week' | 'season';
    operator: '>' | '<' | '=' | 'between';
    value: number | [number, number];
  };

  adjustment: {
    type: 'percentage' | 'fixed';
    value: number; // positive = increase, negative = decrease
  };

  active: boolean;
  appliedCount: number;
  revenueImpact: number;
}

// Marketing Channels
interface MarketingChannel {
  channel: Channel;

  // Budget
  monthlyBudget: number;
  spentThisMonth: number;

  // Performance
  impressions: number;
  clicks: number;
  bookings: number;
  revenue: number;

  // Calculated
  ctr: number;           // Click-through rate
  conversionRate: number;
  cpc: number;           // Cost per click
  cpa: number;           // Cost per acquisition
  roas: number;          // Return on ad spend

  // Quality
  avgStayLength: number;
  avgReviewScore: number;
  repeatRate: number;
}

interface Campaign {
  id: string;
  name: string;
  channel: Channel;
  platform: 'google' | 'meta' | 'tiktok' | 'pinterest' | 'email';

  // Dates
  startDate: Date;
  endDate?: Date;
  status: 'draft' | 'active' | 'paused' | 'completed';

  // Budget
  budget: number;
  spent: number;

  // Performance
  impressions: number;
  clicks: number;
  bookings: number;
  revenue: number;
  roas: number;

  // Creative
  creativeAssets?: string[];
  targetAudience?: string;

  // UTM
  utmSource: string;
  utmMedium: string;
  utmCampaign: string;
}

// Influencer
interface InfluencerPartnership {
  id: string;

  // Profile
  handle: string;
  platform: 'instagram' | 'tiktok' | 'youtube' | 'blog';
  followers: number;
  engagementRate: number;

  // Deal
  compensation: {
    type: 'free_stay' | 'paid' | 'hybrid';
    stayValue?: number;
    cashPayment?: number;
    totalValue: number;
  };

  // Deliverables
  deliverables: {
    posts: { required: number; delivered: number };
    stories: { required: number; delivered: number };
    reels?: { required: number; delivered: number };
  };

  // Tracking
  uniqueCode: string;
  trackingLink: string;

  // Results
  reach: number;
  engagement: number;
  clicksTracked: number;
  bookingsTracked: number;
  revenueTracked: number;
  calculatedROI: number;

  // Status
  status: 'negotiating' | 'confirmed' | 'in_progress' | 'completed' | 'cancelled';
  visitDates?: DateRange;
}

// Content Performance
interface ContentPost {
  id: string;
  platform: 'instagram' | 'facebook' | 'tiktok' | 'blog';
  type: 'post' | 'reel' | 'story' | 'article' | 'video';

  // Content
  title?: string;
  description?: string;
  mediaUrls: string[];
  publishedAt: Date;

  // Performance
  impressions: number;
  reach: number;
  engagement: number;
  engagementRate: number;
  clicks: number;
  shares: number;
  saves: number;

  // Attribution
  bookingsAttributed: number;
  revenueAttributed: number;

  // Analysis
  effectiveHourlyRate: number; // Revenue / Time invested
}

// Email Automation
interface EmailSequence {
  id: string;
  name: string;
  trigger: 'booking' | 'post_stay' | 'anniversary' | 'win_back' | 'referral';

  emails: Array<{
    id: string;
    subject: string;
    delayDays: number;

    // Performance
    sent: number;
    opened: number;
    clicked: number;
    converted: number;

    openRate: number;
    clickRate: number;
    conversionRate: number;
  }>;

  status: 'active' | 'paused' | 'draft';
  totalRevenue: number;
}
```

---

## PART 6: IMPLEMENTATION PRIORITY

### Recommended Build Order

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                         MARKETING MODULE ROADMAP                                │
├─────────────────────────────────────────────────────────────────────────────────┤
│                                                                                 │
│   PHASE 1: FOUNDATION                                                           │
│   ═══════════════════                                                           │
│   □ Guest database with acquisition tracking                                    │
│   □ Basic LTV calculation                                                       │
│   □ "How did you hear about us?" field on booking                              │
│   □ UTM parameter capture                                                       │
│                                                                                 │
│   PHASE 2: ATTRIBUTION                                                          │
│   ════════════════════                                                          │
│   □ Channel performance dashboard                                               │
│   □ ROAS calculation per channel                                                │
│   □ Booking source breakdown                                                    │
│   □ Cost tracking per platform                                                  │
│                                                                                 │
│   PHASE 3: LOYALTY                                                              │
│   ═══════════════                                                               │
│   □ Loyalty tier system                                                         │
│   □ Referral program with tracking codes                                        │
│   □ Repeat guest recognition                                                    │
│   □ LTV:CAC dashboard                                                           │
│                                                                                 │
│   PHASE 4: PROMOTIONS                                                           │
│   ══════════════════                                                            │
│   □ Discount code management                                                    │
│   □ Dynamic pricing rules                                                       │
│   □ Promotion impact analysis                                                   │
│   □ A/B test framework                                                          │
│                                                                                 │
│   PHASE 5: CONTENT & INFLUENCER                                                 │
│   ════════════════════════════                                                  │
│   □ Content calendar                                                            │
│   □ Post performance tracking                                                   │
│   □ Influencer campaign management                                              │
│   □ UGC collection system                                                       │
│                                                                                 │
│   PHASE 6: AUTOMATION                                                           │
│   ══════════════════                                                            │
│   □ Email sequence builder                                                      │
│   □ Guest lifecycle automation                                                  │
│   □ Win-back campaigns                                                          │
│   □ Review solicitation                                                         │
│                                                                                 │
└─────────────────────────────────────────────────────────────────────────────────┘
```

---

## PART 7: SUMMARY — WHAT CHANGES

| Area | Current State | Proposed State |
|------|---------------|----------------|
| **Architecture** | 3 Layers | 4 Layers (+Growth Engine) |
| **Guest Data** | Booking-centric | Guest-centric with history |
| **Attribution** | None | Full multi-touch |
| **LTV** | Mentioned only | Calculated & tracked |
| **CAC** | Mentioned only | Per-channel tracking |
| **Referrals** | None | Full program with tracking |
| **Discounts** | Sankey shows 3% | Management system |
| **Content** | None | Performance tracking |
| **Influencer** | None | Campaign management |
| **Loyalty** | None | 4-tier program |
| **Automation** | None | Guest lifecycle flows |

---

## APPENDIX: New KPI Additions

Add to existing KPI dashboard:

| KPI | Formula | Target | Category |
|-----|---------|--------|----------|
| **LTV** | Avg Value × Frequency × Margin × Lifespan | >€500 | Customer |
| **LTV:CAC** | LTV / CAC | >3:1 | Efficiency |
| **Repeat Rate** | Returning / Total Guests | >25% | Loyalty |
| **Referral Rate** | Referral Bookings / Total | >15% | WOM |
| **ROAS** | Revenue / Ad Spend | >5x | Marketing |
| **Direct %** | Direct Bookings / Total | >25% | Channel |
| **NPS** | Promoters - Detractors | >50 | Satisfaction |
| **Email Open Rate** | Opens / Sent | >25% | Engagement |
| **Churn Rate** | Churned / Total Base | <30% | Retention |

---

> **Document Version:** 1.0
> **Created:** 2025-12-19
> **Purpose:** Enhancement recommendations for GlampModeler marketing & LTV capabilities
