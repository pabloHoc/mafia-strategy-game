# Mission Approaches, Axes, and Resolution

**Status:** Discarded. Superseeded by [MISSIONS](../mechanics/MISSIONS.md)

## Core Idea

Introduce **Approaches** (formerly "Means") as mission stances that define **how** a mission is executed.

Approaches are:

- Not stats
- Not resources
- Not capabilities
- Not numeric values

Approaches are:

> Operational doctrines chosen per mission.

Examples:

- Force
- Intrigue
- Commerce
- Faith
- Knowledge

---

## Relationship with Capabilities

Capabilities answer:

> What resources do you possess?

Approaches answer:

> How are you solving this problem?

**Capabilities are ingredients.**
**Approaches are recipes.**

Example:

- Spy Network
  - Stealth +3
  - Intel +2

Under **Intrigue**:
- Highly effective

Under **Force**:
- Less effective

The same resource can be used differently depending on the approach.

---

## Mission Structure

Each mission defines:

- Objectives
- Rewards
- Consequences
- **2–4 Axes**
- Supported Approaches

Example:

### Assassinate Noble

Axes:
- Elimination
- Secrecy
- Escape

Supported approaches:
- Force
- Intrigue
- Commerce

---

## Soft Restrictions

Avoid hard restrictions.

Prefer:

> An approach is possible, but carries different risks.

Example:

**Acquire Church Support**

Faith:
- Natural approach
- Low risk

Force:
- Possible
- Massive backlash

---

## Approach Effects

Approaches modify:

- Capability weights
- Discovery profile
- Exposure generated
- Fallout profile

Example:

### Force

Strengths:
- Violence
- Escalation

Weaknesses:
- Visibility
- Heat

Typical consequences:
- Fear
- Damage
- Retaliation

---

### Intrigue

Strengths:
- Stealth
- Intel

Weaknesses:
- Fragile if discovered

Typical consequences:
- Secrets
- Suspicion
- Blackmail

---

## Resolution Framework

Resources provide capabilities.

Approaches modify capabilities.

Effective capabilities generate:

1. Overall Mission Strength
2. Axis Scores

Flow:

Resources
→ Capabilities
→ Approach Modifiers
→ Effective Capabilities
→ Mission Strength
→ Axis Scores
→ Consequences

---

## Mission Strength

Single value used for:

- Success level
- Escalation
- Reserves

Possible outcomes:

- Critical Success
- Success
- Partial Success
- Failure
- Catastrophic Failure

---

## Axis Scores

Axes generate consequences and stories.

Important:

> Players should rarely win every axis.

Approaches redistribute power rather than increase it.

Example:

### Assassinate Noble

**Force Build**

Axes:

| Axis | Score |
|------|-------|
| Elimination | High |
| Secrecy | Low |
| Escape | Medium |

Outcome:

> The noble dies, but witnesses identify your crew.

---

**Intrigue Build**

| Axis | Score |
|------|-------|
| Elimination | Medium |
| Secrecy | High |
| Escape | High |

Outcome:

> The noble dies quietly and nobody knows who was responsible.

---

## Opposed Missions

Attackers and defenders may choose different approaches.

Example:

Attacker:
- Intrigue

Defender:
- Force

Approaches do not directly counter each other.

Instead:

- Resources contribute capabilities.
- Missions determine which capabilities matter.

Example:

Intel Network vs Enforcers

Not:

> Intrigue beats Force

Instead:

- Intel helps avoid detection.
- Enforcers improve patrols and response.

The fiction creates the interaction.

---

## Consequences by Axis

Examples:

| Axis Lost | Consequence |
|-----------|-------------|
| Secrecy | Heat, exposure |
| Escape | Captured crews |
| Legitimacy | Public backlash |
| Violence | Territory damage |
| Influence | Reputation loss |

Design principle:

> Players optimize which consequences they are willing to accept.

Not simply whether they succeed.

---

## Design Principles

- Approaches create different stories.
- The same mission can be solved in multiple ways.
- Resources remain reusable across approaches.
- Avoid rock-paper-scissors counters.
- Prefer soft counters and emergent interactions.
- The city remembers how power was used.

## Open Questions

- [QUESTION] What is the final list of Approaches (4–5 maximum)?
- [QUESTION] Are Approaches chosen only by attackers, or also by defenders during interference?
- [QUESTION] Which Approaches are naturally suited for each mission template?
- [QUESTION] Should unsupported Approaches be forbidden or merely penalized?
- [QUESTION] Which mission templates exist (Covert, Political, Open Conflict, etc.)?
- [QUESTION] Which 2–4 Axes does each mission template use?
- [QUESTION] Which capabilities contribute to each Axis?
- [QUESTION] Are Axis scores opposed, one-sided, or environment-based?
- [QUESTION] Do defenders contest every Axis or only some of them?
- [QUESTION] How exactly are Axis scores calculated?
- [QUESTION] How strongly should Approaches modify capabilities?
- [QUESTION] How does Intel affect Mission Strength and individual Axes?
- [QUESTION] How do hidden reserves affect Mission Strength and Axes?
- [QUESTION] Are Axis values visible to players or abstracted into labels?
- [QUESTION] Can players intentionally sacrifice some Axes for strategic benefits?
- [QUESTION] How are ties resolved on individual Axes?
- [QUESTION] How much randomness should exist in Axis resolution?
- [QUESTION] Should certain Approaches generate unique world consequences?
- [QUESTION] How does AI choose Approaches and prioritize Axes?
- [QUESTION] Does this system create genuinely different stories or merely different numbers?

## TODOs

- [ ] Define the final list of Approaches.
- [ ] Define capability weighting for each Approach.
- [ ] Define discovery and exposure profiles for each Approach.
- [ ] Define unique fallout profiles for each Approach.
- [ ] Create 5–8 reusable mission templates.
- [ ] Define 2–4 Axes for each mission template.
- [ ] Define which capabilities contribute to each Axis.
- [ ] Define the formula for calculating Mission Strength.
- [ ] Define the formula for calculating Axis scores.
- [ ] Define how Intel modifies Mission Strength and Axes.
- [ ] Define how reserves modify Mission Strength and Axes.
- [ ] Define how defenders interfere with missions.
- [ ] Define whether defenders choose their own Approach.
- [ ] Define consequences for winning or losing each Axis.
- [ ] Define how Axis outcomes generate Heat, Exposure, and Debts.
- [ ] Define how Axis outcomes affect districts and organizations.
- [ ] Define UI for mission planning and Axis previews.
- [ ] Prototype a complete mission (e.g. Assassinate Noble).
- [ ] Simulate multiple scenarios by hand to validate tradeoffs.
- [ ] Validate that no single Approach dominates all situations.
- [ ] Validate that players cannot consistently maximize every Axis.
- [ ] Validate that the system produces emergent stories rather than optimization puzzles.
