# Enklava Yurts: SOP Infrastructure

## Complete Client Flow Coverage

```
┌──────────────────────────────────────────────────────────────────────────────────────────┐
│                           ENKLAVA YURTS - COMPLETE SOP SUITE                             │
├──────────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                          │
│  ┌─────────┐   ┌─────────┐   ┌─────────┐   ┌─────────┐   ┌─────────┐   ┌─────────┐      │
│  │  SALES  │ → │  PREP   │ → │  PROD   │ → │   LOG   │ → │  ASSY   │ → │  CARE   │      │
│  │ Part 0  │   │ Part 1  │   │ Part 2  │   │ Part 3  │   │ Part 4  │   │ Part 5  │      │
│  └─────────┘   └─────────┘   └─────────┘   └─────────┘   └─────────┘   └─────────┘      │
│                                                                                          │
│   8 SOPs        5 SOPs       12 SOPs        4 SOPs        8 SOPs        6 SOPs          │
│                                                                                          │
│   Attention    Order         Wood          Pack          Site          Follow-up        │
│   Engagement   Materials     Sewing        Load          Foundation    Warranty         │
│   Enquiry      Suppliers     Insulation    Transport     Structure     Referrals        │
│   Sales        Receiving     External      Deliver       Covers        Maintenance      │
│   Money        Planning                                  Handover      Repeat           │
│   Orders                                                                                 │
│                                                                                          │
├──────────────────────────────────────────────────────────────────────────────────────────┤
│                              TOTAL: 43 SOPs + Quality Gates                              │
└──────────────────────────────────────────────────────────────────────────────────────────┘
```

### CCF Mapping

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│  CRITICAL CLIENT FLOW (Jurta v3.0)           →    SOP COVERAGE                          │
├─────────────────────────────────────────────────────────────────────────────────────────┤
│  Attention ─┐                                                                           │
│  Engagement ├─→ PART 0: SALES                                                           │
│  Enquiry    │   (Lead → Customer)                                                       │
│  Sales      │                                                                           │
│  Money      │                                                                           │
│  Orders ────┘                                                                           │
│       │                                                                                 │
│       ▼                                                                                 │
│  ─────────────────────────────────────────────────────────────────────────────────────  │
│       │                                                                                 │
│       ├─→ PART 1: PREP         (Order → Production Ready)                               │
│       │                                                                                 │
│  Production ─→ PART 2: PROD    (Raw Materials → Components)                             │
│       │        ├─ Wood Stream                                                           │
│       │        ├─ Sewing Stream                                                         │
│       │        └─ Insulation Stream                                                     │
│       │                                                                                 │
│  Delivery ───→ PART 3: LOG     (Workshop → Site)                                        │
│       │                                                                                 │
│  Assembly ───→ PART 4: ASSY    (Components → Standing Yurt)                             │
│       │                                                                                 │
│  ─────────────────────────────────────────────────────────────────────────────────────  │
│       │                                                                                 │
│  Repeat ─────→ PART 5: CARE    (Satisfied Customer → Ambassador)                        │
│                                                                                         │
└─────────────────────────────────────────────────────────────────────────────────────────┘

LEGEND:
═══════════════════════════════════════════════════════════════
  PART 0 + PART 5  = Customer Relationship (before & after)
  PART 1-4         = Physical Operations (current focus) ◀◀◀
