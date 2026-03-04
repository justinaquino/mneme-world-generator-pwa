# Mneme World Generator Wiki Sync

**Canonical Source:** https://wiki.gi7b.org/index.php/Mneme_World_Generator
**Last Synced:** 2026-03-04
**Status:** ✅ Initial sync complete

---

## Purpose

This file instructs developers and AI assistants to keep the project's knowledge base in sync with the live Mneme World Generator wiki. The wiki is the authoritative source for rules, tables, and generation procedures. Local markdown copies in `docs/knowledge/` are the in-repo reference for AI-assisted development.

**URL Pattern:** The wiki uses subpages — `Mneme_World_Generator/SubpageName` — not chapter-numbered URLs.

---

## Core Chapters

| Chapter | Title | Wiki URL | Local File | Status |
|---------|-------|----------|------------|--------|
| Index | Main Index | https://wiki.gi7b.org/index.php/Mneme_World_Generator | `docs/knowledge/00_index.md` | ✅ Synced 2026-03-04 |
| 0 | Front Matter & Credits | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Front_Matter | `docs/knowledge/00_front_matter.md` | ✅ Synced 2026-03-04 |
| 1 | Definitions | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Definitions | `docs/knowledge/01_definitions.md` | ✅ Synced 2026-03-04 |
| 2 | Minor Mechanics | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Minor_Mechanics | `docs/knowledge/02_minor_mechanics.md` | ✅ Synced 2026-03-04 |
| 3 | Overview | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Overview | `docs/knowledge/03_overview.md` | ⚠️ Minimal content on wiki |
| 4 | Determine Star | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Determine_Star | `docs/knowledge/04_determine_star.md` | ✅ Synced 2026-03-04 |
| 5 | Determine Main World | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Determine_Main_World | `docs/knowledge/05_determine_main_world.md` | ✅ Synced 2026-03-04 |
| 6 | Determine Habitability | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Determine_Habitability | `docs/knowledge/06_determine_habitability.md` | ✅ Synced 2026-03-04 |
| 7 | Determine Position | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Determine_Position | `docs/knowledge/07_determine_position.md` | ✅ Synced 2026-03-04 |
| 8 | Determine Inhabitants | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Determine_Inhabitants | `docs/knowledge/08_determine_inhabitants.md` | ✅ Synced 2026-03-04 |
| 9 | Determine Planetary System | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Determine_Planetary_System | `docs/knowledge/09_determine_planetary_system.md` | ✅ Synced 2026-03-04 |
| 10 | Appendix | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Appendix | `docs/knowledge/10_appendix.md` | ✅ Synced 2026-03-04 |
| 11 | OGL | https://wiki.gi7b.org/index.php/Mneme_World_Generator/OGL | `docs/knowledge/11_ogl.md` | ⚠️ Legal text only — not yet written |

---

## Supplemental Documents

| Document | Wiki URL | Local File | Status |
|----------|----------|------------|--------|
| Ships & Star Systems — Master Equation Sheet | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Ships_and_Star_Systems | `docs/knowledge/S1_ships_and_star_systems.md` | ✅ Synced 2026-03-04 |
| Logic Specification (Feb 02 2026) | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Logic_Specification_(Feb_02_2026) | `docs/knowledge/S2_logic_spec_260202.md` | ✅ Synced 2026-03-04 |
| Logic Specification (Feb 22 2026) — **canonical v2.1** | https://wiki.gi7b.org/index.php/Mneme_World_Generator/Logic_Specification_(Feb_22_2026) | `docs/knowledge/S3_logic_spec_260222.md` | ✅ Synced 2026-03-04 |

---

## Re-Sync Instructions

### When to Re-Sync

Check the wiki's Recent Changes page for updates since **Last Synced** date above:
- https://wiki.gi7b.org/index.php/Special:RecentChanges (filter by "Mneme_World_Generator")

### Manual Sync (Human)

1. Visit the wiki URL for the changed chapter
2. Copy content and update the corresponding `docs/knowledge/` file
3. Update **Last Synced** date at the top of this file
4. Update the **Status** column in the tables above
5. Add an entry to the Change Log below
6. Commit: `docs: sync wiki — [chapter] — [date]`

### AI-Assisted Sync

```
Please re-sync the Mneme World Generator wiki.

Check https://wiki.gi7b.org/index.php/Special:RecentChanges for pages
changed since [LAST SYNC DATE].

For each changed page:
1. Fetch the wiki URL using WebFetch
2. Update the corresponding docs/knowledge/ file
3. Update the sync status and Last Synced date in Mneme_World_Generator_Wiki_Sync.md
4. Add a change log entry

Wiki base URL: https://wiki.gi7b.org/index.php/Mneme_World_Generator
```

---

## For AI Assistants

**Always check this file first** before implementing generation logic. If a local file exists and is marked ✅, use it as the reference. If a chapter is marked ⚠️ or 🔄, note it in your implementation.

**Never implement generation rules from memory.** Always reference `docs/knowledge/` files.

**Key implementation files by feature:**

| Feature | File |
|---------|------|
| Star generation | `04_determine_star.md` |
| World type / size | `05_determine_main_world.md` |
| Habitability | `06_determine_habitability.md` |
| World position (AU) | `07_determine_position.md` |
| Inhabitants / PVS / Starport | `08_determine_inhabitants.md` |
| Planetary system | `09_determine_planetary_system.md` |
| Orbital mechanics v2.1 (canonical) | `S3_logic_spec_260222.md` |
| All definitions | `01_definitions.md` |
| Dice mechanics (Adv/Dis) | `02_minor_mechanics.md` |

---

## Change Log

### 2026-03-04 — Initial Sync

- First sync of all wiki chapters
- Chapters 0–10 + 3 supplemental documents fetched and written to `docs/knowledge/`
- **Chapter 3** (Overview) has minimal content on wiki — flagged ⚠️
- **Chapter 11** (OGL) contains legal text only — local file pending
- v2.1 changes (Logic Spec Feb 22 2026) noted as active draft — canonical implementation reference
- Wiki URL pattern confirmed: `Mneme_World_Generator/SubpageName` (not chapter-numbered)
