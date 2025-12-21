# Miro AI Flowchart Prompts - Enklava Yurts SOP Infrastructure v2.1

## Strategy: 13 Modular Flowcharts → Manual Assembly

**Workflow:**
1. Create each section as a separate flowchart using prompts below
2. Manually drag them side-by-side in Miro (left to right)
3. Manually add connecting arrows between columns
4. Add title and legend

---

## Prompt 1: CORE Column

```
Create a vertical flowchart titled "CORE - Cross-Cutting SOPs"

Header bar: Dark gray (#4A4A4A), white text "CORE"

[BOX] CORE-001: Customer Communication Protocol
  ↓
[BOX] CORE-002: Issue & Exception Handling
  ↓
[BOX] CORE-003: Safety & PPE Standards
  ↓
[BOX] CORE-004: Documentation & Photo Capture

Styling:
- Gray boxes (#D9D9D9) with dark gray border
- Each box shows ID on first line (bold), name on second line
- Add dashed arrow pointing RIGHT from each box
- Footer text: "4 SOPs | Applies to ALL phases →"
- Make column narrow
```

---

## Prompt 2: SALES Column

```
Create a vertical flowchart titled "SALES - Lead to Order"

Header bar: Yellow (#FFD966), text "SALES"

[BOX] SALES-001: Lead Capture
  ↓
[BOX] SALES-002: Lead Qualification
  ↓
[DIAMOND] QG-1: Qualified?
  → YES → SALES-003
  → NO  → EXIT gray box "Archive/Nurture"
  ↓
[BOX] SALES-003: Onboarding Multimedia
  ↓
[BOX] SALES-004: Needs Assessment
  ↓
[BOX] SALES-005: Proposal Creation
  ↓
[DIAMOND] QG-2: Accepted?
  → YES → SALES-006
  → NO  → LOOP back to SALES-005 "Revise"
  ↓
[BOX] SALES-006: Agreement & Close
  ↓
[BOX] SALES-007: Contract
  ↓
[BOX] SALES-008: Payment
  ↓
[DIAMOND] QG-3: Paid?
  → YES → EXIT box "→ PREP"
  → NO  → box "Hold/Remind" with loop arrow

Styling:
- Yellow boxes (#FFF2CC fill, #FFD966 border)
- Orange diamonds (#F6B26B)
- Green arrows for YES, red dashed for NO
- Footer: "8 SOPs | 3 QGs"
```

---

## Prompt 3: PREP Column

```
Create a vertical flowchart titled "PREP - Production Preparation"

Header bar: Blue (#9FC5E8), text "PREP"

[BOX] PREP-001: Order Intake & Specification
  ↓
[DIAMOND] QG-1: Specs Confirmed?
  → YES → PREP-002
  → NO  → LOOP to PREP-001 "Clarify"
  ↓
[BOX] PREP-002: Materials Calculation
  ↓
[BOX] PREP-003: Supplier Ordering
  ↓
[BOX] PREP-004: Materials Receiving QC
  ↓
[DIAMOND] QG-2: Materials OK?
  → YES → PREP-005
  → NO  → box "Reject" → LOOP to PREP-003
  ↓
[BOX] PREP-005: Production Planning
  ↓
[BOX] PREP-006: Workshop & Tool Setup
  ↓
[DIAMOND] QG-3: Ready?
  → YES → EXIT box "→ PROD"
  → NO  → box "Resolve Blockers" → LOOP to PREP-005

Styling:
- Blue boxes (#CFE2F3 fill, #9FC5E8 border)
- Orange diamonds (#F6B26B)
- Footer: "6 SOPs | 3 QGs"
```

---

## Prompt 4: PROD Column - Stream A (Wood)