═══════════════════════════════════════════════════════════════
```

---

## Part 0: SALES (Lead to Order)

*From first contact to signed agreement and payment*

### Acquisition (SALES-001 to SALES-003)

| SOP ID | Name | Purpose | CCF Stage |
|--------|------|---------|-----------|
| **SALES-001** | Lead Capture & Response | Respond to inquiries from all channels within 24h | Attention → Engagement |
| **SALES-002** | Channel Management | Manage Facebook, Messenger, WhatsApp, personal referrals | Engagement |
| **SALES-003** | Onboarding Multimedia Delivery | Send intro videos, photos, testimonials | Engagement → Enquiry |

### Conversion (SALES-004 to SALES-006)

| SOP ID | Name | Purpose | CCF Stage |
|--------|------|---------|-----------|
| **SALES-004** | Needs Assessment & Discovery | Define client requirements, site conditions, budget | Enquiry |
| **SALES-005** | Proposal Creation | Build customized proposal with specs and pricing | Sales |
| **SALES-006** | Agreement & Closing | Present proposal, handle objections, close deal | Sales |

### Transaction (SALES-007 to SALES-008)

| SOP ID | Name | Purpose | CCF Stage |
|--------|------|---------|-----------|
| **SALES-007** | Contract & Documentation | Generate agreement, collect signatures | Money |
| **SALES-008** | Invoicing & Payment Collection | Issue invoice, track payment, confirm receipt | Money → Orders |

### SALES Quality Gates

| Gate | Checkpoint | Pass Criteria |
|------|------------|---------------|
| QG-SALES-1 | Lead Qualified | Budget, timeline, site confirmed viable |
| QG-SALES-2 | Proposal Accepted | Customer confirms specs in writing |
| QG-SALES-3 | Payment Received | Deposit/full payment cleared |

---

## Part 1: PREP (Production Preparation)

*Before any production starts - planning, ordering, workspace setup*

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **PREP-001** | Order Intake & Specification | Convert signed agreement into production specs | Agreement signed |
| **PREP-002** | Materials Calculation | Calculate exact materials needed per order | Specs confirmed |
| **PREP-003** | Supplier Ordering | Order external components (windows, doors, skylight, connectors, canvases) | Materials calculated |
| **PREP-004** | Materials Receiving & QC | Inspect incoming materials, reject defects | Delivery arrives |
| **PREP-005** | Production Planning & Scheduling | Schedule the 3 parallel production streams | All materials ready |

### PREP Quality Gates

| Gate | Checkpoint | Pass Criteria |
|------|------------|---------------|
| QG-PREP-1 | Spec Confirmation | Customer sign-off on final specs |
| QG-PREP-2 | Materials Ready | All materials received and QC passed |
| QG-PREP-3 | Production Scheduled | All 3 streams have start dates |

---

## Part 2: PRODUCTION

*Three parallel streams + external orders*

### Stream A: Wooden Structure (PROD-001 to PROD-004)

| SOP ID | Name | Purpose | Output |
|--------|------|---------|--------|
| **PROD-001** | Wood Selection & Cutting | Cut battens to spec dimensions | Cut pieces |
| **PROD-002** | Khana (Wall Lattice) Assembly | Drill, connect lattice sections | Lattice panels |
| **PROD-003** | Uni (Roof Poles) Preparation | Shape and finish roof poles | Roof poles set |
| **PROD-004** | Tono (Crown Ring) Construction | Build the crown/skylight ring | Crown ring |

### Stream B: Sewing Covers (PROD-005 to PROD-008)

| SOP ID | Name | Purpose | Output |
|--------|------|---------|--------|
| **PROD-005** | Canvas Measurement & Cutting | Cut canvas to pattern | Cut canvas pieces |
| **PROD-006** | Wall Cover Sewing | Sew outer wall covering | Wall cover |
| **PROD-007** | Roof Cover Sewing | Sew roof cone covering | Roof cover |
| **PROD-008** | Inner Liner Sewing | Sew interior decorative liner | Inner liner |

### Stream C: Insulation Shaping (PROD-009 to PROD-010)

| SOP ID | Name | Purpose | Output |
|--------|------|---------|--------|
| **PROD-009** | Insulation Cutting | Cut insulation to pattern | Insulation pieces |
| **PROD-010** | Insulation Assembly | Layer and connect insulation | Insulation set |

### External Components (PROD-011 to PROD-012)

| SOP ID | Name | Purpose | Output |
|--------|------|---------|--------|
| **PROD-011** | Door & Window Fitting | Prep ordered doors/windows for install | Fitted openings |
| **PROD-012** | Hardware & Connectors Prep | Organize all metal connectors, ropes, stakes | Hardware kit |

### PRODUCTION Quality Gates

| Gate | Checkpoint | Pass Criteria |
|------|------------|---------------|
| QG-PROD-1 | Wood Structure Complete | All wooden components pass dimension check |
| QG-PROD-2 | Covers Complete | All covers pass seam strength test |
| QG-PROD-3 | Insulation Complete | Insulation passes thickness check |
| QG-PROD-4 | Pre-Pack Inspection | All components present, labeled, QC stamped |

---

## Part 3: LOGISTICS

*From workshop to construction site*

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **LOG-001** | Component Packing | Pack all components for transport | QG-PROD-4 passed |
| **LOG-002** | Loading & Securing | Load onto transport vehicle | Packing complete |
| **LOG-003** | Transport & Tracking | Deliver to site, track location | Vehicle loaded |
| **LOG-004** | Site Delivery & Handover | Unload, verify inventory with site contact | Arrival at site |

### LOGISTICS Quality Gates

| Gate | Checkpoint | Pass Criteria |
|------|------------|---------------|
| QG-LOG-1 | Packing Complete | All items on checklist packed |
| QG-LOG-2 | Delivery Confirmed | Site contact signs inventory receipt |

---

## Part 4: ASSEMBLY

*On-site construction*

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **ASSY-001** | Site Assessment & Preparation | Check ground, mark foundation | Day before assembly |
| **ASSY-002** | Foundation Setup | Level platform or ground preparation | Site approved |
| **ASSY-003** | Khana (Wall) Erection | Expand and connect lattice walls | Foundation ready |
| **ASSY-004** | Door Frame Installation | Set door frame into wall ring | Walls standing |
| **ASSY-005** | Uni (Roof Poles) Installation | Connect roof poles to walls and crown | Door frame set |
| **ASSY-006** | Tono (Crown) Placement | Secure crown ring at apex | Roof poles up |
| **ASSY-007** | Cover Installation | Install insulation, covers, liner | Structure complete |
| **ASSY-008** | Final Touches & Customer Handover | Windows, finishing, walkthrough, sign-off | Covers on |

### ASSEMBLY Quality Gates

| Gate | Checkpoint | Pass Criteria |
|------|------------|---------------|
| QG-ASSY-1 | Structure Stable | Walls and roof pass stability test |
| QG-ASSY-2 | Weatherproof | Covers sealed, no gaps |
| QG-ASSY-3 | Customer Sign-off | Customer walks through, signs acceptance |

---

## Part 5: CARE (After-Sale & Repeat)

*Customer satisfaction, support, and relationship building*

### Immediate After-Care (CARE-001 to CARE-002)

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **CARE-001** | Post-Assembly Follow-up | Check-in call/message 48h after handover | Handover complete |
| **CARE-002** | Satisfaction Survey | Collect NPS, testimonial, photos | 1 week post-handover |

### Support (CARE-003 to CARE-004)

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **CARE-003** | Warranty Claim Handling | Process and resolve warranty issues | Customer reports issue |
| **CARE-004** | Maintenance Guidance | Provide seasonal care instructions | Quarterly reminders |

### Growth (CARE-005 to CARE-006)

| SOP ID | Name | Purpose | Trigger |
|--------|------|---------|---------|
| **CARE-005** | Referral Program | Incentivize and track customer referrals | Satisfied customer |
| **CARE-006** | Repeat & Upsell | Offer additional yurts, upgrades, accessories | 6+ months post-delivery |

### CARE Quality Gates

| Gate | Checkpoint | Pass Criteria |
|------|------------|---------------|
| QG-CARE-1 | Customer Satisfied | NPS ≥ 8, no open complaints |
| QG-CARE-2 | Referral Active | Customer enrolled in referral program |

---

## Complete File Structure

```
Glamplaybook/
├── SOPs/
│   ├── SALES/
│   │   ├── SALES-001_Lead_Capture_Response.md
│   │   ├── SALES-002_Channel_Management.md
│   │   ├── SALES-003_Onboarding_Multimedia.md
│   │   ├── SALES-004_Needs_Assessment.md
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
│   │   └── PREP-005_Production_Planning.md
│   │
│   ├── PROD/
│   │   ├── PROD-001_Wood_Selection_Cutting.md
│   │   ├── PROD-002_Khana_Lattice_Assembly.md
│   │   ├── PROD-003_Uni_Roof_Poles.md
│   │   ├── PROD-004_Tono_Crown_Ring.md
│   │   ├── PROD-005_Canvas_Measurement_Cutting.md
│   │   ├── PROD-006_Wall_Cover_Sewing.md
│   │   ├── PROD-007_Roof_Cover_Sewing.md
│   │   ├── PROD-008_Inner_Liner_Sewing.md
│   │   ├── PROD-009_Insulation_Cutting.md
│   │   ├── PROD-010_Insulation_Assembly.md
│   │   ├── PROD-011_Door_Window_Fitting.md
│   │   └── PROD-012_Hardware_Connectors_Prep.md
│   │
│   ├── LOG/
│   │   ├── LOG-001_Component_Packing.md
│   │   ├── LOG-002_Loading_Securing.md
│   │   ├── LOG-003_Transport_Tracking.md
│   │   └── LOG-004_Site_Delivery_Handover.md
│   │
│   ├── ASSY/
│   │   ├── ASSY-001_Site_Assessment_Preparation.md
│   │   ├── ASSY-002_Foundation_Setup.md
│   │   ├── ASSY-003_Khana_Wall_Erection.md
│   │   ├── ASSY-004_Door_Frame_Installation.md
│   │   ├── ASSY-005_Uni_Roof_Poles_Installation.md
│   │   ├── ASSY-006_Tono_Crown_Placement.md
│   │   ├── ASSY-007_Cover_Installation.md
│   │   └── ASSY-008_Final_Touches_Handover.md
│   │
│   └── CARE/
│       ├── CARE-001_Post_Assembly_Followup.md
│       ├── CARE-002_Satisfaction_Survey.md
│       ├── CARE-003_Warranty_Claim_Handling.md
│       ├── CARE-004_Maintenance_Guidance.md
│       ├── CARE-005_Referral_Program.md
│       └── CARE-006_Repeat_Upsell.md
│
├── Checklists/
│   ├── QC-SALES_Lead_Qualification.md
│   ├── QC-PREP_Materials_Receiving.md
│   ├── QC-PROD_Pre_Pack_Inspection.md
│   ├── QC-LOG_Packing_Inventory.md
│   ├── QC-ASSY_Structure_Stability.md
│   ├── QC-ASSY_Customer_Handover.md
│   └── QC-CARE_Satisfaction_Survey.md
│
├── QuickRef/
│   ├── SALES_Quick_Reference.pdf
│   ├── PREP_Quick_Reference.pdf
│   ├── PROD_Wood_Quick_Reference.pdf
│   ├── PROD_Sewing_Quick_Reference.pdf
│   ├── LOG_Quick_Reference.pdf
│   ├── ASSY_Quick_Reference.pdf
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
| **PHYSICAL** | Workshop / Site | Laminated cards | Quick Reference only |

