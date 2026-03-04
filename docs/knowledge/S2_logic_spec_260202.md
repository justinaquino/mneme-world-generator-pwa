# Supplemental 2 — Logic Specification v2.1 (Feb 02 2026)

**Source:** https://wiki.gi7b.org/index.php/Mneme_World_Generator/Logic_Specification_(Feb_02_2026)
**Last Synced:** 2026-03-04
**Note:** Earlier draft. See S3_logic_spec_260222.md for the current canonical version.

---

## Contents

Same four-level hierarchy as the Feb 22 spec. This earlier draft documents:

- Gravitational Waterfall / Mutual Hill Radius formula
- Rule of Five for companion stars
- The Shove / Ripple Effect chain reaction
- Crowd Status / Overflow Rule for terrestrial placement
- Gravitational Queue Process (full step-by-step)
- Doubling Power Scale (SOC as base-2 logarithm)
- Elite Ratio formula
- Effective SOC formula

---

## Civilisation Mechanics (from this draft)

### Doubling Power Scale

SOC retooled to a Base-2 logarithmic scale — every +1 SOC = 2× increase in Income, Wealth, and Resource Access.

| SOC | Meaning |
|-----|---------|
| 10–11 | "Billionaire" / Head of State |
| 14+ | Stellar Elite (owns Habitats / Megacorps) |

### Elite Ratio Formula

```
Elite Ratio = (1 / (Gini Score + 1)) × 10%
```

### Effective SOC

```
Effective SOC = Individual SOC + (World Average SOC - 7)
```

---

## Tech Divide Access Logic

| SOC Level | Tech Access |
|-----------|------------|
| High SOC (Elites) | Full access to Setting TL |
| Mid SOC (Citizens) | Access to Standard TL |
| Low SOC (Subsistence) | Restricted to Scavenged / Archaic Tech |

---

## Key Formulas (same as Feb 22 spec — see S3 for canonical)

- Snow Line: D_snow = 2.7 × √L_Star
- HZ: center = √L_Star; inner = 0.95×; outer = 1.37×
- Mutual Hill Radius: R_H = a_avg × ∛((m₁+m₂)/(3×M_Star))
- Required Safety Space: W_req = K × R_H (K=5 Mneme Standard)
