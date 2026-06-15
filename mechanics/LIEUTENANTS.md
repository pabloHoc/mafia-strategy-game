# Lieutenant & Organization System

**Status:** WIP

## Purpose

Lieutenants are the primary bottleneck of organizational growth.

This mechanic exists to:

- Prevent asset and territorial snowballing.
- Shift progression from accumulation to organization.
- Create internal politics and emergent stories.
- Compress complexity through delegation.

Core principle:

> Power is limited not by money or territory, but by trusted people.

## Core Concept

Lieutenants are character assets that provide organizational capacity and manage portions of the player's organization.

Growth creates instability: promoting capable subordinates grants power but also creates future rivals.

Personhood begins at promotion. Before promotion, candidates are lightweight previews rather than fully simulated characters.

## Entities

- Lieutenant (asset)
- Underboss
- Goon Group (asset)
- Candidate
- Managed Asset

## Rules

### Organizational Structure

Early:

Boss
- Lieutenants

Late:

Boss
- Underboss
  - Lieutenants

Progression is organizational sophistication rather than asset accumulation.

### Ownership Model

Player → Lieutenants → Assets

Lieutenants manage:
- Assets
- Goons
- Ongoing operations

Lieutenants do not own districts.

### Capacity

Each lieutenant provides organizational capacity.

Example formula:

`Capacity = Leadership × Rank + Traits`

Overextension may cause:
- Reduced efficiency
- Increased exposure
- Lower loyalty
- Asset decay

### Promotion

Goon groups accumulate XP and generate candidates.

The player chooses which group's candidate to promote.

Promotion:
- Creates a Lieutenant asset
- Grants organizational capacity
- Unlocks politics
- Weakens the source group

Possible weakening:
- Strength -1
- XP reset
- Temporary efficiency penalty

### Personhood

Before promotion candidates:
- Are visible
- Have traits and specialization
- Cannot participate in politics
- Cannot become angry

After promotion lieutenants gain:
- Loyalty
- Ambition
- Influence
- Political agency

### Politics

Politics emerge from ownership.

Examples:
- Rivalries
- Succession struggles
- Power blocs
- Betrayal

Politics should be event-driven rather than constantly simulated.

### Dependence

Powerful lieutenants become difficult to remove.

Removing them may cause:
- Asset disruption
- Loss of efficiency
- Disloyalty

## Player Interaction

Players decide:

- Which groups to develop.
- Which candidates to promote.
- Which assets to assign.
- Whether to centralize or distribute power.
- How to respond to ambitions.
- Whether to remove dangerous lieutenants.

## Progression

### Early Game

1–3 lieutenants.
Minimal politics.

### Mid Game

Specialized lieutenants manage operations.
Politics emerge.

### Late Game

Underbosses and power blocs appear.
Internal politics become a major challenge.

## Interactions

- `MISSIONS.md` — Lieutenants participate in operations.
- `ASSETS.md` — Lieutenants manage assets.
- `INFORMATION.md` — Hidden traits and ambitions may exist.
- `DISTRICTS.md` — Groups originate from districts.

## Examples

### Example: Promotion

Dock Thugs
- Strength: 3
- XP: 85/100
- Candidate: Viktor

Promote Viktor:

- Create Lieutenant Viktor
- Candidate slot becomes empty
- Group weakened

Later:

Dock Thugs generate Elena.

### Example: Dangerous Dependence

Marco controls:
- 3 gangs
- 2 smuggling routes
- 40 goons

Removing Marco may destabilize the organization.

## Design Notes

Design principles:

- Growth creates instability.
- Complexity should emerge gradually.
- Event-driven politics are preferred.
- Specialties should unlock mechanics rather than percentages.

Avoid:
- Individual goon wages
- District governors
- Pairwise relationships between all lieutenants
- Complex inheritance laws

Decisions:
- Lieutenants are assets.
- Goon groups are assets.
- Personhood begins at promotion.
- Politics begin after promotion.

## Open Questions

- [QUESTION] What exactly does capacity constrain?
- [QUESTION] Which assets require management?
- [QUESTION] What does ownership mean mechanically?
- [QUESTION] How much autonomy should lieutenants have?
- [QUESTION] What happens when a lieutenant dies?

## TODO

- [ ] Define loyalty mechanics.
- [ ] Define ambition mechanics.
- [ ] Define removal mechanics.
- [ ] Define succession and inheritance.
- [ ] Define candidate generation rules.
- [ ] Validate that politics prevent snowballing.
