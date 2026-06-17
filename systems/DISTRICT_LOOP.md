# District Turn Loop (Player + System Interaction Model)

This document defines the runtime flow of a district during a single update cycle.  
It explains how player actions and system simulations interact over time.

---

## 1. Intelligence Phase (Information Snapshot)

The game presents the current known state of the district:

- Influence per organization
- Active conditions
- Visible Points of Interest (PoIs) and their states
- Slot pressure status
- Known assets and their effects

### Purpose
Establish what is currently known before decisions are made.

### Design Intent
Information may be partial or imperfect depending on intelligence systems.

---

## 2. Strategic Planning Phase (Player Decisions)

The player selects actions for the district, such as:

- Installing or removing assets in slots
- Assigning force presence or influence pressure (if applicable)
- Launching missions into the district
- Targeting PoIs for capture, corruption, or disruption
- Responding to active conditions

### Purpose
Define intent under constraints (slots, resources, available agents).

---

## 3. Execution Phase (Active Operations Resolve)

All player and AI-initiated actions begin resolution:

- Missions are resolved or progress
- PoI interactions advance (contest, capture, transformation)
- Force presence applies pressure effects
- Conflicts between organizations are processed

### Key Idea
Actions do not instantly change final state—they initiate outcomes.

---

## 4. System Resolution Phase (District Simulation Tick)

The district simulates autonomous system behavior:

- Assets execute continuous effects (income, influence shifts, heat, etc.)
- Conditions apply modifiers and evolve
- Slot pressure is applied (efficiency, instability, vulnerability)
- Passive PoI effects are applied (if not actively contested)

### Purpose
Ensure the district evolves independently of player input.

---

## 5. Influence Reconciliation Phase

All influence changes are consolidated:

- Asset-driven influence changes
- Mission outcomes
- PoI control shifts
- Condition-based modifiers

### Result
Updated influence distribution per organization.

### Control States
Influence determines control tiers (e.g. Presence → Controlled → Stronghold).

---

## 6. Event Resolution Phase

If conditions or thresholds are met, events are triggered:

- Emergent conditions (riots, crackdowns, festivals)
- PoI transformations or emergence
- External faction interventions
- New mission opportunities

### Purpose
Introduce instability and prevent static optimization.

---

## 7. State Update Phase (Loop Reset)

The updated district state is finalized:

- Influence map updated
- PoI states updated
- Conditions updated
- Slot pressure recalculated
- Visibility recalculated

The system then returns to Phase 1.

---

## Design Summary

This loop ensures districts are:

- Reactive to player decisions
- Autonomous in simulation
- Competitive between organizations
- Driven by contested points of control (PoIs)

Districts are not static containers—they are evolving strategic systems.
