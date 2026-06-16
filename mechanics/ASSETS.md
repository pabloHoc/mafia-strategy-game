# Assets

**Status:** WIP

## Purpose

Assets are the primary representation of leverage in the game.

They provide capabilities, opportunities, and influence that organizations use to pursue their ambitions. Assets serve as the central abstraction connecting districts, organizations, missions, and politics.

The mechanic exists to create meaningful decisions about acquisition, delegation, risk, and commitment.

## Core Concept

Assets represent persistent leverage over the world rather than simple possessions or resources.

A nightclub, a gang, a secret, a smuggling route, or a debt can all be assets because they enable the organization to influence events and pursue opportunities.

Assets are acquired, assigned, improved, risked, and sometimes lost. Power comes not from owning assets, but from using them effectively.

## Entities

- Asset
- Organization
- Lieutenant
- District
- Mission

## Rules

### Asset Properties

Every asset has a common interface:

- Type
- Tags
- Owner
- Location (optional)
- Assignment
- State
- Exposure
- Upkeep (optional)
- Capabilities

This interface allows assets to interact with multiple systems consistently.

### Assignment

Assets may be assigned to:

- Lieutenants
- Districts
- Missions
- Organizations

Assignments determine what an asset is currently contributing to and may restrict other uses.

### Exposure

Assets generate risk.

Powerful or active assets may attract attention from rivals, authorities, or supernatural forces.

Growth increases both influence and vulnerability.

### State

Assets may exist in different states:

- Hidden
- Active
- Damaged
- Infiltrated
- Exhausted

State changes affect effectiveness and available actions.

### Lifecycle

Assets progress through a lifecycle:

- Acquisition
- Development
- Maintenance
- Decline
- Loss

Different asset types may follow different lifecycle rules.

### Capabilities

Assets provide capabilities that are used by other systems.

Examples include:

- Violence
- Stealth
- Influence
- Wealth
- Logistics
- Intel
- Occult
- Faith

Capabilities allow systems to remain generic and emergent.

## Player Interaction & Tradeoffs

Players decide:

- Which assets to acquire.
- Which lieutenants manage them.
- Which missions should risk them.
- Whether to expand or remain hidden.
- Whether to specialize or diversify.

Tradeoffs include:

- Growth vs safety.
- Delegation vs control.
- Short-term gain vs long-term leverage.
- Specialization vs resilience.

Assigning assets to one purpose often prevents their use elsewhere.

## Progression

### Early Game

Acquire basic assets and establish footholds.

Focus on survival, expansion, and opportunity.

### Mid Game

Develop specialized asset networks and delegate management to lieutenants.

Internal politics become increasingly important.

### Late Game

Manage vast networks of assets across multiple districts while balancing ambition, loyalty, and exposure.

Large organizations become powerful but difficult to control.

## Interactions

- `organizations.md`
- `lieutenants.md`
- `districts.md`
- `missions.md`
- `information.md`
- `debt.md`
- `schemes.md`

Assets are the connective tissue between most game systems.

## Examples

### Example: Smuggling Operation

A smuggling route provides Logistics and Wealth.

Assigning it to a mission increases potential rewards but also raises Exposure.

### Example: Political Blackmail

A secret provides Influence.

Using it may secure a short-term advantage but destroys future leverage.

## Design Notes

Assets are the primary abstraction of power in the game.

Assets represent leverage rather than ownership.

Characters and assets are separate systems:

- Assets represent leverage.
- Characters represent relationships and agency.

However, both may share similar card-based UI representations.

Generic groups such as gangs or spy cells may be modeled as assets, while named individuals remain characters.

## Open Questions

- [QUESTION] Can assets support multiple assignments simultaneously?
- [QUESTION] How much management capacity do lieutenants provide?
- [QUESTION] Which asset states are universal and which are type-specific?
- [QUESTION] Should some assets be consumable while others remain persistent?

## TODO

- [ ] Define assignment rules in detail.
- [ ] Define capability values and scaling.
- [ ] Define exposure mechanics.
- [ ] Define asset acquisition and generation.
- [ ] Define specific asset types as content.
