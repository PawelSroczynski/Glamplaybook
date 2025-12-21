# Miro AI Flowchart Prompts - Enklava Yurts SOP Infrastructure v2.1

## Strategy: 7 Standalone Flowcharts → Manual Assembly

**Workflow:**
1. Create each column as a separate flowchart using prompts below
2. Manually drag them side-by-side in Miro (left to right)
3. Manually add connecting arrows between columns
4. Add title and legend

---

## Prompt 1: CORE Column

```
Create a vertical flowchart titled "CORE - Cross-Cutting SOPs"

Header bar: Dark gray (#4A4A4A), white text "CORE"

Stack these 4 labeled boxes vertically, connected by down arrows:

Row 1: Box labeled "CORE-001" with subtitle "Customer Communication Protocol"
Row 2: Box labeled "CORE-002" with subtitle "Issue & Exception Handling"
Row 3: Box labeled "CORE-003" with subtitle "Safety & PPE Standards"
Row 4: Box labeled "CORE-004" with subtitle "Documentation & Photo Capture"

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

Stack these rows vertically, connected by arrows:

Row 1: Box "SALES-001" / "Lead Capture"
Row 2: Box "SALES-002" / "Lead Qualification"
Row 3: Diamond "QG-1" / "Qualified?"
        → YES (green arrow down): continue
        → NO (red arrow right): gray box "Archive/Nurture" (exit)
Row 4: Box "SALES-003" / "Onboarding Multimedia"
Row 5: Box "SALES-004" / "Needs Assessment"
Row 6: Box "SALES-005" / "Proposal Creation"
Row 7: Diamond "QG-2" / "Accepted?"
        → YES (green down): continue
        → NO (red left): arrow loops back to Row 6 with label "Revise"
Row 8: Box "SALES-006" / "Agreement & Close"
Row 9: Box "SALES-007" / "Contract"
Row 10: Box "SALES-008" / "Payment"
Row 11: Diamond "QG-3" / "Paid?"
        → YES (green right): box "→ PREP" (exit point)
        → NO (red down): box "Hold/Remind" with loop arrow

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

Stack these rows vertically:

Row 1: Box "PREP-001" / "Order Intake & Specification"
Row 2: Diamond "QG-1" / "Specs Confirmed?"
        → YES (green down): continue
        → NO (red left): loops to Row 1 with label "Clarify"
Row 3: Box "PREP-002" / "Materials Calculation"
Row 4: Box "PREP-003" / "Supplier Ordering"
Row 5: Box "PREP-004" / "Materials Receiving QC"
Row 6: Diamond "QG-2" / "Materials OK?"
        → YES (green down): continue
        → NO (red right): box "Reject" → loops to Row 4
Row 7: Box "PREP-005" / "Production Planning"
Row 8: Box "PREP-006" / "Workshop & Tool Setup"
Row 9: Diamond "QG-3" / "Ready?"
        → YES (green right): box "→ PROD" (exit)
        → NO (red down): box "Resolve Blockers" → loops to Row 7

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

Stack these rows vertically:

Row 1: Box "PROD-001" / "Wood Selection & Cutting"
Row 2: Small diamond "QG-A1" / "Accurate?"
        → YES (green down): continue
        → NO (red left): loops to Row 1 "Recut"
Row 3: Box "PROD-002" / "Wood Treatment & Finishing"
Row 4: Box "PROD-003" / "Khana Lattice Assembly"
Row 5: Small diamond "QG-A2" / "Structure OK?"
        → YES (green down): continue
        → NO (red left): loops to Row 4 "Repair"
Row 6: Box "PROD-004" / "Uni Roof Poles"
Row 7: Box "PROD-005" / "Tono Crown Ring"
Row 8: Small diamond "QG-A3" / "Complete?"
        → YES (green down): box "→ MERGE"
        → NO (red left): loops to Row 7 "Rebuild"

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

Stack these rows vertically:

Row 1: Box "PROD-006" / "Canvas Measurement & Cutting"
Row 2: Small diamond "QG-B1" / "Cut OK?"
        → YES (green down): continue
        → NO (red left): loops to Row 1 "Recut"
Row 3: Box "PROD-007" / "Wall Cover Sewing"
Row 4: Small diamond "QG-B2" / "Seams OK?"
        → YES (green down): continue
        → NO (red left): loops to Row 3 "Resew"
Row 5: Box "PROD-008" / "Roof Cover Sewing"
Row 6: Box "PROD-009" / "Inner Liner Sewing"
Row 7: Small diamond "QG-B3" / "All Covers OK?"
        → YES (green down): box "→ MERGE"
        → NO (red left): loops to affected row "Repair"

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

Stack these rows vertically:

Row 1: Box "PROD-010" / "Insulation Cutting"
Row 2: Box "PROD-011" / "Insulation Assembly"
Row 3: Small diamond "QG-C1" / "Complete?"
        → YES (green down): box "→ MERGE"
        → NO (red left): loops to Row 2 "Rework"

Styling:
- Light orange boxes (#F9CB9C fill)
- Small orange diamond
- Footer: "2 SOPs | 1 QG"
```

