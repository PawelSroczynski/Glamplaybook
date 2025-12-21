# Enklava Yurts: SOP Infrastructure

## Overview

```
┌─────────────────────────────────────────────────────────────────────────────┐
│  PREP          │  PRODUCTION        │  LOGISTICS      │  ASSEMBLY           │
│  (Before)      │  (Making)          │  (Moving)       │  (Building)         │
├────────────────┼────────────────────┼─────────────────┼─────────────────────┤
│  PREP-001-005  │  PROD-001-012      │  LOG-001-004    │  ASSY-001-008       │
│  5 SOPs        │  12 SOPs           │  4 SOPs         │  8 SOPs             │
└────────────────┴────────────────────┴─────────────────┴─────────────────────┘
                                                              TOTAL: 29 SOPs
```

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

## File Structure

```
Glamplaybook/
├── SOPs/
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
│   └── ASSY/
│       ├── ASSY-001_Site_Assessment_Preparation.md
│       ├── ASSY-002_Foundation_Setup.md
│       ├── ASSY-003_Khana_Wall_Erection.md
│       ├── ASSY-004_Door_Frame_Installation.md
│       ├── ASSY-005_Uni_Roof_Poles_Installation.md
│       ├── ASSY-006_Tono_Crown_Placement.md
│       ├── ASSY-007_Cover_Installation.md
│       └── ASSY-008_Final_Touches_Handover.md
│
├── Checklists/
│   ├── QC-PREP_Materials_Receiving.md
│   ├── QC-PROD_Pre_Pack_Inspection.md
│   ├── QC-LOG_Packing_Inventory.md
│   ├── QC-ASSY_Structure_Stability.md
│   └── QC-ASSY_Customer_Handover.md
│
├── QuickRef/
│   ├── PREP_Quick_Reference.pdf
│   ├── PROD_Wood_Quick_Reference.pdf
│   ├── PROD_Sewing_Quick_Reference.pdf
│   ├── LOG_Quick_Reference.pdf
│   └── ASSY_Quick_Reference.pdf
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

## Production Flow Visualization

```
                    ┌─────────────────────────────────────┐
                    │           PREP PHASE                │
                    │  PREP-001 → 002 → 003 → 004 → 005   │
                    └─────────────────┬───────────────────┘
                                      │
                    ┌─────────────────▼───────────────────┐
                    │         PRODUCTION PHASE            │
                    │                                     │
                    │  ┌─────────┐ ┌─────────┐ ┌───────┐ │
                    │  │  WOOD   │ │ SEWING  │ │ INSUL │ │
                    │  │ 001-004 │ │ 005-008 │ │009-010│ │
                    │  └────┬────┘ └────┬────┘ └───┬───┘ │
                    │       │           │          │      │
                    │       └───────────┼──────────┘      │
                    │                   │                 │
                    │          ┌────────▼────────┐        │
                    │          │ PROD-011 & 012  │        │
                    │          │ (External prep) │        │
                    │          └────────┬────────┘        │
                    └──────────────────┬──────────────────┘
                                       │
                    ┌──────────────────▼──────────────────┐
                    │         LOGISTICS PHASE             │
                    │    LOG-001 → 002 → 003 → 004        │
                    └──────────────────┬──────────────────┘
                                       │
                    ┌──────────────────▼──────────────────┐
                    │          ASSEMBLY PHASE             │
                    │  ASSY-001 → 002 → 003 → 004 →       │
                    │       → 005 → 006 → 007 → 008       │
                    └─────────────────────────────────────┘
```

---

## Priority for Documentation Sprint (Dec 2025 - Feb 2026)

### High Priority (Document First)
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

### Lower Priority (Can Document Later)
| SOP | Reason |
|-----|--------|
| PREP-001/002/003 | Currently founder knowledge, less hands-on |
| LOG-002/003 | Standard transport, less specialized |

---

*Document created: December 2025*
*Next review: After March 2026 pilot assembly*