```
Create a vertical flowchart titled "PROD - Stream A: Wood"

Header bar: Green (#93C47D), text "WOOD"

[BOX] PROD-001: Wood Selection & Cutting
  ↓
[DIAMOND] QG-A1: Accurate?
  → YES → PROD-002
  → NO  → LOOP to PROD-001 "Recut"
  ↓
[BOX] PROD-002: Wood Treatment & Finishing
  ↓
[BOX] PROD-003: Khana Lattice Assembly
  ↓
[DIAMOND] QG-A2: Structure OK?
  → YES → PROD-004
  → NO  → LOOP to PROD-003 "Repair"
  ↓
[BOX] PROD-004: Uni Roof Poles
  ↓
[BOX] PROD-005: Tono Crown Ring
  ↓
[DIAMOND] QG-A3: Complete?
  → YES → EXIT box "→ MERGE"
  → NO  → LOOP to PROD-005 "Rebuild"

Styling:
- Light green boxes (#B6D7A8 fill, #93C47D border)
- Small orange diamonds
- Footer: "5 SOPs | 3 QGs"
```

---

## Prompt 5: PROD Column - Stream B (Sewing)

```
Create a vertical flowchart titled "PROD - Stream B: Sewing"

Header bar: Green (#93C47D) with blue tint, text "SEWING"

[BOX] PROD-006: Canvas Measurement & Cutting
  ↓
[DIAMOND] QG-B1: Cut OK?
  → YES → PROD-007
  → NO  → LOOP to PROD-006 "Recut"
  ↓
[BOX] PROD-007: Wall Cover Sewing
  ↓
[DIAMOND] QG-B2: Seams OK?
  → YES → PROD-008
  → NO  → LOOP to PROD-007 "Resew"
  ↓
[BOX] PROD-008: Roof Cover Sewing
  ↓
[BOX] PROD-009: Inner Liner Sewing
  ↓
[DIAMOND] QG-B3: All Covers OK?
  → YES → EXIT box "→ MERGE"
  → NO  → LOOP to affected row "Repair"

Styling:
- Light blue-green boxes (#A4C2F4 fill)
- Small orange diamonds
- Footer: "4 SOPs | 3 QGs"
```

---

## Prompt 6: PROD Column - Stream C (Insulation)

```
Create a vertical flowchart titled "PROD - Stream C: Insulation"

Header bar: Green (#93C47D) with orange tint, text "INSULATION"

[BOX] PROD-010: Insulation Cutting
  ↓
[BOX] PROD-011: Insulation Assembly
  ↓
[DIAMOND] QG-C1: Complete?
  → YES → EXIT box "→ MERGE"
  → NO  → LOOP to PROD-011 "Rework"

Styling:
- Light orange boxes (#F9CB9C fill)
- Small orange diamond
- Footer: "2 SOPs | 1 QG"
```

---

## Prompt 7: PROD Column - Merge & Exit

```
Create a flowchart section titled "PROD - External & Exit"

Three boxes in horizontal row:
[BOX] PROD-012: Door & Window Prep
[BOX] PROD-013: Rope & Tensioning
[BOX] PROD-014: Hardware & Connectors

All three connect down to:

[DIAMOND] QG-PROD-4: Pre-Pack Inspection OK?
  → YES → EXIT box "→ LOG"
  → NO  → three red dashed arrows up labeled "Rework Stream A/B/C"

Styling:
- Gray boxes (#D9D9D9)
- Large orange diamond for final QG
- Footer: "3 SOPs | 1 QG (Final)"
```

---

## Prompt 8: LOG Column

```
Create a vertical flowchart titled "LOG - Logistics"

Header bar: Purple (#B4A7D6), text "LOGISTICS"

[BOX] LOG-001: Component Packing
  ↓
[DIAMOND] QG-1: All Packed?
  → YES → LOG-002
  → NO  → LOOP to LOG-001 "Complete"
  ↓
[BOX] LOG-002: Loading & Securing
  ↓
[BOX] LOG-003: Transport, Delivery & Handover
  ↓
[DIAMOND] QG-2: Delivered OK?
  → YES → EXIT box "→ ASSY"
  → NO  → box "Document Damage" → "CORE-002"

Styling:
- Purple boxes (#D9D2E9 fill, #B4A7D6 border)
- Orange diamonds
- Make column narrow
- Footer: "3 SOPs | 2 QGs"
```

---

## Prompt 9: ASSY Column - Pre-Assembly

