# **Missions**

Missions are the primary way organizations act on the world, but they are not simply selected actions. Instead, missions are **assembled operations** that emerge from the interaction of districts, Points of Interest (PoIs), assets, intel discoveries, and ongoing faction activity.

A mission begins when the player identifies or constructs an opportunity, such as a vulnerable treasury, a contested PoI, a rival operation, or a discovered weakness. Intel can reshape this opportunity by revealing alternative interpretations of the situation, turning a simple objective into multiple possible operations with different risks and rewards.

For example, a “raid the treasury” opportunity might instead become:

- a direct robbery
- an embezzlement scheme via a corrupt official
- a blackmail operation targeting the treasurer
- a framing operation that shifts blame to a rival faction

The mission system is therefore not just execution — it is **choice generation from discovered context**.

Once a mission is defined, the player assembles it by committing resources such as lieutenants, crew, wealth, leverage assets, and infrastructure assets deployed in relevant districts. These resources are not generic modifiers; they are **capability sources that define what solutions are possible**. For example, a smuggling route may enable extraction paths that would otherwise not exist, while a safehouse may enable stealth staging or escape routes.

The player then chooses a **mission approach** (such as Force, Intrigue, or Commerce), which defines how their capabilities are applied. Approaches do not increase power directly — they determine how effectiveness is distributed across different mission outcomes.

# Mission Axes

Every mission is evaluated across multiple **mission axes**, which represent different dimensions of how the operation unfolds. Common axes include:

- Secrecy (was the mission exposed?)
- Escape (were operatives able to extract safely?)
- Elimination (was the target fully neutralized?)
- Control (was the objective held or secured?)
- Influence (what political or social effect was created?)

Axes are not “secondary stats” — they are **independent outcome dimensions**. A mission can succeed in its primary goal while partially failing or succeeding across different axes, producing distinct consequences.

For example:

- A successful assassination (Elimination success)
- but exposed operation (Secrecy failure)
- with a clean escape (Escape success)

This might result in:

- target eliminated
- increased heat in the district
- retaliation from rival factions
- long-term instability in local influence networks

Axes therefore define how the world changes, not just how well the mission went.

# Mission Approaches

Mission approaches define **how a mission is executed and how capabilities are distributed across axes**.

After assembling resources, the player selects an approach such as:

- **Force** → favors Elimination and Control, risks Secrecy and Escape
- **Intrigue** → favors Secrecy, Influence, and manipulation, weaker direct impact
- **Commerce** → favors Wealth generation, access, and long-term positioning

Approaches do not add power; they **reallocate effectiveness between axes**, shaping tradeoffs.

For example, the same “eliminate a rival leader” mission:

- Force approach: high chance of elimination, high exposure risk
- Intrigue approach: slower setup, but lower exposure and potential for political framing
- Commerce approach: may convert the situation into bribery, buyouts, or negotiated removal instead of violence

# Assets in Missions

Assets are not passive modifiers — they are **capability sources that define what mission options exist**.

During mission assembly, assets can be committed to:

- enable entirely new approaches (e.g. infiltration via smuggling route)
- solve constraints (escape routes, access, concealment)
- enhance specific axes (Secrecy, Escape, Influence, etc.)
- create alternative mission structures (blackmail instead of assassination)

Assets are often the difference between:

“How do I increase success?”

and

“What kind of mission is even possible here?”

However, committing assets creates risk: they may become exposed, occupied, damaged, or targeted by rivals.

# Mission Resolution

Once a mission is assembled and executed, it enters a resolution phase where uncertainty and opposition matter.

If the mission is discovered, other factions may intervene. However, discovery is partial and depends on intel quality — factions rarely have perfect information about:

- mission objective
- involved assets
- force strength
- timing or intent

When interference occurs, factions enter a **simultaneous escalation phase**, where they must secretly choose:

- commit reserves
- hold position
- withdraw

Because decisions are simultaneous and information is incomplete, missions become a system of:

- bluffing
- commitment
- risk prediction
- reserve management

After escalation, final strength across all sides is calculated, and the mission resolves into a **graded outcome across all axes**, producing consequences rather than binary success/failure.

# Mission Outcome Philosophy

Missions are not evaluated as success/failure, but as **world changes shaped by multiple interacting outcomes**.

A mission is considered successful if its primary objective is achieved, but the *shape of that success* depends on axis performance and interference.

This ensures that:

- success can still create problems
- failure can still generate opportunities
- partial outcomes are the norm, not the exception

# Core Mission Loop

The full loop is:

1. **Opportunity emerges or is discovered**
- from districts, PoIs, assets, events, intel, or schemes
2. **Intel reshapes interpretation**
- reveals alternative objectives, stakeholders, or approaches
3. **Player assembles mission**
- commits assets, crew, resources, and leverage
4. **Player chooses approach**
- defines how capabilities map to mission axes
5. **Execution + potential discovery**
- other factions may partially or fully detect the mission
6. **Interference + escalation (if applicable)**
- simultaneous decisions with imperfect information
7. **Resolution across axes**
- determines outcomes and world changes
8. **New opportunities and consequences emerge**
- feeding back into districts, assets, intel, and future missions

# Mission Lifecycle & State Model (Execution Layer)

Missions are not resolved immediately after being started. Instead, once a mission is committed, it becomes an **active world entity** that persists over time and can evolve before final resolution.

## 1. Mission Shell (Pre-Execution State)

A mission begins as a shell when a player selects either:

- a UI action (player-initiated intent), or
- a world opportunity (system-generated situation)

At this stage, the mission is not yet active in the world. It exists in a **preparation phase**, where the player:

- assembles required resources (lieutenants, crew, assets, leverage)
- selects a mission approach
- optionally incorporates intel discoveries
- can still cancel without consequence

This phase defines what the mission *will become*.

## 2. Commitment (Start of Execution)

Once the player confirms the mission:

- the mission becomes **locked**
- committed assets and resources are tied to it
- the mission enters the world as an active entity

From this point onward, the mission is no longer hypothetical — it is a **live operation** in progress.

## 3. Active Mission State (World Entity)

During execution, the mission exists as a persistent world object.

This allows:

- rival factions to detect or partially discover the operation
- interference or escalation to occur mid-process
- complications, delays, or branching outcomes to emerge
- evolving conditions based on district state and faction actions

Missions are therefore not instantaneous resolutions, but **ongoing situations in the world simulation**.

## 4. Temporal Resolution Model (Open Design)

A key unresolved design choice is how mission time progression works.

Currently, missions may:

- last a fixed number of turns
- progress through internal phases over time
- resolve based on triggered conditions (completion, discovery, interference, etc.)

This remains an open question and will define:

- pacing of gameplay
- strategic timing decisions
- how pressure and escalation develop over time

## 5. Final Resolution

At the end of the mission lifecycle:

- outcomes are calculated across mission axes
- interference and escalation outcomes are applied
- world state is updated (districts, assets, influence, exposure, relationships)
- new opportunities and consequences are generated

## Open Questions (Design Pending)

- Do missions progress on a fixed turn timer, or variable event-driven timing?
- Can missions branch or change objectives mid-execution, or only outcomes?
- Are there intermediate resolution checkpoints, or only a final resolution?
- How granular is escalation during the active mission state?

# Mission Axes (Type-Defined Outcome Dimensions)

Mission axes are not universal metrics applied to every operation. Instead, each mission type defines which outcome dimensions are relevant, and only those axes are evaluated during resolution.

This means axes function as **contextual evaluation dimensions**, not fixed global statistics. The meaning of success or failure is therefore shaped by the nature of the mission itself.

## Core Principle

Each mission type defines:

- which axes exist for that mission
- which outcomes matter
- which forms of success or failure are possible

Axes are therefore part of the **mission definition layer**, not a separate scoring system.

## System Implications

**1. Missions define their own evaluation space**

Axes are not universal rules — they are derived from mission type. This ensures each mission represents a distinct problem space with its own success logic.

**2. Approaches operate within relevant axes only**

Mission approaches (Force, Intrigue, Commerce, etc.) redistribute effectiveness only across axes that exist for that mission type.

**3. Assets are context-dependent tools**

Assets are valuable because they enable or influence specific mission types. Their usefulness depends on which axes are active in a given operation.

**4. Intel can redefine mission framing**

Intel may reveal that a mission is not what it initially appears to be, effectively changing:

- mission type
- relevant axes
- viable approaches

**Summary of what is missing (compressed)**

Only 4 real mechanical ambiguities remain:

1. **Execution timing model** (turn-based vs event-driven vs hybrid)
2. **Interference trigger logic hierarchy** (what actually causes detection/action)
3. **Asset state transitions during execution** (loss, exposure, degradation rules)
4. **Definition of mission failure state** (objective vs axes vs composite)
5. *(optional but important)* **scope of mid-mission branching**

# **Mission Awareness & Visibility**

Missions do not have a binary “detected / not detected” state. Instead, they exist as **world activities that emit signals**, which may or may not be interpreted by other factions depending on their intelligence and context awareness.

Visibility is therefore not a single value, but an emergent result of **signals, environment, and interpretation capacity**.

## Core Principle

Missions are not detected directly — they are reconstructed by factions from partial information.

Different factions may have different levels of awareness, and may reach different conclusions about the same mission.

## Mission Signal Profile (Intrinsic Layer)

Every mission produces a level of “signal” in the world based on:

- scale and complexity of the operation
- duration of execution
- notoriety of the objective
- inherent stealthiness of the chosen approach
- number and type of committed assets

This defines how “loud” the mission is in the world.

## Environmental Exposure (District Layer)

The district where a mission takes place affects how easily signals can be observed or contextualized:

- surveillance intensity and institutional presence
- local instability or attention level
- density of actors and observers
- relevance of the district to competing factions

The same mission may be highly visible in one district and barely noticeable in another.

## Intelligence Coverage (Observer Layer)

Each observing faction interprets signals based on its intelligence network, including:

- knowledge of the district
- knowledge of the player faction
- knowledge of relevant institutions (police, corporations, etc.)
- ongoing investigations or surveillance operations

This determines how accurately signals can be interpreted.

## Operational Exposure (Execution Layer)

During execution, missions generate additional exposure based on:

- committed assets and their footprint
- personnel activity in the field
- infrastructure usage (safehouses, routes, contacts)
- timing and coordination patterns
- mistakes, leaks, or interference

This layer represents how much actionable information exists for others to observe.

## Awareness States (Emergent Outcome)

Based on the interaction of these layers, factions may reach different levels of awareness:

- **Unaware** → no meaningful interpretation of activity
- **Suspicious** → partial signals suggest something is happening
- **Informed** → mission type or target is partially inferred
- **Aware** → mission is identified and can be acted upon

Different factions may exist in different states simultaneously.

## Design Outcome

This system ensures that:

- detection is asymmetrical across factions
- missions can be misinterpreted or only partially understood
- districts meaningfully affect stealth and exposure
- intelligence is about interpretation, not raw detection
- interference emerges naturally from partial awareness
