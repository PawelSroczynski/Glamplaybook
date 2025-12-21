# Enklava Yurts: SOP Infrastructure

**Version:** 2.0
**Optimized:** December 2025

## Complete Client Flow Coverage

```
┌────────────────────────────────────────────────────────────────────────────────────────────┐
│                           ENKLAVA YURTS - COMPLETE SOP SUITE v2.0                          │
├────────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                            │
│  ┌─────────────────────────────────────────────────────────────────────────────────────┐   │
│  │  CORE (Cross-Cutting)                                                               │   │
│  │  Communication │ Exceptions │ Safety │ Documentation                                │   │
│  │  ─────────────────────────────────────────────────────────────────────────────────  │   │
│  │  Applies to ALL phases below                                              4 SOPs    │   │
│  └─────────────────────────────────────────────────────────────────────────────────────┘   │
│                                                                                            │
│  ┌─────────┐   ┌─────────┐   ┌─────────┐   ┌─────────┐   ┌─────────┐   ┌─────────┐        │
│  │  SALES  │ → │  PREP   │ → │  PROD   │ → │   LOG   │ → │  ASSY   │ → │  CARE   │        │
│  │ Part 1  │   │ Part 2  │   │ Part 3  │   │ Part 4  │   │ Part 5  │   │ Part 6  │        │
│  └─────────┘   └─────────┘   └─────────┘   └─────────┘   └─────────┘   └─────────┘        │
│                                                                                            │
│   8 SOPs        6 SOPs       14 SOPs        3 SOPs       11 SOPs        7 SOPs            │
│                                                                                            │
├────────────────────────────────────────────────────────────────────────────────────────────┤
│                    TOTAL: 4 CORE + 49 Operational = 53 SOPs + 20 Quality Gates            │
└────────────────────────────────────────────────────────────────────────────────────────────┘
```

### CCF Mapping

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│  CRITICAL CLIENT FLOW (Jurta v3.0)           →    SOP COVERAGE                          │
├─────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                         │
│  ╔═══════════════════════════════════════════════════════════════════════════════════╗  │
│  ║  CORE: Cross-Cutting SOPs (Apply Throughout)                                      ║  │
│  ║  CORE-001 Communication │ CORE-002 Exceptions │ CORE-003 Safety │ CORE-004 Docs   ║  │
│  ╚═══════════════════════════════════════════════════════════════════════════════════╝  │
│                                                                                         │
│  Attention ─┐                                                                           │
│  Engagement ├─→ PART 1: SALES      (Lead → Customer)                                    │
│  Enquiry    │                                                                           │
│  Sales      │                                                                           │
│  Money      │                                                                           │
│  Orders ────┘                                                                           │
│       │                                                                                 │
│       ▼                                                                                 │
│  ─────────────────────────────────────────────────────────────────────────────────────  │
│       │                                                                                 │
│       ├─→ PART 2: PREP         (Order → Production Ready)                               │
│       │                                                                                 │
│  Production ─→ PART 3: PROD    (Raw Materials → Components)                             │
│       │        ├─ Wood Stream      (6 SOPs)                                             │
│       │        ├─ Sewing Stream    (4 SOPs)                                             │
│       │        ├─ Insulation Stream (2 SOPs)                                            │
│       │        └─ External/Hardware (2 SOPs)                                            │
│       │                                                                                 │
│  Delivery ───→ PART 4: LOG     (Workshop → Site)                                        │
│       │                                                                                 │
│  Assembly ───→ PART 5: ASSY    (Components → Standing Yurt)                             │
│       │                                                                                 │
│  ─────────────────────────────────────────────────────────────────────────────────────  │
│       │                                                                                 │
│  Repeat ─────→ PART 6: CARE    (Satisfied Customer → Ambassador)                        │
│                                                                                         │
└─────────────────────────────────────────────────────────────────────────────────────────┘

LEGEND:
═══════════════════════════════════════════════════════════════
  CORE           = Cross-cutting (safety, comms, exceptions, docs)
  PART 1 + 6     = Customer Relationship (before & after)
  PART 2-5       = Physical Operations (current focus) ◀◀◀
