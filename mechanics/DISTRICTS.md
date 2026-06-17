# Districts

## Purpose

Districts are the spatial layer of the game.

They answer two questions:

- Where does gameplay happen?
- Who holds power there?

Districts are not owned provinces. They are evolving opportunity spaces where organizations compete for influence.

---

## Design Goals

- Create strategic decisions about expansion and investment.
- Provide context for missions and assets.
- Support political competition rather than territorial conquest.
- Remain lightweight and avoid city simulation.

---

## Core Structure

A district contains:

```text
District
- Type
- Tags
- Influence (per organization)
- Slots
- Point of Interests (PoI)
- Conditions
```

---

## Type

Defines the district's identity.

Examples:

- Docks
- Noble Quarter
- Slums
- Market
- Temple District
- Industrial Zone

---

## Tags

Tags describe district characteristics.

Examples:

- wealthy
- poor
- corrupt
- religious
- industrial
- isolated
- crowded
- violent
- coastal

Tags are intentionally lightweight and reusable.

They feed multiple systems:

- Mission generation
- Asset bonuses
- Organization traits
- Scheme interactions
- Event generation

---

## Points of Interest (PoIs)

Points of Interest are **strategic locations or institutions inside a district that modify how the district behaves and is contested**.

They represent concentrated sources of leverage, conflict, or opportunity.

### Key Properties

- PoIs are **pre-existing or emergent**, not player-built structures.
- They are **rare and meaningful**, not granular or decorative.
- They act as **rule modifiers and strategic targets**.

---

### What PoIs do

A PoI can:

#### 1. Modify district rules
Example:
- A Black Market increases income from illegal activity but raises heat generation.

#### 2. Enable or unlock mechanics
Example:
- A Cathedral enables influence-based religious operations.

#### 3. Create strategic targets
PoIs can be:
- infiltrated
- corrupted
- controlled
- destroyed or transformed

#### 4. Generate unique mission opportunities
PoIs are often the source of high-value missions.

---

### Types of PoIs

PoIs can appear as:

#### Fixed PoIs
- Existing locations (docks, markets, temples, casinos)

#### Emergent PoIs
- Created through events, missions, or conditions

#### Transformed PoIs
- Existing PoIs that change state over time (e.g. casino → money laundering hub)

---

### Key Rule

PoIs are **not buildings constructed by the player**.

They are **objects of control and transformation**.

---

### Design Intent

PoIs create **localized power centers that shape district identity and conflict**.

---

## Influence

Influence is the core territorial currency.

Each organization may hold influence in a district.

Example:

```text
Player: 45
Church: 30
Rival Family: 25
```

---

## Slots

## Slots

Slots represent the **structural capacity of a district to host systems**.

They do not define *what* must be placed there, only **how much can be active at the same time**.

Slots are intentionally generic.

### Purpose of Slots

- Limit simultaneous systems operating in a district.
- Force strategic tradeoffs between different forms of power.
- Prevent full optimization of all systems in a single district.
- Create vulnerability through overextension.

### What can occupy slots

Slots may be used by:

- Assets (persistent systems such as smuggling networks or propaganda cells)
- District-level force presence (e.g. enforcement groups, garrisons, agent presence)
- Other long-term district systems (future expansions)

### Key Rule

Slots are **not typed**.

A slot does not inherently belong to economy, influence, or combat.

Instead, systems impose their own requirements and effects once installed.

### Design Intent

Slots are a **pressure mechanism**, not a categorization system.

---

## Conditions

Conditions represent temporary district states.

Examples:

- Riots
- Festivals
- Plague

---
## District Runtime Model

Districts operate in a continuous resolution cycle during gameplay.

This cycle defines how assets, influence, and conditions interact over time.

---

### 1. State Read

At the start of a cycle, the district reads:

- Influence per organization
- Active assets
- Active conditions
- Slot usage
- PoI ownership states

---

### 2. Asset Resolution

Assets execute their continuous effects.

Examples:
- Generate income
- Modify influence
- Increase or decrease heat
- Alter district conditions

---

### 3. Condition Resolution

Conditions apply temporary or persistent modifiers to the district.

Examples:
- Riots reduce stability and disrupt assets
- Festivals increase influence generation opportunities
- Gang wars increase volatility and mission availability

---

### 4. Influence Update

Influence values are adjusted based on:

- Asset output
- Mission outcomes
- Condition effects
- PoI control

This determines relative control states in the district.

---

### 5. Slot Effects Application

Slots determine **how many systems can be active**, not what they are.

Overcapacity or contested slots may introduce:
- reduced efficiency
- instability
- vulnerability to enemy actions

---

### 6. Event Trigger Check

If thresholds are met, the district may generate events:

- Power shifts
- Outbreaks of violence
- Political interventions
- Opportunistic mission generation

---

### Design Intent

The runtime model ensures districts are **dynamic systems where multiple forces continuously interact**, rather than static containers of bonuses.

---

### Design Intent

The runtime model ensures districts function as dynamic, evolving systems where multiple forces continuously interact rather than static containers of bonuses or resources.

---

## Delegated Systems

| Mechanic | Owner |
|----------|-------|
| Income | Assets |
| Missions | Missions |
| Fear | Schemes |
| Corruption | Schemes |
| Heat | Organizations |
| Stability | Conditions |

---

## Core Insight

Districts are contested spaces of evolving power, not static territory.

## Open Questions
[QUESTION] What exactly is Force Presence: a subtype of assets, a separate system, or a district-level modifier layer?
[QUESTION] What are the exact rules for slot occupancy (single system per slot vs stacking vs partial occupancy)?
[QUESTION] How are Points of Interest captured, contested, and transferred between organizations?
[QUESTION] How does influence translate into actual control states beyond threshold labels?
[QUESTION] Can Conditions modify structural systems such as slots, assets, or PoIs, or are they strictly modifiers?
[QUESTION] What is the strict separation boundary between Assets and Conditions in terms of allowed effects?
[QUESTION] What is the exact origin logic of Events (threshold-based, PoI-driven, condition-driven, random, or hybrid)?
[QUESTION] What is the temporal structure of the runtime model (turn-based, tick-based, or real-time simulation)?
[QUESTION] What is the intended scale of districts (number of districts and gameplay granularity per district)?
[QUESTION] What information is visible to the player regarding enemy influence, PoIs, assets, and internal district state?

## TODO
[] Define Force Presence as a formal system (ownership, effects, and interaction rules)
[] Define Slot occupancy rules (capacity model, stacking rules, and constraints)
[] Define PoI capture/contest/transfer mechanics
[] Define Influence-to-Control conversion as a mechanical system (not only thresholds)
[] Define Conditions interaction boundaries with Assets, Slots, and PoIs
[] Define strict separation rules between Assets and Conditions
[] Define Event generation system (sources, triggers, and resolution rules)
[] Define Runtime temporal model (tick definition and resolution ordering)
[] Define District scale and density model (number of districts and abstraction level)
[] Define Information/visibility rules for districts and their systems
