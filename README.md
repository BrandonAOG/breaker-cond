# Breaker & Conductor Sizing Tool

A professional, NEC 2023-compliant calculator for electrical contractors, engineers, and field technicians to determine proper conductor sizing and equipment grounding conductor (EGC) requirements.

## Features

✨ **NEC 2023 Compliance**
- **240.4(B)** — Next standard breaker size ≤ 800A
- **240.4(C)** — Exact ampacity required > 800A
- **310.16** — Conductor ampacity tables (75°C copper & aluminum)
- **310.12** — Dwelling service/feeder 83% rule (100A–400A)
- **310.10(H)** — Parallel conductor validation (minimum 1/0 AWG)
- **310.15(C)(1)** — Derating factors for bundled conductors (3–40+ CCC)
- **250.122** — Equipment grounding conductor sizing

📊 **Dual Application Modes**
- **General (310.16)** — All standard circuits and services
- **Dwelling (310.12)** — 1 & 2 family dwelling services/feeders with 83% rule optimization

🔌 **Advanced Options**
- Copper & aluminum conductor selection
- Parallel conductor set sizing (1–10 sets)
- Current-carrying conductor (CCC) derating
- Real-time violation detection & code citations

🎨 **Modern UI**
- Dark & light theme toggle
- Responsive mobile design
- Animated grid background
- Color-coded result badges (OK / Warning / Error / Info)
- Inline code references with explanatory notes

## Quick Start

1. **Open in browser:** No installation needed — just open `index.html`
2. **Select parameters:** Breaker size, conductor material, application, parallel sets, and CCC count
3. **View results:** Conductor size, derated ampacity, EGC size, and code basis notes
4. **Toggle theme:** Use the light/dark mode button (top right)

## Usage Examples

### Example 1: Single 100A Dwelling Service (Copper)
- **Breaker:** 100 A
- **Material:** Copper
- **Application:** 1 & 2 Family Dwelling Svc/Feeder
- **Parallel Sets:** 1
- **CCC:** 1–3 (no derating)

**Result:** 3 AWG copper @ 100A per 310.12 (83% rule: 100A × 83% = 83A)

### Example 2: 200A General Circuit with Derating (Aluminum, 4 Parallel Sets)
- **Breaker:** 200 A
- **Material:** Aluminum / CU-clad AL
- **Application:** General (310.16 75°C)
- **Parallel Sets:** 4
- **CCC:** 4–6 conductors (80% derating)

**Result:** 1/0 AWG aluminum per set (50A min per set after 80% derate)

### Example 3: 600A Feeder (Copper, 2 Parallel Sets, High Bundle Count)
- **Breaker:** 600 A
- **Material:** Copper
- **Application:** General (310.16 75°C)
- **Parallel Sets:** 2
- **CCC:** 21–30 conductors (45% derating)

**Result:** 250 kcmil copper per set (derated from 255A base ampacity)

## NEC References

| Section | Topic |
|---------|-------|
| **240.4** | Protection of Conductors |
| **240.6** | Standard Ampere Ratings |
| **250.122** | Size of Equipment Grounding Conductors |
| **310.10(H)** | Paralleled Conductors |
| **310.12** | Dwelling Services & Feeders (83% rule) |
| **310.15(C)(1)** | Adjustment Factors (CCC derating) |
| **310.16** | Allowable Ampacities (75°C, 90°C, 110°C) |

## Data Tables Included

- **310.16 Copper (75°C):** 14 AWG through 2000 kcmil
- **310.16 Aluminum (75°C):** 12 AWG through 2000 kcmil
- **310.15(C)(1) Derating:** Factors for 3–40+ current-carrying conductors
- **250.122 EGC:** Minimum grounding conductor sizes 15A–6000A

## Validation & Error Handling

⚠️ **The tool detects and warns about:**
- **Parallel violations** — Conductors < 1/0 AWG cannot be paralleled (310.10(H))
- **Dwelling 310.12 violations** — Out-of-range breaker sizes (< 100A or > 400A)
- **Dwelling + parallel conflict** — 310.12 doesn't permit parallel sets
- **Table exceedance** — Required ampacity exceeds largest available conductor
- **Derating adequacy** — Post-derate ampacity insufficient for load

## Browser Support

Works on all modern browsers (Chrome, Firefox, Safari, Edge). Mobile-responsive down to 320px width.

## License

Public domain. Use freely for educational, commercial, or field applications.

## Disclaimer

**This tool is informational only.** Always consult the current NEC code book, local authority having jurisdiction (AHJ), and a licensed electrician for final design decisions. Electrical system design involves many factors beyond conductor sizing—consult qualified professionals before installation.

---

**Always On Generators**

NEC 2023 Edition