═══════════════════════════════════════════════════════════════
```

---

## Part 0: CORE (Cross-Cutting SOPs)

*These SOPs apply across ALL phases and must be referenced by operational SOPs*

| SOP ID | Name | Purpose | Applies To |
|--------|------|---------|------------|
| **CORE-001** | Customer Communication Protocol | Standard touchpoints, updates, response times | SALES → CARE |
| **CORE-002** | Issue & Exception Handling | What to do when things go wrong, escalation paths | ALL |
| **CORE-003** | Safety & PPE Standards | Required safety equipment, briefings, incident reporting | PROD, LOG, ASSY |
| **CORE-004** | Documentation & Photo Capture | Evidence standards for QC, portfolio, disputes | ALL |

### Exception Handling Matrix (CORE-002)

| Phase | Exception Type | Immediate Action | Escalation |
|-------|---------------|------------------|------------|
| PREP | Materials fail QC | Reject, reorder, notify customer | Founder if >3 day delay |
| PROD | Component fails inspection | Rework or remake, log defect | QA Lead |
| LOG | Damage during transport | Photo document, assess severity | Founder |
| ASSY | Weather delay | Reschedule, notify customer | Site Lead |
| ASSY | Customer rejects handover | Document issues, create punch list | Founder |

---

## Part 1: SALES (Lead to Order)

*From first contact to signed agreement and payment*

### Acquisition (SALES-001 to SALES-003)

| SOP ID | Name | Purpose | CCF Stage |
|--------|------|---------|-----------|
| **SALES-001** | Lead Capture & Response | Respond to inquiries from all channels within 24h | Attention → Engagement |
| **SALES-002** | Lead Qualification & Scoring | Assess budget, timeline, site viability | Engagement |
| **SALES-003** | Onboarding Multimedia Delivery | Send intro videos, photos, testimonials | Engagement → Enquiry |

### Conversion (SALES-004 to SALES-006)

| SOP ID | Name | Purpose | CCF Stage |
|--------|------|---------|-----------|
| **SALES-004** | Needs Assessment & Site Discovery | Define requirements, site conditions, constraints | Enquiry |
| **SALES-005** | Proposal Creation | Build customized proposal with specs and pricing | Sales |
| **SALES-006** | Agreement & Closing | Present proposal, handle objections, close deal | Sales |

### Transaction (SALES-007 to SALES-008)

| SOP ID | Name | Purpose | CCF Stage |
|--------|------|---------|-----------|
| **SALES-007** | Contract & Documentation | Generate agreement, collect signatures | Money |
| **SALES-008** | Invoicing & Payment Collection | Issue invoice, track payment, confirm receipt | Money → Orders |

### SALES Quality Gates

| Gate | Checkpoint | Pass Criteria | Pass Action | Fail Action |
|------|------------|---------------|-------------|-------------|
| QG-SALES-1 | Lead Qualified | Budget ≥ min, timeline realistic, site viable | → SALES-003 | Archive lead or nurture sequence |
| QG-SALES-2 | Proposal Accepted | Customer confirms specs in writing | → SALES-006 | ↺ Revise proposal (SALES-005) or close lost |
| QG-SALES-3 | Payment Received | Deposit/full payment cleared | → PREP-001 | Hold until cleared, send reminder |

---

## Part 2: PREP (Production Preparation)

*Before any production starts - planning, ordering, workspace setup*

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **PREP-001** | Order Intake & Specification | Convert signed agreement into production specs | Payment cleared (QG-SALES-3) |
| **PREP-002** | Materials Calculation | Calculate exact materials needed per order | Specs confirmed |
| **PREP-003** | Supplier Ordering | Order external components (windows, doors, skylight, connectors, canvases) | Materials calculated |
| **PREP-004** | Materials Receiving & QC | Inspect incoming materials, reject defects | Delivery arrives |
| **PREP-005** | Production Planning & Scheduling | Schedule the 3 parallel production streams | All materials ready |
| **PREP-006** | Workshop & Tool Setup | Prepare workspace, verify tool readiness, calibrate equipment | Before production start |

### PREP Quality Gates

| Gate | Checkpoint | Pass Criteria | Pass Action | Fail Action |
|------|------------|---------------|-------------|-------------|
| QG-PREP-1 | Spec Confirmation | Customer sign-off on final specs | → PREP-002 | ↺ Clarify with customer (PREP-001) |
| QG-PREP-2 | Materials Ready | All materials received and QC passed | → PREP-005 | ↺ Reject & reorder (PREP-003) via CORE-002 |
| QG-PREP-3 | Production Ready | All 3 streams scheduled, workshop ready | → PROD-001/006/010 | ↺ Resolve blockers (PREP-005/006) |

---

## Part 3: PRODUCTION

*Three parallel streams + external orders*

### Stream A: Wooden Structure (PROD-001 to PROD-005)

| SOP ID | Name | Purpose | Output | QG After |
|--------|------|---------|--------|----------|
| **PROD-001** | Wood Selection & Cutting | Select and cut battens to spec dimensions | Cut pieces | QG-PROD-A1 |
| **PROD-002** | Wood Treatment & Finishing | Apply preservative, sand, finish | Treated pieces | - |
| **PROD-003** | Khana (Wall Lattice) Assembly | Drill, connect lattice sections | Lattice panels | QG-PROD-A2 |
| **PROD-004** | Uni (Roof Poles) Preparation | Shape and finish roof poles | Roof poles set | - |
| **PROD-005** | Tono (Crown Ring) Construction | Build the crown/skylight ring | Crown ring | QG-PROD-A3 |

### Stream B: Sewing Covers (PROD-006 to PROD-009)

| SOP ID | Name | Purpose | Output | QG After |
|--------|------|---------|--------|----------|
| **PROD-006** | Canvas Measurement & Cutting | Cut canvas to pattern | Cut canvas pieces | QG-PROD-B1 |
| **PROD-007** | Wall Cover Sewing | Sew outer wall covering | Wall cover | QG-PROD-B2 |
| **PROD-008** | Roof Cover Sewing | Sew roof cone covering | Roof cover | - |
| **PROD-009** | Inner Liner Sewing | Sew interior decorative liner | Inner liner | QG-PROD-B3 |

### Stream C: Insulation Shaping (PROD-010 to PROD-011)

| SOP ID | Name | Purpose | Output | QG After |
|--------|------|---------|--------|----------|
| **PROD-010** | Insulation Cutting | Cut insulation to pattern | Insulation pieces | - |
| **PROD-011** | Insulation Assembly | Layer and connect insulation | Insulation set | QG-PROD-C1 |

### External & Hardware (PROD-012 to PROD-014)

| SOP ID | Name | Purpose | Output | QG After |
|--------|------|---------|--------|----------|
| **PROD-012** | Door & Window Preparation | Prep ordered doors/windows for install | Fitted openings | - |
| **PROD-013** | Rope & Tensioning Elements | Prepare all ropes, tension bands, tie-downs | Rope kit | - |
| **PROD-014** | Hardware & Connectors Prep | Organize all metal connectors, stakes, tools | Hardware kit | - |

### PRODUCTION Quality Gates

#### In-Process Gates (Per Stream)

| Gate | After | Check | Pass Criteria | Pass Action | Fail Action |
|------|-------|-------|---------------|-------------|-------------|
| QG-PROD-A1 | PROD-001 | Cutting Accuracy | All pieces within ±2mm tolerance | → PROD-002 | ↺ Recut (PROD-001) |
| QG-PROD-A2 | PROD-003 | Khana Structure | Lattice expands/contracts smoothly, no cracks | → PROD-004 | ↺ Repair or remake (PROD-003) |
| QG-PROD-A3 | PROD-005 | Crown Ring | Ring is true circle, all joints solid | → Merge | ↺ Rebuild (PROD-005) |
| QG-PROD-B1 | PROD-006 | Canvas Cutting | All pieces match pattern, no waste errors | → PROD-007 | ↺ Recut (PROD-006) |
| QG-PROD-B2 | PROD-007 | Wall Cover Seams | Seams pass pull test, waterproof | → PROD-008 | ↺ Resew seams (PROD-007) |
| QG-PROD-B3 | PROD-009 | All Covers Complete | All 3 covers pass visual + seam inspection | → Merge | ↺ Repair defects (PROD-007/008/009) |
| QG-PROD-C1 | PROD-011 | Insulation Complete | Full coverage, correct thickness, no gaps | → Merge | ↺ Rework (PROD-011) |

#### Phase Exit Gate

| Gate | Checkpoint | Pass Criteria | Pass Action | Fail Action |
|------|------------|---------------|-------------|-------------|
| QG-PROD-4 | Pre-Pack Inspection | All components present, labeled, QC stamped | → LOG-001 | ↺ Rework/remake failed items → back to stream |

---

## Part 4: LOGISTICS

*From workshop to construction site*

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **LOG-001** | Component Packing | Pack all components for transport, create inventory | QG-PROD-4 passed |
| **LOG-002** | Loading & Securing | Load onto transport vehicle, secure for transit | Packing complete |
| **LOG-003** | Transport, Delivery & Site Handover | Deliver to site, track, unload, verify inventory with site contact | Vehicle loaded |

### LOGISTICS Quality Gates

| Gate | Checkpoint | Pass Criteria | Pass Action | Fail Action |
|------|------------|---------------|-------------|-------------|
| QG-LOG-1 | Packing Complete | All items on checklist packed, labeled | → LOG-002 | ↺ Complete packing (LOG-001) |
| QG-LOG-2 | Delivery Confirmed | Site contact signs inventory receipt, no damage | → ASSY-000 | Document damage via CORE-002, assess severity |

---

## Part 5: ASSEMBLY

*On-site construction*

### Pre-Assembly (ASSY-000 to ASSY-002)

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **ASSY-000** | Site Safety Briefing | PPE check, hazard identification, emergency procedures | Before any work |
| **ASSY-001** | Site Assessment & Preparation | Check ground, mark foundation, clear area | Day before assembly |
| **ASSY-002** | Foundation Setup | Level platform or ground preparation | Site approved |

### Structure (ASSY-003 to ASSY-006)

| SOP ID | Name | Purpose | Trigger | QG After |
|--------|------|---------|---------|----------|
| **ASSY-003** | Khana (Wall) Erection | Expand and connect lattice walls | Foundation ready (QG-ASSY-1) | - |
| **ASSY-004** | Door Frame Installation | Set door frame into wall ring | Walls standing | - |
| **ASSY-005** | Uni (Roof Poles) Installation | Connect roof poles to walls and crown | Door frame set | - |
| **ASSY-006** | Tono (Crown) Placement | Secure crown ring at apex | Roof poles up | QG-ASSY-2 |

### Covering (ASSY-007a to ASSY-007c)

| SOP ID | Name | Purpose | Trigger | QG After |
|--------|------|---------|---------|----------|
| **ASSY-007a** | Insulation Installation | Install insulation layer on walls and roof | Structure complete (QG-ASSY-2) | QG-ASSY-3a |
| **ASSY-007b** | Outer Cover Installation | Install wall and roof covers, secure, seal | Insulation complete | QG-ASSY-3b |
| **ASSY-007c** | Inner Liner Installation | Install decorative inner liner | Outer covers complete | - |

### Completion (ASSY-008)

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **ASSY-008** | Final Touches & Customer Handover | Windows, door hardware, finishing, walkthrough, sign-off | All covers installed |

### ASSEMBLY Quality Gates

| Gate | After | Check | Pass Criteria | Pass Action | Fail Action |
|------|-------|-------|---------------|-------------|-------------|
| QG-ASSY-0 | ASSY-000 | Safety Ready | All crew briefed, PPE confirmed | → ASSY-001 | ⛔ STOP WORK until resolved |
| QG-ASSY-1 | ASSY-002 | Foundation Level | Platform level within 5mm across diameter | → ASSY-003 | ↺ Re-level foundation (ASSY-002) |
| QG-ASSY-2 | ASSY-006 | Structure Stable | Walls plumb, roof poles secure, crown centered | → ASSY-007a | ↺ Structural adjustment (ASSY-003-006) |
| QG-ASSY-3a | ASSY-007a | Insulation Coverage | No gaps, correct thickness throughout | → ASSY-007b | ↺ Fill gaps (ASSY-007a) |
| QG-ASSY-3b | ASSY-007b | Weatherproof | All seams sealed, no visible gaps | → ASSY-007c | ↺ Reseal (ASSY-007b) |
| QG-ASSY-4 | ASSY-008 | Customer Sign-off | Customer walks through, signs acceptance | → CARE-001 | Create punch list → rework → re-inspect |

---

## Part 6: CARE (After-Sale & Repeat)

*Customer satisfaction, support, and relationship building*

### Immediate After-Care (CARE-001 to CARE-002)

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **CARE-001** | Post-Assembly Follow-up | Check-in call/message 48h after handover | Handover complete |
| **CARE-002** | Satisfaction Survey & Portfolio | Collect NPS, testimonial, photos for portfolio | 1 week post-handover |

### Support (CARE-003 to CARE-004)

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **CARE-003a** | Warranty Claim Handling | Process and resolve warranty/defect issues | Customer reports defect |
| **CARE-003b** | Service Complaint Handling | Handle non-warranty complaints (communication, delays, etc.) | Customer reports complaint |
| **CARE-004** | Maintenance Guidance | Provide seasonal care instructions, reminders | Quarterly schedule |

### Growth (CARE-005 to CARE-006)

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **CARE-005** | Referral Program | Incentivize and track customer referrals | Satisfied customer (NPS ≥ 8) |
| **CARE-006** | Repeat & Upsell | Offer additional yurts, upgrades, accessories | 6+ months post-delivery |

### CARE Quality Gates

| Gate | Checkpoint | Pass Criteria | Pass Action | Fail Action |
|------|------------|---------------|-------------|-------------|
| QG-CARE-1 | Customer Satisfied | NPS ≥ 8, no open complaints | → CARE-004 | Escalate to founder, trigger CORE-002 |
| QG-CARE-2 | Referral Active | Customer enrolled in referral program | → CARE-006 | ↺ Follow up in 30 days (CARE-005) |

---

## Complete File Structure

```
Glamplaybook/
├── SOPs/
│   ├── CORE/
│   │   ├── CORE-001_Customer_Communication_Protocol.md
│   │   ├── CORE-002_Issue_Exception_Handling.md
│   │   ├── CORE-003_Safety_PPE_Standards.md
│   │   └── CORE-004_Documentation_Photo_Capture.md
│   │
│   ├── SALES/
│   │   ├── SALES-001_Lead_Capture_Response.md
│   │   ├── SALES-002_Lead_Qualification_Scoring.md
│   │   ├── SALES-003_Onboarding_Multimedia.md
│   │   ├── SALES-004_Needs_Assessment_Site_Discovery.md
│   │   ├── SALES-005_Proposal_Creation.md
│   │   ├── SALES-006_Agreement_Closing.md
│   │   ├── SALES-007_Contract_Documentation.md
│   │   └── SALES-008_Invoicing_Payment.md
│   │
│   ├── PREP/
│   │   ├── PREP-001_Order_Intake_Specification.md
│   │   ├── PREP-002_Materials_Calculation.md
│   │   ├── PREP-003_Supplier_Ordering.md
│   │   ├── PREP-004_Materials_Receiving_QC.md
│   │   ├── PREP-005_Production_Planning.md
│   │   └── PREP-006_Workshop_Tool_Setup.md
│   │
│   ├── PROD/
│   │   ├── Stream_A_Wood/
│   │   │   ├── PROD-001_Wood_Selection_Cutting.md
│   │   │   ├── PROD-002_Wood_Treatment_Finishing.md
│   │   │   ├── PROD-003_Khana_Lattice_Assembly.md
│   │   │   ├── PROD-004_Uni_Roof_Poles.md
│   │   │   └── PROD-005_Tono_Crown_Ring.md
│   │   │
│   │   ├── Stream_B_Sewing/
│   │   │   ├── PROD-006_Canvas_Measurement_Cutting.md
│   │   │   ├── PROD-007_Wall_Cover_Sewing.md
│   │   │   ├── PROD-008_Roof_Cover_Sewing.md
│   │   │   └── PROD-009_Inner_Liner_Sewing.md
│   │   │
│   │   ├── Stream_C_Insulation/
│   │   │   ├── PROD-010_Insulation_Cutting.md
│   │   │   └── PROD-011_Insulation_Assembly.md
│   │   │
│   │   └── External_Hardware/
│   │       ├── PROD-012_Door_Window_Preparation.md
│   │       ├── PROD-013_Rope_Tensioning_Elements.md
│   │       └── PROD-014_Hardware_Connectors_Prep.md
│   │
│   ├── LOG/
│   │   ├── LOG-001_Component_Packing.md
│   │   ├── LOG-002_Loading_Securing.md
│   │   └── LOG-003_Transport_Delivery_Handover.md
│   │
│   ├── ASSY/
│   │   ├── Pre_Assembly/
│   │   │   ├── ASSY-000_Site_Safety_Briefing.md
│   │   │   ├── ASSY-001_Site_Assessment_Preparation.md
│   │   │   └── ASSY-002_Foundation_Setup.md
│   │   │
│   │   ├── Structure/
│   │   │   ├── ASSY-003_Khana_Wall_Erection.md
│   │   │   ├── ASSY-004_Door_Frame_Installation.md
│   │   │   ├── ASSY-005_Uni_Roof_Poles_Installation.md
│   │   │   └── ASSY-006_Tono_Crown_Placement.md
│   │   │
│   │   ├── Covering/
│   │   │   ├── ASSY-007a_Insulation_Installation.md
│   │   │   ├── ASSY-007b_Outer_Cover_Installation.md
│   │   │   └── ASSY-007c_Inner_Liner_Installation.md
│   │   │
│   │   └── Completion/
│   │       └── ASSY-008_Final_Touches_Handover.md
│   │
│   └── CARE/
│       ├── CARE-001_Post_Assembly_Followup.md
│       ├── CARE-002_Satisfaction_Survey_Portfolio.md
│       ├── CARE-003a_Warranty_Claim_Handling.md
│       ├── CARE-003b_Service_Complaint_Handling.md
│       ├── CARE-004_Maintenance_Guidance.md
│       ├── CARE-005_Referral_Program.md
│       └── CARE-006_Repeat_Upsell.md
│
├── Checklists/
│   ├── QC-CORE_Safety_Briefing.md
│   ├── QC-SALES_Lead_Qualification.md
│   ├── QC-PREP_Materials_Receiving.md
│   ├── QC-PROD-A_Wood_Stream.md
│   ├── QC-PROD-B_Sewing_Stream.md
│   ├── QC-PROD-C_Insulation_Stream.md
│   ├── QC-PROD_Pre_Pack_Inspection.md
│   ├── QC-LOG_Packing_Inventory.md
│   ├── QC-ASSY_Foundation_Level.md
│   ├── QC-ASSY_Structure_Stability.md
│   ├── QC-ASSY_Weatherproof.md
│   ├── QC-ASSY_Customer_Handover.md
│   └── QC-CARE_Satisfaction_Survey.md
│
├── QuickRef/
│   ├── CORE_Safety_Quick_Reference.pdf
│   ├── SALES_Quick_Reference.pdf
│   ├── PREP_Quick_Reference.pdf
│   ├── PROD_Wood_Quick_Reference.pdf
│   ├── PROD_Sewing_Quick_Reference.pdf
│   ├── PROD_Insulation_Quick_Reference.pdf
│   ├── LOG_Quick_Reference.pdf
│   ├── ASSY_Structure_Quick_Reference.pdf
│   ├── ASSY_Covering_Quick_Reference.pdf
│   └── CARE_Quick_Reference.pdf
│
└── templates/
    └── SOP_TEMPLATE.md
