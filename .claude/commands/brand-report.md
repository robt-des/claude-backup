Build a visual brand guideline on the "Brand Report" page of the Figma file.

## Before you start

1. Read `brief.md` in the current project directory to get the Figma file URL and brand name.
2. Connect to the Figma file via MCP. If access fails, stop and report clearly.
3. Do NOT regenerate tokens or modify any Figma variables — only build the report page.
4. If a "Brand Report" page does not exist in the Figma file, stop and tell the designer.

## How to build

Pull all current token values live from these Figma collections:
- `color_primitives` — for all colour swatches and hex values
- `font_primitives` — for typeface name and weight values
- `spacing` — for spacing scale values
- `border` — for radius and width values

Use actual Figma variable references when available rather than hard-coding resolved values. If a colour, text, spacing, or border value can be assigned as a live Figma variable binding, preserve that binding on the canvas.

Build one auto-layout frame (1280px wide, vertical, height auto) positioned at x:200 y:200 on the page. Name it "Brand Report — [Brand Name]". Background: neutral/0.

## Section structure

Build these sections in order. Each section fills the full 1280px width.

### Header
- Background: brand/primary/800
- Contents: pill badge ("DESIGN SYSTEM · BRAND TOKEN REFERENCE"), brand name (60px Bold), subtitle "Brand Token Reference Guide" (22px Regular), meta row with Typeface / Primary colour / Neutral / Mode / Date

### 01 — Colour Palette
- Background: #FFFFFF
- Brand Primary subsection: all steps (25–900) as a horizontal swatch row, each 104×80px. Mark step 500 with ★. Include hex value and step number under each swatch. Add a use-case note below the row.
- Neutral subsection: key steps (0, 100, 300, 500, 700, 900, 1000) as a swatch row, 164×72px each. Include hex, step, and a one-word descriptor. Add a use-case note.
- System colours subsection: Positive / Negative / Caution / Info as cards each showing light/mid/dark swatches. Add Sale and Focus as inline rows below.

### 02 — Typography
- Background: neutral/0
- Typeface specimen card: large "Aa" at 96px, full alphabet rows, family/classification/weights/tier metadata.
- Weights subsection: three cards (Regular / Medium / Bold) each showing the weight name, a pangram sentence in that weight, and the token name.
- Type scale note: explain that size tokens live in font_semantics.

### 03 — Spacing
- Background: #FFFFFF
- Visual bar chart: one column per token (0 through 4xl), bar height proportional to value (capped at 84px), name and px value labelled below.

### 04 — Border Radius
- Background: neutral/0
- Shared scale: one card per step (square through circular), each showing a rounded rectangle illustration sized to the radius value.
- Component aliases: one card per component (Button, Card, Input, Pill, Panel, Tag, Swatch) showing a small rectangle preview, the component name, the alias it points to, and a one-line use note.

### 05 — Border Width
- Background: #FFFFFF
- One card per width token (0, sm, md, lg, xl), each showing a vertical line at the correct thickness, the token name, the px value, and a use-case description.

### 06 — Use Case Guidance
- Background: neutral/0
- A table with columns: CATEGORY / TOKEN / VALUE / WHEN TO USE
- Dark header row using brand/primary/800
- Cover at minimum: 3 brand colour rows, 4 neutral rows, 4 system rows, 3 typography rows, 4 spacing rows, 3 radius rows, 2 border rows
- Alternate row backgrounds (#FFFFFF / #FAFAF9)

### Footer
- Background: brand/primary/800
- Left: brand name + "Brand Token Reference — [mode] mode — Generated [month year]"
- Right: agency contact email from the CLAUDE.md userEmail context

## Visual rules

- Use Inter for all report text (it is always available in Figma)
- Section number labels: 11px Semi Bold, colour brand/primary/400, letter-spacing 10%
- Section titles: 28px Bold, neutral/1000
- Subsection labels: 11px Semi Bold, neutral/400, letter-spacing 10%, ALL CAPS
- Body/description text: 14px Regular, neutral/500
- Token name labels: 11–12px Regular or Medium, neutral/400
- Hex value labels: 11px Regular, neutral/400
- Use-case note pills: background brand/primary/25, text brand/primary/600, 13px Regular
- All cards: 1px stroke neutral/100, 8px corner radius, white background
- Swatch corner radius: 0 (flush within card)

## On completion

Print a one-line confirmation: "Brand Report built on the Brand Report page — [N] sections, [brand name]."
