# **System Invariants (Core Simulation Rules)**

This document defines the non-negotiable structural rules of the game world. These invariants ensure consistency across missions, assets, intel, districts, institutions, and time.

# **1. Everything Exists as Stateful Entities**

All major systems are persistent entities with explicit states:

- Factions
- Missions
- Assets
- Districts
- Intel networks
- Institutions

**Invariant:**

No system is purely transient or stateless. Every meaningful action modifies persistent world state.

# **2. All Player Actions Flow Through Missions or State Modification**

Player interaction always resolves into:

- creating a mission (direct action or opportunity engagement)
- modifying assets
- conducting intel investigations
- influencing districts or institutions

**Invariant:**

The player never directly changes world outcomes without passing through a structured system (mission, asset, or intel).

# **3. Missions Are Temporal State Machines**

Missions always follow this structure:

Opportunity → Shell → Preparation → Active → Resolved

**Invariant:**

Missions cannot skip phases or resolve instantly once started. They are always multi-phase temporal entities.

# **4. Preparation and Execution Are Strictly Separated**

- Preparation = deterministic player configuration layer
- Execution = autonomous world simulation layer

**Invariant:**

Player control ends at mission start. Execution is fully simulation-driven.

# **5. Assets Are Stateful and Risk-Bearing**

Assets always exist in one of these states:

Idle → Deployed → Committed → Active → (Exposed / Damaged / Lost / Returned)

**Invariant:**

Assets are never free modifiers. Every use carries potential state change or risk.

# **6. Intel Is Interpretive, Not Deterministic**

Intel represents:

- partial knowledge
- inferred possibilities
- discovered relationships or opportunities

**Invariant:**

Intel never produces certainty or optimal solutions, only expanded possibility space.

# **7. Districts Are Dynamic State Containers**

Districts continuously evolve based on:

- missions
- asset activity
- institutional pressure
- faction influence

**Invariant:**

Districts are never static maps. They are always in a state of flux driven by system interactions.

# **8. Institutions Are Reactive Systems, Not Static Backdrops**

Institutions:

- observe signals
- interpret mission activity
- react via pressure, interference, or enforcement

**Invariant:**

Institutions are active participants in world simulation, not environmental flavor.

# **9. Time Advances All Systems**

Time progression:

- advances missions
- updates district states
- triggers institution reactions
- resolves delayed effects

**Invariant:**

The world is always moving forward; no system is frozen unless explicitly designed to be dormant.

# **10. All Systems Interact Through a Closed Loop**

Core loop:

Assets → enable actions

Intel → reveals possibilities

Missions → execute actions

Districts → absorb consequences

Institutions → react and interfere

Time → advances all states

**Invariant:**

No system exists in isolation; every system both consumes and produces state changes in at least one other system.

# **11. No System Produces Pure Advantage Without Tradeoffs**

All gains have at least one cost:

- exposure
- resource commitment
- opportunity cost
- risk escalation
- future instability

**Invariant:**

There are no purely positive actions; every advantage creates a future vulnerability or constraint.

# **Core Design Identity (Summary)**

The game is a closed-loop state simulation where player agency operates through structured systems (missions, assets, intel), and every action produces persistent world changes that propagate through districts, institutions, and factions over time.

If you want next step, the most valuable thing now is not more mechanics — it’s probably:

👉 identifying **UI-level complexity risks (what the player will struggle to understand or track)**

Because your system is now structurally solid enough that usability becomes the real bottleneck.