### Sync Protocol

```
1. Master source: Online (LMS)
2. Before each project:
   └─ Export updated PDFs → Laptop folder
3. On version update:
   └─ Reprint laminated Quick Reference cards
```

---

## Complete Flow Visualization

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                         │
│  ╔═══════════════════════════════════════════════════════════════════════════════════╗  │
│  ║                            PART 0: SALES                                          ║  │
│  ║  SALES-001 → 002 → 003 → 004 → 005 → 006 → 007 → 008                              ║  │
│  ║  (Lead)     (Channels) (Onboard) (Needs) (Proposal) (Close) (Contract) (Payment)  ║  │
│  ╚═══════════════════════════════════════════════════════════════════════════════════╝  │
│                                          │                                              │
│                                          ▼                                              │
│  ┌───────────────────────────────────────────────────────────────────────────────────┐  │
│  │                              PART 1: PREP                                         │  │
│  │              PREP-001 → 002 → 003 → 004 → 005                                     │  │
│  └───────────────────────────────────────┬───────────────────────────────────────────┘  │
│                                          │                                              │
│                                          ▼                                              │
│  ┌───────────────────────────────────────────────────────────────────────────────────┐  │
│  │                              PART 2: PRODUCTION                                   │  │
│  │                                                                                   │  │
│  │      ┌──────────────┐   ┌──────────────┐   ┌──────────────┐                       │  │
│  │      │    WOOD      │   │   SEWING     │   │  INSULATION  │                       │  │
│  │      │  PROD 001-004│   │  PROD 005-008│   │  PROD 009-010│                       │  │
│  │      └──────┬───────┘   └──────┬───────┘   └──────┬───────┘                       │  │
│  │             │                  │                  │                               │  │
│  │             └──────────────────┼──────────────────┘                               │  │
│  │                                │                                                  │  │
│  │                    ┌───────────▼───────────┐                                      │  │
│  │                    │  PROD 011-012         │                                      │  │
│  │                    │  (External & Hardware)│                                      │  │
│  │                    └───────────┬───────────┘                                      │  │
│  └────────────────────────────────┬──────────────────────────────────────────────────┘  │
│                                   │                                                     │
│                                   ▼                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────────┐  │
│  │                              PART 3: LOGISTICS                                    │  │
│  │                    LOG-001 → 002 → 003 → 004                                      │  │
│  └───────────────────────────────────────┬───────────────────────────────────────────┘  │
│                                          │                                              │
│                                          ▼                                              │
│  ┌───────────────────────────────────────────────────────────────────────────────────┐  │
│  │                              PART 4: ASSEMBLY                                     │  │
│  │        ASSY-001 → 002 → 003 → 004 → 005 → 006 → 007 → 008                         │  │
│  └───────────────────────────────────────┬───────────────────────────────────────────┘  │
│                                          │                                              │
│                                          ▼                                              │
│  ╔═══════════════════════════════════════════════════════════════════════════════════╗  │
│  ║                              PART 5: CARE                                         ║  │
│  ║            CARE-001 → 002 → 003 → 004 → 005 → 006                                 ║  │
│  ║            (Follow-up) (Survey) (Warranty) (Maint) (Referral) (Repeat)            ║  │
│  ║                                          │                                        ║  │
│  ║                                          └────────────────┐                       ║  │
│  ╚══════════════════════════════════════════════════════════════════════════════════╝  │
│                                                              │                          │
│                                                              ▼                          │
│                                                    ┌─────────────────┐                  │
│                                                    │  LOOP TO SALES  │                  │
│                                                    │  (New Order)    │                  │
│                                                    └─────────────────┘                  │
│                                                                                         │
└─────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## SOP Summary Table