```

---

## Three-Tier Distribution

| Tier | Location | Format | Contents |
|------|----------|--------|----------|
| **ONLINE** | LMS / Course Platform | Video + MD + Quiz | Full SOPs with video walkthroughs |
| **OFFLINE** | Laptop at site | Local folder | PDF exports + video files |
| **PHYSICAL** | Workshop / Site | Laminated cards | Quick Reference + Safety |

### Sync Protocol

```
1. Master source: Online (LMS)
2. Before each project:
   └─ Export updated PDFs → Laptop folder
3. On version update:
   └─ Reprint laminated Quick Reference cards
4. Safety cards: Always current, check quarterly
```

---

## Complete Flow Visualization

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                         │
│  ╔═══════════════════════════════════════════════════════════════════════════════════╗  │
│  ║  CORE: CORE-001 (Comms) │ CORE-002 (Exceptions) │ CORE-003 (Safety) │ CORE-004   ║  │
│  ║  ─────────────────────────────────────────────────────────────────────────────────║  │
│  ║                    Applies to all phases below                                    ║  │
│  ╚═══════════════════════════════════════════════════════════════════════════════════╝  │
│                                                                                         │
│  ┌───────────────────────────────────────────────────────────────────────────────────┐  │
│  │  PART 1: SALES                                                                    │  │
│  │  001 → 002 → 003 → 004 → 005 → 006 → 007 → 008                                    │  │
│  │  [QG-1]     [QG-2]                         [QG-3]                                 │  │
│  └───────────────────────────────────────┬───────────────────────────────────────────┘  │
│                                          │                                              │
│                                          ▼                                              │
│  ┌───────────────────────────────────────────────────────────────────────────────────┐  │
│  │  PART 2: PREP                                                                     │  │
│  │  001 → 002 → 003 → 004 → 005 → 006                                                │  │
│  │  [QG-1]          [QG-2]     [QG-3]                                                │  │
│  └───────────────────────────────────────┬───────────────────────────────────────────┘  │
│                                          │                                              │
│                                          ▼                                              │
│  ┌───────────────────────────────────────────────────────────────────────────────────┐  │
│  │  PART 3: PRODUCTION                                                               │  │
│  │                                                                                   │  │
│  │   STREAM A (Wood)          STREAM B (Sewing)       STREAM C (Insulation)          │  │
│  │   001→002→003→004→005      006→007→008→009         010→011                        │  │
│  │      [A1] [A2]    [A3]        [B1][B2]   [B3]            [C1]                      │  │
│  │            │                      │                       │                       │  │
│  │            └──────────────────────┴───────────────────────┘                       │  │
│  │                                   │                                               │  │
│  │                    ┌──────────────▼──────────────┐                                │  │
│  │                    │  012 + 013 + 014            │                                │  │
│  │                    │  (External & Hardware)      │                                │  │
│  │                    └──────────────┬──────────────┘                                │  │
│  │                                   │                                               │  │
│  │                              [QG-PROD-4]                                          │  │
│  └───────────────────────────────────┬───────────────────────────────────────────────┘  │
│                                      │                                                  │
│                                      ▼                                                  │
│  ┌───────────────────────────────────────────────────────────────────────────────────┐  │
│  │  PART 4: LOGISTICS                                                                │  │
│  │  001 → 002 → 003                                                                  │  │
│  │  [QG-1]     [QG-2]                                                                │  │
│  └───────────────────────────────────┬───────────────────────────────────────────────┘  │
│                                      │                                                  │
│                                      ▼                                                  │
│  ┌───────────────────────────────────────────────────────────────────────────────────┐  │
│  │  PART 5: ASSEMBLY                                                                 │  │
│  │                                                                                   │  │
│  │  PRE:  000 → 001 → 002                                                            │  │
│  │       [QG-0]      [QG-1]                                                          │  │
│  │                     │                                                             │  │
│  │  STRUCT: 003 → 004 → 005 → 006                                                    │  │
│  │                          [QG-2]                                                   │  │
│  │                            │                                                      │  │
│  │  COVER: 007a → 007b → 007c                                                        │  │
│  │        [QG-3a] [QG-3b]                                                            │  │
│  │                   │                                                               │  │
│  │  COMPLETE: 008                                                                    │  │
│  │           [QG-4]                                                                  │  │
│  └───────────────────────────────────┬───────────────────────────────────────────────┘  │
│                                      │                                                  │
│                                      ▼                                                  │
│  ┌───────────────────────────────────────────────────────────────────────────────────┐  │
│  │  PART 6: CARE                                                                     │  │
│  │  001 → 002 → 003a/003b → 004 → 005 → 006                                          │  │
│  │            [QG-1]              [QG-2]                                              │  │
│  │                                   │                                               │  │
│  │                                   └──────────────────┐                            │  │
│  └──────────────────────────────────────────────────────┼────────────────────────────┘  │
│                                                         │                               │
│                                                         ▼                               │
│                                               ┌─────────────────┐                       │
│                                               │  LOOP TO SALES  │                       │
│                                               │  (Repeat Order) │                       │
│                                               └─────────────────┘                       │
│                                                                                         │
└─────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## SOP Summary Table

| Part | Name | SOPs | Quality Gates | Focus | Priority |
|------|------|------|---------------|-------|----------|
| **0** | CORE | 4 | - | Cross-cutting | **HIGH** |
| **1** | SALES | 8 | 3 | Lead → Order | Later |
| **2** | PREP | 6 | 3 | Order → Ready | Medium |
| **3** | PROD | 14 | 8 | Raw → Components | **HIGH** |
| **4** | LOG | 3 | 2 | Workshop → Site | Medium |
| **5** | ASSY | 11 | 6 | Components → Yurt | **HIGH** |
| **6** | CARE | 7 | 2 | Satisfaction → Repeat | Later |
| | **TOTAL** | **53** | **24** | | |

---

## Quality Gate Summary

| Phase | Gates | Critical Gates | Fail Pattern |
|-------|-------|----------------|--------------|
| SALES | 3 | QG-SALES-3 (Payment) | Archive / Revise / Hold |
| PREP | 3 | QG-PREP-2 (Materials QC) | Clarify / Reorder / Resolve |
| PROD | 8 | QG-PROD-4 (Pre-Pack) | ↺ Rework loop to source step |
| LOG | 2 | QG-LOG-2 (Delivery) | Complete / CORE-002 |
| ASSY | 6 | QG-ASSY-0 (Safety), QG-ASSY-4 (Handover) | ⛔ Stop / ↺ Rework / Punch list |
| CARE | 2 | QG-CARE-1 (Satisfaction) | Escalate / Follow-up |
| **TOTAL** | **24** | | |

### Quality Gate Decision Pattern

```
                    ┌─────────────────┐
                    │    Process      │
                    │    (SOP-XXX)    │
                    └────────┬────────┘
                             │
                             ▼
                      ╔═════════════╗
                      ║   QG-XXX    ║
                      ║   Check?    ║
                      ╚══════╤══════╝
                             │
              ┌──────────────┼──────────────┐
              │              │              │
              ▼              │              ▼
        ┌─────────┐          │        ┌─────────┐
        │   YES   │          │        │   NO    │
        │  (Pass) │          │        │ (Fail)  │
        └────┬────┘          │        └────┬────┘
             │               │             │
             ▼               │             ▼
    ┌─────────────────┐      │    ┌─────────────────────┐
    │  Next Process   │      │    │   Fail Action:      │
    │  (Continue)     │      │    │   ↺ Rework loop     │
    └─────────────────┘      │    │   ⛔ Stop work      │
                             │    │   → CORE-002        │
                             │    │   → Escalate        │
                             │    └─────────────────────┘
