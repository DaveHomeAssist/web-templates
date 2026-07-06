# Web Templates

An internal reference pack of self-contained HTML/CSS layout patterns, served from this repo's `main` branch at **[davehomeassist.github.io/web-templates](https://davehomeassist.github.io/web-templates/)**. Each page is a distinct, single-file layout — a different aesthetic, different demo content, no build step, no JS framework — meant to be copied and adapted as a starting point when a new dashboard/reference page is needed elsewhere in the estate. `index.html` is the gallery/catalog that links to every layout.

Despite the repo name, this is **not** a public, general-purpose template library — it's a design-reference tool used internally when deciding how a new project's UI should look and behave.

## What's here

| Path | What it is |
|---|---|
| `index.html` | Catalog/gallery of all layouts, with a live theme switcher and a "coming next" placeholder card |
| `prompt_engineering_ref.html` | **Filterable Reference Table** — searchable index of prompting patterns with category/cost/model filters. Dark monospace aesthetic |
| `live_event_gear_map.html` | **Field Guide** — department-sorted gear reference with signal-chain position and failure-mode notes. Warm amber editorial aesthetic |
| `home_automation_map.html` | **Capability Comparison Map** — head-to-head platform feature comparison with scored bar charts and a protocol sidebar. Steel-blue instrument aesthetic |
| `layout_decision_matrix.html` | **Decision Matrix** — weighted scoring across options/criteria with live-reweighting sliders and an auto-computed winner. Cream/ink editorial aesthetic |
| `layout_phase_roadmap.html` | **Timeline / Phase Roadmap** — expandable phase blocks with task detail, owner, effort, status filter, and progress bars. Forest-green geometric aesthetic |
| `layout_status_board.html` | **Kanban Status Board** — five-column status view with type/owner/priority filters. Concrete brutalist light aesthetic |
| `layout_directory_index.html` | **Profile Directory** — filterable card grid of people with a persistent detail panel. Warm purple luxury aesthetic |
| `layout_annotated_review.html` | **Annotated Review / Issue Register** — two linked views (filterable priority-ranked issue list + source text with numbered margin comments), a headline-metric block, and a copy-ready summary. Light editorial, fully self-contained (no CDN fonts) |
| `security/service-quote-template.html` | **Client Portal Intake** — editorial client-facing quote/proposal page built for a fictional event-security firm ("ShieldBox"), with scope toggles, billing selection, and a print-ready layout |
| `AGENTS.md` | Agent-facing project notes: stack, key decisions, session log |
| `assets/icons/favicon/` | Shared favicon set used by every page |
| `icons/`, `shield.png` | Loose reference/demo icon assets used by individual layouts |

## How it's used

Every layout is a standalone HTML file with the shared favicon set and a sticky demo-nav bar linking to the others. Most pages embed an "adapt this" comment block (see `layout_annotated_review.html`) describing which sections to find/replace for a new use case. There's no shared build tooling — a new layout is added by copying the closest existing file, swapping the palette in `:root`, and replacing the demo data.
