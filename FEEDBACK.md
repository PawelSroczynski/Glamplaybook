# GlampModeler Ultimate — Constructive Feedback & Enhancement Recommendations

---

## Executive Summary

The current spec is solid for a **one-time investment calculator**. To transform it into a **daily operational tool** that glamping owners actually live in, we need to add:

1. **Real-time operational layer** (bookings, occupancy, revenue tracking)
2. **Actionable KPIs** with drill-down capability
3. **Sankey diagrams** for revenue/cost flow visualization
4. **Benchmark comparisons** (vs. plan, vs. industry, vs. previous period)
5. **Alert system** for underperformance

---

## Gap Analysis: What's Missing

### Currently Strong
- CapEx configuration (excellent detail)
- 10-year projection model
- Asset lifecycle awareness
- Staffing step-function logic

### Currently Weak / Missing

| Gap | Impact | Priority |
|-----|--------|----------|
| No live data integration | Tool becomes "use once, forget" | Critical |
| No daily/weekly KPI tracking | Can't measure actual vs. projected | Critical |
| No booking/channel data | Revenue tracking is theoretical only | High |
| No expense tracking | OpEx is estimated, not actual | High |
| No alerts/notifications | User must manually check everything | Medium |
| No mobile view for quick checks | Operators are on-site, not at desks | Medium |

---

## Recommended Architecture: Three-Layer System

```
┌─────────────────────────────────────────────────────────────────┐
│                     LAYER 1: PLANNING MODE                       │
│            (Current spec - Investment & Projection)              │
│                                                                   │
│   Unit Configurator → Site Setup → 10-Year Model → PDF Export   │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│                    LAYER 2: OPERATIONS MODE                      │
│              (NEW - Daily Business Performance)                  │
│                                                                   │
│   Live Dashboard → Booking Tracker → Expense Log → KPI Alerts   │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│                    LAYER 3: ANALYSIS MODE                        │
│              (NEW - Insights & Optimization)                     │
│                                                                   │
│   Actual vs. Plan → Sankey Flows → Benchmarks → What-If Sims    │
└─────────────────────────────────────────────────────────────────┘
```

---

## Detailed Recommendations

---

### 1. KPI Dashboard (Operations Mode)

#### Top-Level KPIs (Always Visible)

| KPI | Formula | Update Frequency | Visualization |
|-----|---------|------------------|---------------|
| **Occupancy Rate** | `Nights Booked / Available Nights × 100` | Daily | Gauge (0-100%) |
| **RevPAR** | `Total Revenue / Available Room Nights` | Daily | Number + Trend |
| **ADR** | `Room Revenue / Rooms Sold` | Daily | Number + Trend |
| **GOP** | `Gross Operating Profit` | Monthly | Number + Trend |
| **EBITDA Margin** | `EBITDA / Revenue × 100` | Monthly | Gauge |
| **Cash Runway** | `Cash Balance / Monthly Burn` | Weekly | Number (months) |

#### Second-Tier KPIs (Expandable Cards)

**Revenue Health:**
- Revenue per Unit per Month
- Ancillary Revenue % of Total
- Direct vs. OTA Booking Ratio
- Average Length of Stay (ALOS)
- Booking Lead Time (days ahead)

**Cost Control:**
- Energy Cost per Occupied Night
- Labor Cost % of Revenue
- Maintenance Cost vs. Budget
- Cost per Available Room (CPAR)

**Guest Metrics:**
- Repeat Guest Rate
- Average Review Score
- Cancellation Rate
- No-Show Rate

---

### 2. Sankey Diagram Applications

Sankey diagrams are perfect for showing **flow and leakage**. Here's where to use them:

#### A. Revenue Flow Sankey

```
┌──────────────┐
│ GROSS BOOKING│ ────┬────→ Net Room Revenue (75%)
│   €100,000   │     │
└──────────────┘     ├────→ OTA Commissions (15%)
                     │
                     ├────→ Cancellations (7%)
                     │
                     └────→ Discounts/Promos (3%)
```

**Purpose:** Show where gross revenue "leaks" before becoming net revenue.

#### B. Operating Cost Flow Sankey