---

## Prompt 7: PROD Column - Merge & Exit

```
Create a flowchart section titled "PROD - External & Exit"

Three boxes in a horizontal row:
Box 1: "PROD-012" / "Door & Window Prep"
Box 2: "PROD-013" / "Rope & Tensioning"
Box 3: "PROD-014" / "Hardware & Connectors"

All three connect down to:

Row: Large diamond "QG-PROD-4" / "Pre-Pack Inspection OK?"
        → YES (green right): box "→ LOG" (exit)
        → NO (red up): three red dashed arrows going back up labeled "Rework Stream A/B/C"

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

Stack these rows vertically:

Row 1: Box "LOG-001" / "Component Packing"
Row 2: Diamond "QG-1" / "All Packed?"
        → YES (green down): continue
        → NO (red left): loops to Row 1 "Complete"
Row 3: Box "LOG-002" / "Loading & Securing"
Row 4: Box "LOG-003" / "Transport, Delivery & Handover"
Row 5: Diamond "QG-2" / "Delivered OK?"
        → YES (green right): box "→ ASSY" (exit)
        → NO (red down): box "Document Damage" → "CORE-002"

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

Inside, stack vertically:

Row 1: Box "ASSY-000" / "Site Safety Briefing"
Row 2: Diamond "QG-0" / "Safety OK?"
        → YES (green down): continue
        → NO (red right): red box "⛔ STOP WORK" (hard stop, no loop)
Row 3: Box "ASSY-001" / "Site Assessment & Preparation"
Row 4: Box "ASSY-002" / "Foundation Setup"
Row 5: Diamond "QG-1" / "Foundation Level?"
        → YES (green down): exits container "→ STRUCTURE"
        → NO (red left): loops to Row 4 "Re-level"

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

Inside, stack vertically:

Row 1: Box "ASSY-003" / "Khana Wall Erection"
Row 2: Box "ASSY-004" / "Door Frame Installation"
Row 3: Box "ASSY-005" / "Uni Roof Poles Installation"
Row 4: Box "ASSY-006" / "Tono Crown Placement"
Row 5: Diamond "QG-2" / "Structure Stable?"
        → YES (green down): exits container "→ COVERING"
        → NO (red left): loops to Row 1 "Adjust"

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

Inside, stack vertically:

Row 1: Box "ASSY-007a" / "Insulation Installation"
Row 2: Diamond "QG-3a" / "Coverage OK?"
        → YES (green down): continue
        → NO (red left): loops to Row 1 "Fill Gaps"
Row 3: Box "ASSY-007b" / "Outer Cover Installation"
Row 4: Diamond "QG-3b" / "Sealed?"
        → YES (green down): continue
        → NO (red left): loops to Row 3 "Reseal"
Row 5: Box "ASSY-007c" / "Inner Liner Installation"
        → exits container "→ COMPLETION"

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

Inside:

Row 1: Box "ASSY-008" / "Final Touches & Customer Handover"
Row 2: Diamond "QG-4" / "Customer Accepts?"
        → YES (green right): box "→ CARE" (exit point)
        → NO (red down): box "Punch List" → loops back to Row 1

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

Stack these rows vertically:

Row 1: Box "CARE-001" / "Post-Assembly Follow-up (48h)"
Row 2: Box "CARE-002" / "Satisfaction Survey & Portfolio"
Row 3: Diamond "QG-1" / "NPS ≥ 8?"
        → YES (green down): continue
        → NO (red right): box "Escalate → CORE-002"
Row 4: Two boxes side by side:
        Left: "CARE-003a" / "Warranty Claims"
        Right: "CARE-003b" / "Service Complaints"
        Both connect down
Row 5: Box "CARE-004" / "Maintenance Guidance"
Row 6: Box "CARE-005" / "Referral Program"
Row 7: Diamond "QG-2" / "Referred?"
        → YES (green down): continue
        → NO (red left): loops to Row 6 "Follow up 30d"
Row 8: Box "CARE-006" / "Repeat & Upsell"
Row 9: Curved arrow pointing LEFT with label "→ SALES (Repeat Order)"

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
│ ┌─────────┐  = SOP Process              │
│ │ ID/Name │                             │
│ └─────────┘                             │
│                                         │
│    ◇       = Quality Gate (Decision)    │
│                                         │
│ ────────►  = YES / Pass (green)         │
│ - - - - ►  = NO / Fail (red dashed)     │
│    ↺       = Rework loop                │
│    ⛔      = Hard stop (safety)         │
│ ─ · ─ · ► = Cross-cutting (CORE)        │
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
