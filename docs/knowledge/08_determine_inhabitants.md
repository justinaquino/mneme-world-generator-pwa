# Chapter 8 — Determine Inhabitants

**Source:** https://wiki.gi7b.org/index.php/Mneme_World_Generator/Determine_Inhabitants
**Last Synced:** 2026-03-04

---

## Four Scalable Qualities

1. Technology Level
2. Development
3. Source of Power
4. Power Structure

---

## Population

**Formula:** Bp = 10^Hab

Roll 2D6 × base population for actual population.

> Example: Hab 8 → base 100M; roll 6 → 600M population

**Habitats:** Base Pop = Max Capacity ÷ 12 (minimum 1)

---

## Wealth (2D6)

| Roll | Wealth | SOC Modifier |
|------|--------|-------------|
| 2–8 | Average | +0 |
| 9–10 | Better-off | +1 |
| 11 | Prosperous | +2 |
| 12 | Affluent | +3 |

**Abundance modifiers:**
- Abundant resources: Adv+1
- Inexhaustible resources: Adv+2

---

## Power Structure (2D6)

| Roll | Power Structure | Mechanical Effect |
|------|----------------|-------------------|
| ≤7 | Anarchy | Attitudes vary by faction |
| 8–9 | Confederation | Attitude severity reduced (Hostile→Unfriendly, Helpful→Friendly) |
| 10–11 | Federation | Deal with federal/national government |
| ≥12 | Unitary State | Bureaucratic delays |

---

## Development Levels (2D6)

| Roll | Development | HDI Range | Avg SOC |
|------|------------|-----------|---------|
| 2 | Underdeveloped | 0.0–0.39 | 2 |
| 3–5 | Underdeveloped | 0.40–0.59 | 3–4 |
| 6–7 | Underdeveloped | 0.50–0.59 | 4 |
| 8 | Developing | 0.60–0.69 | 5 |
| 9 | Mature | 0.70–0.79 | 6 |
| 10 | Developed | 0.80–0.89 | 8 |
| 11 | Well Developed | 0.9–0.94 | 9 |
| 12 | Very Developed | >0.95 | 10 |

### Development Mechanical Effects

| Development | Trade Penalty | Broker Fee | Port Fees | PVS Modifier |
|-------------|--------------|------------|-----------|-------------|
| Underdeveloped | DM-2 Advocate/Admin; +2 trade difficulty | 4× commission | — | — |
| Developing | DM-1 Advocate/Admin; +1 trade difficulty | 2× commission | — | — |
| Mature | No penalty | ×2 | 200Cr/day (first 6 free) | — |
| Developed | Adv+1 Governance; distant >5 parsecs ×2 rolls | ×5 | 500Cr | +1 PVS |
| Well Developed | Adv+2 Governance | ×10 | 1,000Cr | +2 PVS |
| Very Developed | Adv+3 Governance | ×20 | 2,000Cr | +3 PVS |

### Calamities

| Type | Effect |
|------|--------|
| Major | Reduces development one level (wars, economic collapse, environmental disasters) |
| Severe | Reduces development >1 level |
| Serious | Setbacks lasting years, not decades |

---

## Governance (2D6 + modifiers)

**Development DM:**

| Development | DM |
|-------------|-----|
| Underdeveloped | -9 |
| Developing | -8 |
| Mature | -7 |
| Developed | -6 |
| Well Developed | -5 |
| Very Developed | -4 |

**Wealth DM:** Better-off +1, Prosperous +2, Affluent +3

---

## Source of Power (2D6)

| Roll | Source of Power |
|------|----------------|
| 2–5 | Aristocracy |
| 6–7 | Ideocracy |
| 8–9 | Kratocracy |
| 10–11 | Democracy |
| 12 | Meritocracy |

Other power systems: Plutocracy, Stratocracy, Theocracy, Netocracy, Particracy, Timocracy, Technocracy, Kritarchy, Ergocracy.

---

## Travel Zones

### Amber Zone
Auto-assigned for: high biohazard, high radiation
Otherwise: roll 2D6 → result of 2 = Amber

**Amber Reasons (2D6):**
War, Plague, Insurgency, Heightened Security, Political Purging, Economic Crisis, Political Issue, Environmental Disaster, Major Social Issue, Engineering Disaster, Economic Collapse.

### Red Zone
Interdicted — travel forbidden. Referee discretion.

---

## Port Value Score (PVS)

**Formula:**
```
PVS = (Habitability / 4) + (TL - 7) + Wealth Modifier + Development Modifier
```

| PVS | Starport Class | Notes |
|-----|---------------|-------|
| <4 | X | Unprepared; damage risk (1d3 or 1d6) |
| 4–5 | E | Prepared area; damage risk |
| 6–7 | D | Specialized; damage on fail 6+; Scout Base roll 8+ |
| 8–9 | C | Scout Base roll 8+ on 2D6-1 |
| 10–11 | B | Naval Base 8+; Pirate 12+; Scout 8+ on 2D6-2 |
| +12 | A | Naval Base 8+; Pirate 12+; Scout 8+ on 2D6-3 |

### Starport Weekly Output by PVS

| PVS | Weekly Output |
|-----|-------------|
| 1 | 10 Cr |
| 2 | 100 Cr |
| 3 | 1,000 Cr |
| 4 | 10,000 Cr |
| 5 | 100,000 Cr |
| 6 | 1,000,000 Cr |
| 7 | 10,000,000 Cr |
| 8 | 100,000,000 Cr |
| 9 | 1,000,000,000 Cr |
| 10 | 10,000,000,000 Cr |

### Fuel Prices

| Fuel | Price |
|------|-------|
| Refined | 500 Cr/DTON (+ 100 Cr if shipped = 600 Cr) |
| Unrefined | 100 Cr (or 200 Cr if shipped) |
