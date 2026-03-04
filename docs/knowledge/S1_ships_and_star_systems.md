# Supplemental 1 — Ships & Star Systems: Master Equation Sheet

**Source:** https://wiki.gi7b.org/index.php/Mneme_World_Generator/Ships_and_Star_Systems
**Last Synced:** 2026-03-04

---

A mathematics reference sheet for the Mneme World Generator and Mneme Ship Designer, organized into 16 sections.

---

## Core Orbital Mechanics Formulas

| Formula | Expression |
|---------|-----------|
| Vis-viva | v² = μ(2/r − 1/a) |
| Orbital period | P = 2π√(a³/μ) |
| Circular orbit | v_c = √(μ/r) |
| Escape speed | v_esc = √(2μ/r) |
| Hill radius | r_H = a_p × (m_p/(3M₊))^(1/3) |
| Sphere of Influence | r_SOI = a_p × (m_p/M₊)^(2/5) |
| Roche limit | r_Roche ≈ 2.44 R_p (ρ_p/ρ_s)^(1/3) |
| Hohmann transfer | a_t = (r₁+r₂)/2; Δv₁ = √(μ(2/r₁−1/a_t)) − √(μ/r₁) |
| Tsiolkovsky | Δv = Isp × g₀ × ln(m₀/m_f) |
| Equilibrium temperature | T_eq = ((1−A)L/(16πσr²))^(1/4) |
| Snow Line | D_snow = 2.7 × √L_Star |
| Habitable Zone center | HZ_center = √L_Star |
| HZ inner | HZ_inner = 0.95 × HZ_center |
| HZ outer | HZ_outer = 1.37 × HZ_center |

---

## Task Cards

| Card | Purpose |
|------|---------|
| T1 | Gravity minimum stable distance |
| T2 | Orbital velocities |
| T3 | Δv to intercept |
| T4 | Intercept methods bundle |
| T5 | Hohmann calculator |

---

## Ship Design Scaling Tiers

| Tier | Tonnage | Notes |
|------|---------|-------|
| Micro | <10t | — |
| Small | 10–100t | — |
| Medium | 100–1,000t | — |
| Large | 1,000–10,000t | — |
| Capital | >10,000t | — |

Each tier has: structural fraction, tankage fraction, radiator area, and hab volume rules.