```
┌──────────────┐
│ NET REVENUE  │ ────┬────→ Staff Costs (25%)
│   €75,000    │     │
└──────────────┘     ├────→ Energy (15%)
                     │
                     ├────→ Maintenance (8%)
                     │
                     ├────→ Marketing (10%)
                     │
                     ├────→ Insurance (5%)
                     │
                     ├────→ Loan Repayment (12%)
                     │
                     └────→ NET PROFIT (25%)
```

**Purpose:** Visualize where every euro goes after earning it.

#### C. Booking Funnel Sankey

```
┌──────────────┐
│   WEBSITE    │ ────┬────→ Booking Started (40%)
│   VISITORS   │     │           │
│    10,000    │     │           ├──→ Completed (60%) ──→ Arrived (92%)
└──────────────┘     │           │
                     │           └──→ Abandoned (40%)
                     │
                     └────→ Bounced (60%)
```

**Purpose:** Identify conversion bottlenecks.

#### D. Seasonal Revenue Distribution

```
        ┌─────────────────────────────────────────┐
Q1 ─────┤██░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░│ 8%
Q2 ─────┤██████████████░░░░░░░░░░░░░░░░░░░░░░░░░░│ 28%
Q3 ─────┤██████████████████████████████░░░░░░░░░░│ 48%
Q4 ─────┤████████░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░│ 16%
        └─────────────────────────────────────────┘
```

---

### 3. Actual vs. Plan Tracking

This is the **killer feature** that makes it a daily tool.

#### Monthly Comparison View

| Metric | Plan | Actual | Variance | Status |
|--------|------|--------|----------|--------|
| Occupancy | 65% | 58% | -7pp | 🔴 |
| ADR | €120 | €135 | +€15 | 🟢 |
| RevPAR | €78 | €78.30 | +€0.30 | 🟡 |
| Energy Cost | €2,400 | €3,100 | +€700 | 🔴 |
| Staff Cost | €4,000 | €3,800 | -€200 | 🟢 |

#### Trend Visualization

```
         Plan (dashed) vs Actual (solid)
Revenue
€50k │                          ╭───●
     │                    ╭────╯
€40k │              ╭────╯   - - ●- -
     │        ╭────╯    - - -
€30k │  ╭────╯   - - - -
     │ ╯  - - - -
€20k │- - -
     └────┬────┬────┬────┬────┬────┬────→
         Jan  Feb  Mar  Apr  May  Jun
```

---

### 4. Alert & Notification System

#### Configurable Thresholds

| Alert Type | Condition | Action |
|------------|-----------|--------|
| **Occupancy Warning** | < 40% for next 14 days | Push notification |
| **Revenue Drop** | MTD revenue < 80% of plan | Email alert |
| **Cost Spike** | Any category > 120% of budget | Dashboard badge |
| **Cash Flow Alert** | Runway < 3 months | Critical banner |
| **Maintenance Due** | Scheduled event within 30 days | Task reminder |
| **Review Score Drop** | Average < 4.2 stars | Action required |

---

### 5. Data Input Methods

For the tool to track actuals, data must come from somewhere:

#### Option A: Manual Entry (MVP)

| Data Type | Entry Method | Frequency |
|-----------|--------------|-----------|
| Bookings | Form input or CSV upload | Per booking |
| Revenue | Bank statement upload | Weekly |
| Expenses | Categorized expense form | As incurred |
| Occupancy | Calendar marking | Daily |

#### Option B: Integrations (V2)

| Source | Data Pulled | Sync |
|--------|-------------|------|
| Booking.com API | Reservations, Revenue | Real-time |
| Airbnb API | Reservations, Reviews | Real-time |
| Bank Open API | Transactions | Daily |
| Smart Meter | Energy consumption | Hourly |
| Weather API | Temperature data | Daily |

---

### 6. Missing Financial Metrics

Add these to the 10-year model:

| Metric | Formula | Why It Matters |
|--------|---------|----------------|
| **DSCR** | `NOI / Debt Service` | Bank loan requirement (must be > 1.2) |
| **Cash-on-Cash Return** | `Annual Cash Flow / Total Cash Invested` | True investor return |
| **Cap Rate** | `NOI / Property Value` | Asset valuation metric |
| **Break-Even Occupancy** | `Fixed Costs / (ADR - Variable Cost per Night)` | Survival threshold |
| **LTV** | `Customer Lifetime Value` | For repeat guests |
| **CAC** | `Marketing Spend / New Customers` | Acquisition efficiency |

---

### 7. UI Improvements for Daily Use

#### Quick Actions Bar

```
┌────────────────────────────────────────────────────────────────┐
│  [+ New Booking]  [+ Log Expense]  [Update Rates]  [Run Report]│
└────────────────────────────────────────────────────────────────┘
```

#### Unit Status Grid (At-a-Glance)

```
┌─────────┬─────────┬─────────┬─────────┐
│ Unit 1  │ Unit 2  │ Unit 3  │ Unit 4  │
│ 🟢 OCC  │ 🔵 CLEAN│ 🟢 OCC  │ ⚪ AVAIL│
│ →Dec 22 │ Ready   │ →Dec 20 │ Book me │
│ €150/n  │         │ €120/n  │ €140/n  │
└─────────┴─────────┴─────────┴─────────┘
```

#### Mobile Dashboard (Simplified)

```
┌─────────────────────────────┐
│  Today: 3/4 units occupied  │
│  ████████████████░░░░ 75%   │
├─────────────────────────────┤
│  This Week Revenue          │
│  €2,340 ↑12% vs last week   │
├─────────────────────────────┤
│  ⚠️ 2 Alerts                │
│  • Unit 2 checkout today    │
│  • Energy cost +23% MTD     │
└─────────────────────────────┘
```

---

### 8. Recommended Chart Library Additions

Current spec uses Recharts. Add:

| Library | Use Case |
|---------|----------|
| **react-sankey** or **d3-sankey** | Revenue/cost flow diagrams |
| **react-calendar-heatmap** | Occupancy calendar view |
| **@nivo/bullet** | Target vs. actual gauge charts |
| **react-gauge-chart** | Occupancy/performance meters |

---

### 9. Benchmark Data

Consider adding industry benchmarks:

| Metric | Budget | Midscale | Luxury Glamping |
|--------|--------|----------|-----------------|
| ADR | €80-120 | €120-180 | €200-350 |
| Occupancy | 45-55% | 55-70% | 60-75% |
| RevPAR | €40-65 | €75-120 | €130-250 |
| GOP Margin | 25-35% | 35-45% | 45-55% |
| Energy % | 12-18% | 8-12% | 6-10% |

---

### 10. Export & Reporting Enhancements

| Report | Audience | Frequency |
|--------|----------|-----------|
| **Investor Summary** | Investors/Banks | Quarterly |
| **Owner Dashboard** | Operator | Daily/Weekly |
| **Tax Report** | Accountant | Annual |
| **Maintenance Log** | Operations | As needed |
| **Guest Analytics** | Marketing | Monthly |

---

## Implementation Priority

### Phase 1: Foundation (MVP)
1. Add Actual vs. Plan tracking to existing projections
2. Build simple booking/expense input forms
3. Add 6 core KPI cards to dashboard
4. Implement basic alerts

### Phase 2: Visualization
1. Add Revenue Flow Sankey
2. Add Cost Breakdown Sankey
3. Implement gauge charts for targets
4. Build occupancy calendar heatmap

### Phase 3: Intelligence
1. Add benchmark comparisons
2. Build "What-If" scenario tool
3. Implement predictive occupancy
4. Add weather correlation analysis

### Phase 4: Integration
1. Channel manager API connections
2. Bank feed integration
3. Smart meter data
4. Automated reporting

---

## Summary: The Transformation

| Aspect | Current Spec | Enhanced Spec |
|--------|--------------|---------------|
| **Purpose** | Investment calculator | Business command center |
| **Usage** | Once (before building) | Daily (ongoing operations) |
| **Data** | Projections only | Projections + Actuals |
| **Insight** | "This is what could happen" | "This is what IS happening vs. what we planned" |
| **Action** | Static report | Dynamic alerts + recommendations |

---

*Feedback Version: 1.0*
*Date: 2025-12-19*