```
Create a flowchart section titled "ASSY - Pre-Assembly"

Light red container box (#F4CCCC) with label "PRE-ASSEMBLY"

Inside container:

[BOX] ASSY-000: Site Safety Briefing
  ↓
[DIAMOND] QG-0: Safety OK?
  → YES → ASSY-001
  → NO  → red box "⛔ STOP WORK" (hard stop, no loop)
  ↓
[BOX] ASSY-001: Site Assessment & Preparation
  ↓
[BOX] ASSY-002: Foundation Setup
  ↓
[DIAMOND] QG-1: Foundation Level?
  → YES → EXIT container "→ STRUCTURE"
  → NO  → LOOP to ASSY-002 "Re-level"

Styling:
- Light red boxes inside light red container
- Orange diamonds, red stop box for QG-0 NO
- Footer: "3 SOPs | 2 QGs"
```

---

## Prompt 10: ASSY Column - Structure

```
Create a flowchart section titled "ASSY - Structure"

Medium red container box (#EA9999) with label "STRUCTURE"

Inside container:

[BOX] ASSY-003: Khana Wall Erection
  ↓
[BOX] ASSY-004: Door Frame Installation
  ↓
[BOX] ASSY-005: Uni Roof Poles Installation
  ↓
[BOX] ASSY-006: Tono Crown Placement
  ↓
[DIAMOND] QG-2: Structure Stable?
  → YES → EXIT container "→ COVERING"
  → NO  → LOOP to ASSY-003 "Adjust"

Styling:
- Red-tinted boxes inside container
- Orange diamond
- Footer: "4 SOPs | 1 QG"
```

---

## Prompt 11: ASSY Column - Covering

```
Create a flowchart section titled "ASSY - Covering"

Red container box (#E06666) with label "COVERING"

Inside container:

[BOX] ASSY-007a: Insulation Installation
  ↓
[DIAMOND] QG-3a: Coverage OK?
  → YES → ASSY-007b
  → NO  → LOOP to ASSY-007a "Fill Gaps"
  ↓
[BOX] ASSY-007b: Outer Cover Installation
  ↓
[DIAMOND] QG-3b: Sealed?
  → YES → ASSY-007c
  → NO  → LOOP to ASSY-007b "Reseal"
  ↓
[BOX] ASSY-007c: Inner Liner Installation
  → EXIT container "→ COMPLETION"

Styling:
- Red boxes inside red container
- Orange diamonds
- Footer: "3 SOPs | 2 QGs"
```

---

## Prompt 12: ASSY Column - Completion

```
Create a flowchart section titled "ASSY - Completion"

Dark red container box (#CC0000) with white text label "COMPLETION"

Inside container:

[BOX] ASSY-008: Final Touches & Customer Handover
  ↓
[DIAMOND] QG-4: Customer Accepts?
  → YES → EXIT box "→ CARE"
  → NO  → box "Punch List" → LOOP to ASSY-008

Styling:
- Dark red container, white text for label
- Box inside slightly lighter
- Footer: "1 SOP | 1 QG (Final)"
```

---

## Prompt 13: CARE Column

```
Create a vertical flowchart titled "CARE - After-Sale & Repeat"

Header bar: Teal (#76A5AF), text "CARE"

[BOX] CARE-001: Post-Assembly Follow-up (48h)
  ↓
[BOX] CARE-002: Satisfaction Survey & Portfolio
  ↓
[DIAMOND] QG-1: NPS ≥ 8?
  → YES → CARE-003
  → NO  → box "Escalate → CORE-002"
  ↓
[BOX] CARE-003a: Warranty Claims    [BOX] CARE-003b: Service Complaints
  (side by side, both connect down)
  ↓
[BOX] CARE-004: Maintenance Guidance
  ↓
[BOX] CARE-005: Referral Program
  ↓
[DIAMOND] QG-2: Referred?
  → YES → CARE-006
  → NO  → LOOP to CARE-005 "Follow up 30d"
  ↓
[BOX] CARE-006: Repeat & Upsell
  ↓
Curved arrow pointing LEFT: "→ SALES (Repeat Order)"

Styling:
- Teal boxes (#B2D8D8 fill, #76A5AF border)
- Orange diamonds
- Footer: "7 SOPs | 2 QGs"
```

---

## Manual Assembly Instructions

