# Intel Exploration — Intelligence Networks & Investigations

**Status:** Discarded. Superseeded by [INTEL MECHANIC](../mechanics/INTEL.md)

## Core Realization

The concept of a global "Intel" resource creates thematic and mechanical problems.

Example:

```text
Learn about a labor strike
↓
Gain Intel
↓
Spend Intel on a governor
```

This abstraction feels disconnected from the fantasy.

Additionally, Intel as a generic resource tends to become:

```text
Gather Intel
→ Spend Intel
→ Get Better Outcomes
```

which risks becoming another currency rather than an interesting system.

---

# Rejected Direction: Intel as a Global Resource

Example:

```text
Intel: 25
```

Used to:

```text
Spend 5 Intel
→ Reveal mission details
```

Problems:

- Feels artificial.
- Information loses its source and context.
- Encourages optimization loops.
- Similar to "mana" rather than intelligence.

---

# Emerging Direction

Remove Intel as a spendable resource entirely.

Instead:

```text
Assets
→ Enable Investigations
→ Generate Discoveries
→ Create Opportunities
```

---

# Intelligence Network Model

## Intelligence Assets

The player builds a network of contacts and information sources.

Examples:

- Dock Contact
- Corrupt Clerk
- Watch Captain
- Union Agitator
- Noble Informant
- Smuggler Associate

These are permanent assets.

They represent access to specific parts of society.

---

## Design Principle

Assets do NOT generate information passively.

Bad:

```text
Dock Contact
→ Generates Smuggling Opportunity every few turns
```

This behaves like a resource generator.

Instead:

```text
Dock Contact
→ Unlocks Dock Investigations
```

The player must actively choose to use the network.

---

# Investigations

Investigations are operations.

The player decides:

```text
What are we trying to learn?
```

Examples:

- Investigate Governor
- Search for Leverage
- Investigate Docks
- Investigate Rival Organization
- Investigate Institution
- Search for Opportunities

Investigations consume scarce resources such as:

- Operation Capacity
- Agent Assignment
- Time
- Exposure Risk

---

# Asset-Driven Investigations

Different assets enable different investigations.

Example:

### Dock Contact

Can investigate:

- Smuggling Routes
- Merchant Activity
- Shipping Records

---

### Corrupt Clerk

Can investigate:

- Tax Records
- Noble Finances
- Government Contracts

---

### Union Agitator

Can investigate:

- Labor Unrest
- Worker Leaders
- Industrial Districts

---

This creates a clear relationship between:

```text
Asset
→ Investigation Type
→ Discovery Type
```

---

# Discoveries

Investigations generate discoveries.

Examples:

- Secret
- Lead
- Opportunity
- Vulnerability
- Contact
- Scheme

Discoveries are specific and contextual.

Examples:

```text
Governor Embezzling Funds
```

```text
Weakly Defended Warehouse
```

```text
Rival Smuggling Route
```

```text
Disgruntled Guard Captain
```

---

# Secrets vs Intelligence

Potential distinction:

## Intelligence Network

A capability.

Represents:

- Contacts
- Informants
- Information assets
- Access to information

Used to perform investigations.

---

## Secrets

A resource.

Represents discovered leverage.

Examples:

- Blackmail Material
- Hidden Relationships
- Corruption Evidence

Can be consumed by other mechanics.

Examples:

- Coercion
- Negotiation
- Recruitment
- Political Pressure

---

# Sources of Intelligence Assets

Several possible sources exist.

## Missions

Missions may provide network-building rewards.

Example:

```text
Labor Strike
```

Possible reward:

```text
Union Informant
```

instead of immediate wealth.

---

Example:

```text
Tax Office Raid
```

Possible reward:

```text
Corrupt Clerk
```

---

## Organizations

Organizations may generate or recruit specialized contacts.

Example:

```text
Smuggling Organization
```

can recruit:

```text
Dock Contacts
```

---

## District Presence

Strong district influence may unlock local recruitment opportunities.

Example:

```text
High Influence in Industrial District
```

allows:

```text
Recruit Labor Informant
```

---

# Investigation Outcomes

Investigations should not be guaranteed success.

Possible outcomes:

- Valuable Discovery
- Minor Lead
- No Useful Information
- Exposure
- Counter-Intelligence Response

This creates risk and uncertainty.

---

# Strategic Loop

```text
Acquire Intelligence Assets
          ↓
Unlock Investigation Options
          ↓
Choose What To Investigate
          ↓
Generate Discoveries
          ↓
Exploit Discoveries
          ↓
Expand Network
```

---

# Current Design Principles

## Principle 1

Intel should not primarily improve existing actions.

Bad:

```text
Investigate
→ +10% Mission Success
```

Good:

```text
Investigate
→ New Opportunity
```

---

## Principle 2

Information should have a source.

The network that discovers information determines:

- What can be investigated.
- What can be discovered.

---

## Principle 3

Investigation should be active.

Players should choose:

```text
What are we trying to learn?
```

rather than receiving passive information.

---

## Principle 4

Intelligence should create options.

The primary purpose of intelligence is to reveal:

- Opportunities
- Vulnerabilities
- Relationships
- Secrets
- Schemes

not to optimize probabilities.

---

# Open Questions

- Do investigations require agents?
- Do investigations occupy operation capacity?
- How long should investigations take?
- How much randomness is desirable?
- How are discoveries stored and surfaced to the player?
- Which discoveries become consumable "Secrets"?
- Can rivals conduct counter-intelligence against investigations?
- Are intelligence assets unique entities or generic network strength?
