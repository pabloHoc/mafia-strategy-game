
# **Minimal State Model Map (Whole Game)**

This is a high-level **system graph of what exists and how state changes**.

# **1. Core Entities**

## 1.1 Faction (Player + NPCs)

**State:**

- Resources (Wealth, Intel access, Influence)
- Asset network (owned / deployed / exposed assets)
- Active missions (committed operations)
- Known intel (discovered information graph)
- Relationships (factions, institutions)

**Transitions:**

- gains/loses assets via missions/events
- gains intel via investigations and missions
- gains/loses influence via district outcomes
- reacts to world events and other factions

## 1.2 Mission (Core Execution Entity)

**States:**

- **Opportunity (pre-selection / world state)**
- **Shell (selected, in preparation)**
- **Prepared (assets + approach locked)**
- **Active (world simulation running)**
- **Resolved (final outcomes applied)**

**Transitions:**

- Opportunity → Shell (player or world trigger)
- Shell → Prepared (player commits setup)
- Prepared → Active (start execution)
- Active → Resolved (end condition reached)

## 1.3 Assets (Capability Entities)

**States:**

- **Idle (available)**
- **Deployed (assigned to district)**
- **Committed (assigned to mission)**
- **Active (in use during execution)**
- **Exposed / Damaged / Compromised**
- **Lost / Destroyed**

**Transitions:**

- Idle → Deployed (placed in district)
- Deployed → Committed (used in mission prep)
- Committed → Active (mission starts)
- Active → Exposed/Damaged/Lost (execution outcomes)
- Active → Idle (return after safe resolution)

## 1.4 District (World Container State)

**States:**

- Influence map (factions’ control levels)
- Condition set (temporary modifiers)
- PoIs state (controlled / contested / neutral)
- Active missions affecting district

**Transitions:**

- influenced by missions
- modified by assets presence
- updated through periodic world ticks
- shifts control between factions

## 1.5 Intel Network (Information System)

**States:**

- Unknown → Known → Exploited → Obsolete
- Investigation nodes (active / completed)
- Network strength per faction (coverage levels)

**Transitions:**

- Unknown → Known (via investigation or events)
- Known → Exploited (used in missions/assets decisions)
- Known → Obsolete (world state changes)
- Network expands via assets and contacts

## 1.6 Institution (Police / Corps / Government)

**States:**

- Awareness level per district
- Internal stability
- Corruption level
- Active investigations / responses

**Transitions:**

- reacts to mission visibility
- gains awareness via intel signals
- modifies district pressure
- triggers interference in missions

# 2. Global Systems (Meta State)**

## 2.1 Time System

**State:**

- discrete cycles / ticks (undefined granularity)

**Transitions:**

- advances world state
- progresses missions
- triggers district updates
- resolves delayed effects

## 2.2 World State (Emergent Layer)

**State:**

- distribution of influence across districts
- active conflicts
- ongoing missions
- instability levels per region

**Transitions:**

- updated by all entity systems
- produces new opportunities (missions, intel, events)

# 3. Key Interaction Loops

These are the **actual gameplay loops implied by the model**:

## 3.1 Mission Loop

District / Intel / Event

→ Opportunity

→ Mission Shell

→ Preparation (Assets + Approach)

→ Activation

→ Execution (world reacts)

→ Resolution

→ World state changes

## 3.2 Asset Loop

Faction acquires asset

→ deploys to district

→ uses in missions

→ asset becomes exposed or evolves

→ returns / lost / changed

→ affects future missions and districts

## 3.3 Intel Loop

Unknown world state

→ investigation / infiltration

→ knowledge gained

→ alternative mission options created

→ used in preparation or strategy

→ becomes obsolete or updated

## 3.4 District Loop

missions + assets + institutions

→ influence shifts

→ conditions change

→ PoIs shift control

→ new opportunities appear

→ feeds back into missions + intel

# 4. Critical System Boundaries

**Capability Layer (Assets)**

_“What you can do”_

**Knowledge Layer (Intel)**

_“What you understand is possible”_

**Action Layer (Missions)**

_“What you commit to doing”_

**World Layer (Districts + Institutions)**

_“What reacts and evolves”_