### Step 1: Create All Flowcharts
Run prompts 1-13 in Miro AI, creating 13 separate elements.

### Step 2: Arrange in Miro
Drag and arrange left to right:

```
┌──────┬───────┬──────┬─────────────────────────────┬──────┬─────────────────────────────┬──────┐
│      │       │      │           PROD              │      │           ASSY              │      │
│ CORE │ SALES │ PREP │ ┌─────┬───────┬─────┬─────┐ │ LOG  │ ┌─────┬───────┬──────┬────┐ │ CARE │
│      │       │      │ │Wood │Sewing │Insul│Merge│ │      │ │ Pre │Struct │Cover │Done│ │      │
│      │       │      │ └─────┴───────┴─────┴─────┘ │      │ └─────┴───────┴──────┴────┘ │      │
└──────┴───────┴──────┴─────────────────────────────┴──────┴─────────────────────────────┴──────┘
```

### Step 3: Align
- Align all column headers at same Y position
- Align PROD streams (Wood, Sewing, Insulation) horizontally within PROD area
- Align ASSY sections (Pre, Structure, Covering, Completion) vertically within ASSY area

### Step 4: Connect Exit Points
Draw arrows between columns:
| From | To | Label |
|------|-----|-------|
| SALES QG-3 YES | PREP Row 1 | "→ PREP" |
| PREP QG-3 YES | PROD Streams (top) | "→ PROD" |
| PROD Streams | PROD Merge | (arrows down) |
| PROD QG-4 YES | LOG Row 1 | "→ LOG" |
| LOG QG-2 YES | ASSY Pre Row 1 | "→ ASSY" |
| ASSY QG-4 YES | CARE Row 1 | "→ CARE" |
| CARE Row 9 | SALES Row 1 | "→ SALES (Repeat)" curved |

### Step 5: Add CORE References
Draw dashed gray lines from CORE boxes pointing right across all columns.

### Step 6: Add Title & Legend

**Title (top center):**
```
ENKLAVA YURTS - SOP INFRASTRUCTURE v2.1
53 SOPs | 24 Quality Gates | Complete Client Flow
December 2025
```

**Legend (bottom right):**
```
┌─────────────────────────────────────────┐
│ LEGEND                                  │
│                                         │
│ [BOX]     = SOP Process                 │
│ [DIAMOND] = Quality Gate (Decision)     │
│                                         │
│ → YES →   = Pass (green arrow)          │
│ → NO  →   = Fail (red dashed)           │
│ LOOP      = Rework loop                 │
│ EXIT      = Proceed to next phase       │
│ ⛔        = Hard stop (safety)          │
│ CORE →    = Cross-cutting reference     │
└─────────────────────────────────────────┘
```

**Color Key (bottom left):**
```
CORE: Gray #4A4A4A     SALES: Yellow #FFD966
PREP: Blue #9FC5E8     PROD: Green #93C47D
LOG: Purple #B4A7D6    ASSY: Red #E06666
CARE: Teal #76A5AF
```

---

## Prompt Summary

| # | Prompt | Creates | SOPs | QGs |
|---|--------|---------|------|-----|
| 1 | CORE | Cross-cutting column | 4 | - |
| 2 | SALES | Sales funnel | 8 | 3 |
| 3 | PREP | Preparation column | 6 | 3 |
| 4 | PROD-A | Wood stream | 5 | 3 |
| 5 | PROD-B | Sewing stream | 4 | 3 |
| 6 | PROD-C | Insulation stream | 2 | 1 |
| 7 | PROD-Merge | External + exit | 3 | 1 |
| 8 | LOG | Logistics column | 3 | 2 |
| 9 | ASSY-Pre | Pre-assembly section | 3 | 2 |
| 10 | ASSY-Struct | Structure section | 4 | 1 |
| 11 | ASSY-Cover | Covering section | 3 | 2 |
| 12 | ASSY-Done | Completion section | 1 | 1 |
| 13 | CARE | After-sale column | 7 | 2 |
| **Total** | **13 prompts** | **7 columns** | **53** | **24** |

---

*Created: December 2025*
*For: Enklava Yurts SOP Infrastructure v2.1*
*Format: Hybrid notation for Miro AI*
