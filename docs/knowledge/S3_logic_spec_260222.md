# Supplemental 3 — Logic Specification v2.1 (Feb 22 2026)

**Source:** https://wiki.gi7b.org/index.php/Mneme_World_Generator/Logic_Specification_(Feb_22_2026)
**Last Synced:** 2026-03-04
**Note:** This is the canonical current specification for the v2.1 orbital placement system.

---

## 1. Anchor Formulas

| Formula | Expression |
|---------|-----------|
| Snow Line | D_snow = 2.7 × √L_Star |
| HZ Center | HZ_center = √L_Star |
| HZ Inner | 0.95 × HZ_center |
| HZ Outer | 1.37 × HZ_center |

---

## 2. Dominance Formulas (Hill Stability)

| Formula | Expression |
|---------|-----------|
| Hill Sphere Ratio | μ = ∛((m₁ + m₂) / (3 × M_Star)) |
| Mutual Hill Radius | R_H = a_avg × μ  where a_avg = (a₁ + a₂)/2 |
| Required Safety Space | W_req = K × R_H |

**K Values:**
| K | Standard |
|---|---------|
| K = 5 | Mneme Standard (Rule of Five) |
| K = 8 | Sol Standard / Relaxed System |
| K < 3.5 | Chaos Limit — Unstable |

---

## 3. The Shove

When two objects are too close (gap < W_req), the outer object is moved:

```
a_new_outer = a_inner + W_req + Variance
```

Where Variance = +0.01 to +0.1 AU (random)

**Ripple Effect:** If moving the outer object creates a new conflict with the next object out, repeat The Shove down the chain until no conflicts remain.

**Far Outer Exception:** Objects in the Scatter Disk (>100 AU) are never moved; the intruder is ejected instead.

---

## 4. Multi-Star Stability

| Formula | Expression |
|---------|-----------|
| Barycenter r₁ | D_total × M₂/(M₁+M₂) |
| Barycenter r₂ | D_total × M₁/(M₁+M₂) |
| Binary Forbidden Zone inner | D_total / 5 |
| Binary Forbidden Zone outer | D_total × 5 |
| S-Type orbit minimum | D_min = a_max_desired × 5 |
| P-Type orbit maximum | D_max = a_min_desired / 5 |
| Hierarchical (Alpha Cen model) | D_C ≥ (D_AB × 5) × Safety Factor |

---

## 5. Example Walkthrough: "The Shove"

**Scenario:**
- Gas Giant: 300 EM at 3.0 AU
- Ice Giant: 15 EM at 3.2 AU

**Calculation:**
- a_avg = (3.0 + 3.2) / 2 = 3.1 AU
- μ = ∛((300 + 15) / (3 × M_Star)) ≈ 0.068
- R_H = 3.1 × 0.068 ≈ 0.21 AU
- W_req = 5 × 0.21 = 1.05 AU
- Current gap: 3.2 - 3.0 = 0.2 AU → **conflict**
- New position: 3.0 + 1.05 + 0.05 (variance) = **4.10 AU**

Ice Giant moves from 3.2 AU to 4.10 AU.

---

## 6. Gravitational Queue Process (Full Steps)

1. Sort all objects by Mass (highest → lowest)
2. Place heaviest object first (Gas Giant at Snow Line)
3. Calculate its Forbidden Zone using Mutual Hill Radius
4. Each next object must sit at Δa > 5 × R_H from all existing objects
5. If conflict: Apply The Shove
6. Repeat Ripple Effect down the chain until stable
7. Far Outer Exception: Scatter Disk objects (>100 AU) are never moved; intruder ejected
