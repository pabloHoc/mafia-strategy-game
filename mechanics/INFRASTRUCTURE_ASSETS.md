# Infrastructure Assets

**Status:** Exploration / Checkpoint

## Summary

Infrastructure Assets are persistent pieces of criminal infrastructure that the faction controls and deploys into districts.

Examples:

- Black Market
- Smuggling Route
- Safehouse
- Casino
- Front Company
- Spy Network
- Workshop

They represent long-term leverage embedded in the world rather than temporary favors or consumable influence.

Infrastructure Assets are not passive stat bonuses and are not attached directly to missions by default.

Instead, they are deployed into districts, creating local opportunities that can later be committed to missions and other activities.

---

# Mental Model

Infrastructure Assets answer:

> "What capabilities and opportunities exist in this territory?"

Examples:

- A Black Market means illegal goods can be acquired.
- A Smuggling Route means people and cargo can be moved secretly.
- A Safehouse means agents can disappear from public view.
- A Casino means money can be generated and laundered.

Owning an asset is not enough.

The player must decide:

- Where to deploy it.
- When to use it.
- What purpose to use it for.

---

# Gameplay Loop

## 1. Acquire

The faction gains control of an Infrastructure Asset.

Examples:

- Establish a Black Market.
- Capture a Smuggling Route.
- Build a Safehouse.

---

## 2. Deploy

The asset is assigned to a district.

Example:

Old Port:
- Smuggling Route
- Black Market

Downtown:
- Casino
- Front Company

This creates strategic territorial decisions.

---

## 3. Generate Opportunities

Assets create local opportunities and mission options.

Example:

Black Market:
- Acquire Contraband
- Acquire Forged Documents
- Fence Stolen Goods

Smuggling Route:
- Secret Transportation
- Cargo Movement
- Cross-Border Escape

Safehouse:
- Lay Low
- Hide Evidence
- Shelter Fugitive

---

## 4. Commit

When a mission or situation arises, the player may commit available assets.

Example:

Mission Requirement:
- Escape

Available Solutions:
- Smuggling Route
- Safehouse
- Corrupt Police

Player chooses one.

The asset becomes occupied, exposed, exhausted, or otherwise involved.

---

## 5. Consequences

Using assets may create risks.

Examples:

Smuggling Route:
- Gains Exposure
- May be disrupted

Safehouse:
- Location may be discovered

Black Market:
- Attracts institutional attention

The asset itself becomes part of the strategic game.

---

# Mission Interaction

Infrastructure Assets do not automatically help all missions.

Instead:

1. Assets are compatible with certain mission types.
2. Assets can contribute to specific mission requirements.
3. Different assets solve the same requirement in different ways.

Example:

Requirement:
- Escape

Smuggling Route:
+ Fast extraction
+ Move cargo
- Exposure on route

Safehouse:
+ Reduce Heat
+ Protect agents
- Slower

Corrupt Police:
+ Cancel pursuit
- Consumes favor

All contribute to Escape.

Each creates different outcomes and tradeoffs.

---

# Why Not Direct Mission Assignment?

Rejected model:

Asset Inventory
→ Assign Asset To Mission

Problems:

- Districts become less meaningful.
- Assets feel disconnected from territory.
- Assets can unrealistically help missions anywhere.

Preferred model:

Asset
→ Deployed In District
→ Creates Local Opportunities
→ Committed To Mission When Relevant

This creates both strategic and tactical decisions.

---

# Tradeoffs

## Strategic

Where should the asset be deployed?

Example:

Smuggling Route:
- Industrial Zone
- Harbor
- Border District

Only one location at a time.

---

## Tactical

How should the asset be used?

Example:

Smuggling Route can support:

- Cargo Movement
- Escape
- Infiltration

Using it for one purpose may prevent other uses.

---

## Risk

Using assets creates exposure.

Powerful infrastructure tends to attract:

- Police attention
- Rival interest
- Institutional pressure

---

# Asset Identity

A major design goal is preventing assets from becoming generic capability providers.

Bad:

Black Market:
- Logistics +2

Smuggling Route:
- Logistics +2

Result:
Assets become flavor variants of the same mechanic.

Preferred:

Black Market:
- Acquire Contraband
- Acquire Forged Documents
- Fence Goods

Smuggling Route:
- Secret Transportation
- Cross-Border Escape
- Move Cargo

Assets may solve similar mission requirements while remaining strategically distinct.

---

# Open Questions

- How many mission requirements should exist globally?
- How many mission types should exist globally?
- Can assets support missions in neighboring districts?
- How long does asset commitment last?
- How much exposure should asset use generate?
- Can multiple assets contribute to the same requirement simultaneously?
- Can assets be upgraded to unlock additional opportunities?

---

# TODO

- [ ] Define mission type taxonomy.
- [ ] Define mission requirement taxonomy.
- [ ] Define asset commitment/exhaustion rules.
- [ ] Define exposure and disruption mechanics for assets.
- [ ] Define district range rules (local vs neighboring districts).
- [ ] Create first pass list of infrastructure assets and their opportunities.
- [ ] Stress test with 20+ asset examples to detect overlap and genericization.
