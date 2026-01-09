# Flight Computer (Hardware)

KiCad hardware design for a rocket flight computer.

## Status
- Owner: AlexanderSvarthaugen
- Scope: hardware only
- Current revision: RevB (in design)
- Legacy: RevA (reference / known issues)

## What’s in this repository
- KiCad schematic + PCB layout
- Parts/BOM tracking
- Datasheet source tracking
- Bring-up plan and test checklist
- Manufacturing export structure (exports committed only for releases)

## Folder structure
- `docs/` — overview, architecture, power tree, interfaces, bring-up, risks
- `hardware/kicad/` — KiCad source files (schematic/PCB/project)
- `hardware/bom/` — BOM exports + parts notes
- `hardware/datasheets/` — datasheet sources and optional stored PDFs
- `hardware/manufacturing/` — fabrication/assembly exports by revision
- `releases/` — frozen manufacturing packages tied to version tags

## Quick start
1. Read: `docs/00_overview.md`
2. Open KiCad project: `hardware/kicad/revB/`
3. Parts/datasheets: `hardware/datasheets/sources.csv`
4. Bring-up plan: `docs/05_bringup-plan.md`

## Rules
- KiCad source stays in `hardware/kicad/`.
- Don’t commit random gerbers/exports into the KiCad folder.
- Manufacturing exports go in `hardware/manufacturing/<rev>/`.
- “Frozen” release packages go in `releases/`.
- Update `hardware/datasheets/sources.csv` when a part/datasheet changes.
