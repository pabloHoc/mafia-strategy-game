# Intel Exploration Checkpoint

**Status:** Exploration

## Core Realization

The original assumption was:

```text
Intel
→ Reveals Information
→ Better Mission Decisions
```

However, most implementations of this pattern create one of two problems:

### Certainty Optimization

```text
Gather Intel
→ Better Numbers
→ Better Estimates
```

Problems:

- Feels like optimization busywork.
- Encourages gathering Intel before every mission.
- Creates little strategic depth.
- Often becomes mandatory.

### Counter Discovery

```text
Gather Intel
→ Discover Obstacle
→ Bring Counter
```

Problems:

- Creates tag systems.
- Creates counter systems.
- Creates content explosion.
- Turns missions into puzzles.

---

## Rejected / Unpromising Directions

### Intel as Success Chance Estimation

Examples:

```text
Success Chance:
65%
```

Then:

```text
Success Chance:
78%
```

Problems:

- Mostly improves certainty.
- Doesn't create meaningful choices.
- Encourages optimization.

---

### Intel as Obstacle Discovery

Examples:

```text
Guards
Cameras
Locks
```

Problems:

- Leads to counter gameplay.
- Creates asset matching systems.
- Increases complexity and content requirements.

---

### Intel as Opportunity Timing

Examples:

```text
Wait 3 turns
→ Better opportunity
```

Problems:

- Encourages waiting.
- Delays mission execution.
- Can become:

Investigate
→ Wait
→ Wait
→ Execute

- Risks making optimal play inactive.

---

## Emerging Design Principle

Intel should rarely be:

```text
Intel
→ Better Execution
```

Intel should more often be:

```text
Intel
→ More Strategic Options
```

The goal is not to solve missions.

The goal is to reveal new possibilities.

---

# Intel and Missions

## Promising Direction: Alternative Angles

Intel reveals alternative ways to exploit the same situation.

Example:

Initial Mission:

```text
Treasury Raid
```

Intel may reveal:

```text
Rob Treasury
```

or

```text
Blackmail Treasurer
```

or

```text
Embezzle Funds
```

or

```text
Frame Rival Organization
```

The mission becomes richer rather than easier.

---

## Important Constraint

Intel must not simply reveal additional rewards.

Bad:

```text
Reward:
Gold

Intel:
Gold + Documents
```

This is strictly better.

Players will always investigate.

---

Instead:

```text
Option A:
Gold

Option B:
Blackmail Material

Option C:
Influence
```

Mutually exclusive outcomes create tradeoffs.

---

## Important Constraint

Intel discoveries should not be random.

Bad:

```text
Spend Intel
→ Random Objective
```

Problem:

Player may receive options they do not care about.

Feels frustrating.

Feels RNG-driven.

---

Prefer:

```text
Investigate Objectives
```

```text
Investigate Approaches
```

```text
Investigate Consequences
```

```text
Investigate Participants
```

The player directs the investigation.

---

## Important Realization

Intel spending does NOT need to be worthwhile every time.

Example:

Mission appears.

The player immediately sees an objective they already want.

Optimal play may simply be:

```text
Execute Mission
```

No Intel required.

This is healthy.

Otherwise Intel becomes mandatory.

---

# Broader Role of Intel

A strategic resource should have multiple competing uses.

Intel should not exist solely to support missions.

---

## Mission Discovery

Reveal:

- New missions
- Hidden opportunities
- Rival operations
- Rare events

---

## Mission Expansion

Reveal:

- Alternative objectives
- Alternative approaches
- Additional stakeholders
- New mission angles

---

## Faction Intelligence

Reveal:

- Rival priorities
- Income sources
- Organizational structure
- Ongoing schemes

Purpose:

Help choose targets and strategy.

---

## Scheme Discovery

Reveal:

- Hidden plots
- Long-term projects
- Emerging threats

Purpose:

Allow intervention or exploitation.

---

## Leverage Generation

Generate resources such as:

- Secrets
- Blackmail Material
- Dirt
- Weaknesses

These become usable assets rather than information.

---

## Counter-Intelligence

Hide:

- Schemes
- Missions
- Assets
- Organizational activity

Creates an information war layer.

---

## District Intelligence

Reveal:

- Power structures
- Corruption
- Emerging opportunities
- Threats

Purpose:

Provide strategic understanding of districts.

---

## Asset Discovery

Reveal unique opportunities:

- Corrupt officials
- Informants
- Smuggling routes
- Rare assets

These cannot simply be purchased.

They must be discovered.

---

# Current Working Definition

Intel is not primarily a certainty resource.

Intel is not primarily a counter-discovery resource.

Intel is a strategic resource used to reveal:

- Opportunities
- Leverage
- Vulnerabilities
- Relationships
- Hidden actions
- Alternative courses of action

---

# Current Design Principle

```text
Wealth makes actions stronger.

Intel makes new actions possible.
```

This creates a clear identity for the resource and allows it to interact with multiple systems without becoming a mandatory optimization step before every mission.