```

---

## Priority for Documentation Sprint (Dec 2025 - Feb 2026)

### P0: Critical (Document First)
| SOP | Reason |
|-----|--------|
| CORE-002 | Exception handling prevents chaos |
| CORE-003 | Safety is non-negotiable for franchise |
| PROD-003 | Khana assembly is core skill |
| PROD-007 | Wall cover sewing requires precision |
| ASSY-003 | Wall erection is make-or-break |
| ASSY-007b | Outer cover affects weatherproofing |

### P1: High Priority
| SOP | Reason |
|-----|--------|
| ASSY-000 | Safety briefing for liability |
| PREP-004 | Materials QC prevents downstream issues |
| LOG-001 | Packing errors = site problems |
| ASSY-002 | Foundation determines everything |

### P2: Medium Priority
| SOP | Reason |
|-----|--------|
| CORE-001 | Customer communication standardization |
| CORE-004 | Documentation for QC evidence |
| PROD-001/002 | Wood selection and treatment |
| All other PROD | Complete production documentation |

### P3: Lower Priority (Document After Pilot)
| SOP | Reason |
|-----|--------|
| SALES-* | Currently founder knowledge, relationship-based |
| CARE-* | Focus after first satisfied customers from pilot |

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | Dec 2025 | Initial structure (43 SOPs) |
| 2.0 | Dec 2025 | Systemologist optimization: +CORE category, split ASSY-007, added in-process QGs, merged LOG-003/004, added PREP-006, PROD-002, PROD-013, ASSY-000, CARE-003b. Total: 53 SOPs, 24 QGs |
| 2.1 | Dec 2025 | Added Pass/Fail actions to all Quality Gates, added QG Decision Pattern diagram, updated critical gates |

---

*Document created: December 2025*
*Optimized: December 2025*
*Next review: After March 2026 pilot assembly*
