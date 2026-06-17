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

Points of Interest are strategic locations or institutions inside a district that modify how the district behaves and is contested.

They represent concentrated sources of leverage, conflict, or opportunity.

### Key Properties

- PoIs are pre-existing or emergent, not player-built structures.
- They are rare and meaningful, not decorative.
- They act as rule modifiers and strategic targets.

### What PoIs do

PoIs can:

1. Modify district rules
2. Unlock mechanics
3. Create strategic targets
4. Generate mission opportunities

### Types of PoIs

- Fixed PoIs
- Emergent PoIs
- Transformed PoIs

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

Slots represent district capacity.

They limit how many systems can be active at the same time.

Slots are not typed.

They enforce tradeoffs and prevent overextension.

Slots may host:

- Assets
- Force presence
- Other long-term systems

---

## Conditions

Conditions represent temporary district states.

Examples:

- Riots
- Festivals
- Plague

---

## Runtime Model

### 1. State Read
- Influence
- Assets
- Conditions
- Slots
- PoIs

### 2. Asset Resolution
Assets generate continuous effects.

### 3. Condition Resolution
Conditions modify district behavior.

### 4. Influence Update
Influence shifts based on all systems.

### 5. Slot Pressure
Slots enforce capacity and constraints.

### 6. Event Checks
Triggers emergent events.

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