| Part | Name | SOPs | Focus | Priority |
|------|------|------|-------|----------|
| **0** | SALES | 8 | Lead → Order | Later |
| **1** | PREP | 5 | Order → Production Ready | Medium |
| **2** | PROD | 12 | Raw → Components | **HIGH** |
| **3** | LOG | 4 | Workshop → Site | Medium |
| **4** | ASSY | 8 | Components → Yurt | **HIGH** |
| **5** | CARE | 6 | Satisfaction → Repeat | Later |
| | **TOTAL** | **43** | | |

---

## Priority for Documentation Sprint (Dec 2025 - Feb 2026)

### High Priority (Document First) - PHYSICAL OPERATIONS
| SOP | Reason |
|-----|--------|
| PROD-002 | Core skill - Khana assembly is the heart of yurt |
| PROD-006/007 | Cover sewing requires precision |
| ASSY-003 | Wall erection is make-or-break moment |
| ASSY-007 | Cover installation affects weatherproofing |

### Medium Priority
| SOP | Reason |
|-----|--------|
| PREP-004 | QC at materials receiving prevents downstream issues |
| LOG-001 | Packing errors = site problems |
| ASSY-001/002 | Foundation determines everything |

### Lower Priority (Document After Pilot)
| SOP | Reason |
|-----|--------|
| SALES-* | Currently founder knowledge, relationship-based |
| CARE-* | Focus after first satisfied customers from pilot |
| PREP-001/002/003 | Less hands-on, can document from memory |

---

*Document created: December 2025*
*Next review: After March 2026 pilot assembly*
