# ASTS Valuation Model

Interactive valuation model for AST SpaceMobile (NASDAQ: ASTS) — MNO direct-to-device revenue only.

**▶ Live app:** https://jacob-dashboard.github.io/asts-valuation/

## What's here

| File | What it is |
|---|---|
| `asts_valuation_app.html` | Self-contained interactive app — sliders, charts, financing sim, underwriting notes. Open in any browser; no dependencies. |
| `ASTS_Valuation_Model.xlsx` | The same model as a fully formula-driven Excel workbook (also downloadable from inside the app). |
| `index.html` | Redirect so GitHub Pages serves the app at the root URL. |

## The framework

One steady-state year at a chosen scale, priced through three lenses that anchor on different P&L lines:

- **EV / Gross Profit × 11** — most generous; ignores everything below the gross line
- **EV / EBITDA × 16** — captures opex but blind to satellite replenishment
- **P/E × 28** — the only lens that pays for D&A, interest, and tax

Blended **50 / 35 / 15** (net / EBITDA / gross), deliberately leaning on the lens that sees the capex. An S-curve adoption assumption plus a discount rate separate the growth premium from the multiples (no double counting), and a dilution section models the four outstanding convertible series (~27.7M potential shares, +7%) plus future raises.

Key ranges: 45–248 satellites (248 = FCC-granted constellation, Apr 2026) · 100M–2B subscribers · $2.50–5.00 ARPU · 50–70% gross margin · 5–7 yr satellite life · $20–25M per satellite incl. launch.

Coverage milestones, margin guidance, balance-sheet figures, and convert terms are sourced from AST's own statements and filings — see the app's **Underwriting** tab for the full source list.

*Model assumptions are the owner's. Market data as of Jul 22, 2026. Not investment advice.*
