# Plots & Schemes

## Purpose

Plots represent long-term ambitions pursued by organizations, powerful agents, or factions.

They provide strategic direction, create faction identity, generate emergent narratives, and act as major drivers of world change.

Plots answer the question:

> "What is this faction ultimately trying to achieve?"

---

## Core Concept

Plots are long-term objectives composed of multiple stages.

Progress is achieved through missions, assets, world state manipulation, diplomacy, and other systems.

Plots are not merely victory conditions—they actively generate gameplay by unlocking opportunities, creating conflicts, and reshaping the city.

---

## Hierarchy

Organization
→ pursues Plots
→ through Schemes
→ executed via Missions
→ using Assets, Crews, Intel, Debts, etc.

### Layer Definitions

- **Plot**: Long-term ambition.
- **Scheme**: Intermediate strategic project contributing to a Plot.
- **Mission**: Atomic operation executed by the player.

Example:

Plot:
- Control the High Spire

Schemes:
- Corrupt local officials
- Remove rival influence
- Secure economic dominance

Missions:
- Bribe magistrate
- Assassinate rival lieutenant
- Smuggle contraband

---

## Plot Structure

Plots consist of stages rather than simple progress bars.

Each stage may have:

- Requirements
- Consequences
- Unlocked missions
- World changes
- New counterplay opportunities

Progression should feel like advancing an agenda rather than filling a meter.

Internally, stages may be implemented as clocks if desired.

---

## Progress Sources

Plot progress can be achieved through multiple systems:

### Missions
Complete specific operations.

### Assets
Acquire or control key leverage.

### World State
Alter districts, corruption, faith, unrest, etc.

### Diplomacy / Debts
Create alliances or leverage over factions.

### Sacrifices
Commit or permanently lose valuable resources.

---

## Visibility & Discovery

Plots may be:

- Hidden
- Suspected
- Identified
- Fully Understood

Visibility depends on Intel quality and investigation.

This creates strategic espionage and uncertainty.

Players may discover:

- That a Plot exists
- Its current stage
- Its final objective
- Weak points to exploit

---

## Counterplay

Plots should be contestable.

Rival factions may:

- Interfere with missions
- Launch counter-schemes
- Sabotage progress
- Reverse world changes
- Exploit exposed stages

Plots create indirect conflict without requiring direct warfare.

---

## Plot Types

Plot types primarily provide flavor and content direction.

Examples:

- Domination
- Corruption
- Liberation
- Revelation
- Ascension

Avoid attaching unique mechanics to each type to prevent feature bloat.

---

## Design Principles

- Plots create faction identity.
- Plots generate gameplay, not just victory.
- Every stage should alter the world.
- Plots should create interaction and counterplay.
- Progress should emerge from existing systems.
- The city remembers.

---

## Tradeoffs

Players must choose:

- Which Plot to pursue.
- Whether to reveal or conceal ambitions.
- Which resources to commit long-term.
- Whether to advance quickly or remain hidden.
- When to sacrifice flexibility for power.

Pursuing one Plot often means neglecting others.

---

## Recommendations

### Add
- Plots as a new top-level system.

### Keep
- Missions as the primary gameplay loop.

### Reframe
- Schemes as mid-level strategic projects.

### Avoid
- Pure progress bars.
- New resource systems ("Means") if existing capabilities suffice.
- Multiple overlapping action layers with unclear distinctions.

---

## Open Questions

- How many Plots can a faction pursue simultaneously?
- Are Plots faction-specific or dynamically generated?
- Can multiple factions pursue the same Plot?
- Can Plots fail permanently?
- What determines victory conditions?
- How visible should late-stage Plots become?
- Can players steal or hijack another faction's Plot?
