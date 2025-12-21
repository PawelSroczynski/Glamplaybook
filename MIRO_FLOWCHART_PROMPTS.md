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
Create a vertical flowchart for "CORE - Cross-Cutting SOPs"

Header: Dark gray (#4A4A4A), white text, label "CORE"

4 boxes stacked vertically, connected by arrows:
1. "CORE-001" / "Customer Communication Protocol"
2. "CORE-002" / "Issue & Exception Handling"
3. "CORE-003" / "Safety & PPE Standards"
4. "CORE-004" / "Documentation & Photo Capture"

Use gray color scheme (#4A4A4A header, #D9D9D9 boxes).
Make it narrow. Add dashed arrows pointing right from each box.
Footer label: "Applies to ALL phases →"
Subtitle: "4 SOPs"
```

---

## Prompt 2: SALES Column

```
Create a vertical flowchart for "SALES - Lead to Order"

Header: Yellow (#FFD966), label "SALES"

Flow top-to-bottom with decision diamonds (QG = Quality Gate):

Box: "SALES-001 Lead Capture"
↓
Box: "SALES-002 Lead Qualification"
↓
Diamond: "QG-1 Qualified?"
  → YES (green arrow down): continues
  → NO (red arrow right): "Archive/Nurture" gray box (dead end)
↓
Box: "SALES-003 Onboarding Media"
↓
Box: "SALES-004 Needs Assessment"
↓
Box: "SALES-005 Proposal"
↓
Diamond: "QG-2 Accepted?"
  → YES (green arrow down): continues
  → NO (red arrow left): loops back to SALES-005 "Revise"
↓
Box: "SALES-006 Agreement & Close"
↓
Box: "SALES-007 Contract"
↓
Box: "SALES-008 Payment"
↓
Diamond: "QG-3 Paid?"
  → YES (green arrow right): "→ PREP" (exit point)
  → NO (red arrow down): "Hold/Remind" (wait loop)

Yellow boxes (#FFD966), orange diamonds (#F6B26B).
YES arrows = green. NO arrows = red dashed.
Footer: "8 SOPs | 3 QGs"
```

---

## Prompt 3: PREP Column

```
Create a vertical flowchart for "PREP - Production Preparation"

Header: Blue (#9FC5E8), label "PREP"

Flow top-to-bottom with decision diamonds:

Box: "PREP-001 Order Intake"
↓
Diamond: "QG-1 Specs OK?"
  → YES: continues down
  → NO: red loop back to PREP-001 "Clarify"
↓
Box: "PREP-002 Materials Calculation"
↓
Box: "PREP-003 Supplier Ordering"
↓
Box: "PREP-004 Materials Receiving QC"
↓
Diamond: "QG-2 Materials OK?"
  → YES: continues down
  → NO: red arrow to "Reject & Reorder" box, loops to PREP-003
↓
Box: "PREP-005 Production Planning"
↓
Box: "PREP-006 Workshop Setup"
↓
Diamond: "QG-3 Ready?"
  → YES: "→ PROD" (exit point, green arrow right)
  → NO: red loop to "Resolve Blockers"

Blue boxes (#9FC5E8), orange diamonds (#F6B26B).
YES = green arrows. NO = red dashed arrows with loops.
Footer: "6 SOPs | 3 QGs"
```

---

## Prompt 4: PROD Column (Complex - 3 Streams)

```
Create a flowchart for "PRODUCTION" with 3 parallel streams that merge.

Header: Green (#93C47D), label "PRODUCTION"

THREE PARALLEL VERTICAL STREAMS side by side:

STREAM A "Wood" (left, light green #B6D7A8):
PROD-001 Wood Cut
↓
Diamond A1: YES→down, NO→"Recut" loop
↓
PROD-002 Wood Treatment
↓
PROD-003 Khana Assembly
↓
Diamond A2: YES→down, NO→"Repair" loop
↓
PROD-004 Uni Poles
↓
PROD-005 Tono Crown
↓
Diamond A3: YES→merge, NO→"Rebuild" loop

STREAM B "Sewing" (center, light blue #A4C2F4):
PROD-006 Canvas Cut
↓
Diamond B1: YES→down, NO→"Recut" loop
↓
PROD-007 Wall Cover
↓
Diamond B2: YES→down, NO→"Resew" loop
↓
PROD-008 Roof Cover
↓
PROD-009 Inner Liner
↓
Diamond B3: YES→merge, NO→"Repair" loop

STREAM C "Insulation" (right, light orange #F9CB9C):
PROD-010 Insulation Cut
↓
PROD-011 Insulation Assembly
↓
Diamond C1: YES→merge, NO→"Rework" loop

All three streams MERGE with arrows converging to:

Gray box containing 3 items in a row:
"PROD-012 Door/Window" | "PROD-013 Rope" | "PROD-014 Hardware"

↓

Diamond: "QG-4 Pre-Pack OK?"
  → YES: "→ LOG" (exit right, green)
  → NO: red arrows back to respective streams "Rework"

Footer: "14 SOPs | 8 QGs"
Small diamonds for in-stream QGs, larger diamond for QG-4.
```

---

## Prompt 5: LOG Column

```
Create a vertical flowchart for "LOGISTICS"

Header: Purple (#B4A7D6), label "LOG"

Flow top-to-bottom:

Box: "LOG-001 Component Packing"
↓
Diamond: "QG-1 Packed?"
  → YES: continues down
  → NO: red loop "Complete Packing"
↓
Box: "LOG-002 Loading & Securing"
↓
Box: "LOG-003 Transport & Delivery"
↓
Diamond: "QG-2 Delivered OK?"
  → YES: "→ ASSY" (exit right, green)
  → NO: red arrow to "Document Damage → CORE-002"

Purple boxes (#B4A7D6), orange diamonds.
Make it narrow. YES = green, NO = red.
Footer: "3 SOPs | 2 QGs"
```

---

## Prompt 6: ASSY Column (Complex - 4 Grouped Sections)

```
Create a flowchart for "ASSEMBLY" with 4 grouped sections stacked vertically.

Header: Red (#E06666), label "ASSEMBLY"

SECTION 1 - Light red box (#F4CCCC) labeled "PRE-ASSEMBLY":
ASSY-000 Safety Briefing
↓
Diamond: "QG-0 Safe?"
  → YES: continues
  → NO: "⛔ STOP WORK" red box (hard stop)
↓
ASSY-001 Site Assessment
↓
ASSY-002 Foundation Setup
↓
Diamond: "QG-1 Level?"
  → YES: continues to next section
  → NO: red loop "Re-level"

SECTION 2 - Medium red box (#EA9999) labeled "STRUCTURE":
ASSY-003 Khana Walls
↓
ASSY-004 Door Frame
↓
ASSY-005 Uni Poles
↓
ASSY-006 Tono Crown
↓
Diamond: "QG-2 Stable?"
  → YES: continues
  → NO: red loop "Adjust Structure"

SECTION 3 - Red box (#E06666) labeled "COVERING":
ASSY-007a Insulation Install
↓
Diamond: "QG-3a Coverage?"
  → YES: continues
  → NO: red loop "Fill Gaps"
↓
ASSY-007b Outer Cover
↓
Diamond: "QG-3b Sealed?"
  → YES: continues
  → NO: red loop "Reseal"
↓
ASSY-007c Inner Liner

SECTION 4 - Dark red box (#CC0000, white text) labeled "COMPLETION":
ASSY-008 Final Touches & Handover
↓
Diamond: "QG-4 Accepted?"
  → YES: "→ CARE" (exit right, green)
  → NO: "Punch List" → red loop back to rework

Footer: "11 SOPs | 6 QGs"
```

---

## Prompt 7: CARE Column

```
Create a vertical flowchart for "CARE - After-Sale"

Header: Teal (#76A5AF), label "CARE"

Flow top-to-bottom:

Box: "CARE-001 Follow-up (48h)"
↓
Box: "CARE-002 Survey & Portfolio"
↓
Diamond: "QG-1 NPS ≥ 8?"
  → YES: continues down
  → NO: red arrow to "Escalate → CORE-002"

Branch point - TWO BOXES SIDE BY SIDE:
"CARE-003a Warranty" | "CARE-003b Complaints"
(both connect down)
↓
Box: "CARE-004 Maintenance Guidance"
↓
Box: "CARE-005 Referral Program"
↓
Diamond: "QG-2 Referred?"
  → YES: continues
  → NO: red loop "Follow up 30 days"
↓
Box: "CARE-006 Repeat & Upsell"
↓
Curved arrow looping back left labeled "→ SALES (Repeat Order)"

Teal boxes (#76A5AF), orange diamonds.
Footer: "7 SOPs | 2 QGs"
```

---

## Manual Assembly Instructions

After creating all 7 flowcharts in Miro:

### Step 1: Arrange
Drag flowcharts side-by-side, left to right:
```
[CORE] [SALES] [PREP] [PROD] [LOG] [ASSY] [CARE]
```
Align all headers at the same vertical level.

### Step 2: Connect Phases
Draw arrows between columns at exit/entry points:
- SALES "→ PREP" connects to PREP-001
- PREP "→ PROD" connects to top of PROD streams
- PROD "→ LOG" connects to LOG-001
- LOG "→ ASSY" connects to ASSY-000
- ASSY "→ CARE" connects to CARE-001
- CARE "→ SALES" curved arrow to SALES-001

### Step 3: Add Title Frame
Above all columns:
```
ENKLAVA YURTS - SOP INFRASTRUCTURE v2.1
53 SOPs | 24 Quality Gates | Complete Client Flow
```

### Step 4: Add Legend
Bottom right corner:
```
┌─────────────────────────────────────┐
│ LEGEND                              │
│ ┌───┐ = SOP Process                 │
│  ◇  = Quality Gate (Decision)       │
│ ──► = YES / Pass (green)            │
│ --► = NO / Fail (red dashed)        │
│  ↺  = Rework loop                   │
│  ⛔ = Stop work                      │
│ ─·─ = Cross-cutting reference       │
└─────────────────────────────────────┘
```

### Step 5: Color Key
Add color reference:
```
CORE: Gray    | SALES: Yellow | PREP: Blue
PROD: Green   | LOG: Purple   | ASSY: Red   | CARE: Teal
```

---

## Tips for Miro AI

1. If a prompt is too complex, split it further (e.g., PROD into 3 separate stream prompts)
2. Use "make it narrower" or "make it more compact" if output is too wide
3. Say "use rounded rectangles for process boxes" for consistent styling
4. Say "diamonds should be smaller than boxes" for visual hierarchy
5. If colors aren't applied, specify "fill color" vs "border color"

---

*Created: December 2025*
*For: Enklava Yurts SOP Infrastructure v2.1*
