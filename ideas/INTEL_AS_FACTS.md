# Intel as Facts (Investigation System)

**Status**

Consolidated exploration (pre-implementation design)

## 1. Core Problem We Are Solving

We are defining the ****ontological role of Intel in the game****, specifically:

- What Intel *is** (not just how it works)
- What Intel *allows the player to do**
- How investigation produces meaningful gameplay without becoming:
    - optimization puzzle
    - mission gatekeeping
    - content explosion
    - passive waiting loop

## 2. Rejected Models (What Did NOT Work)

### 2.1 Intel as Currency

Intel points → spend to get advantages

**Why it failed**

- Becomes mana system
- Removes narrative grounding
- Encourages optimization gameplay
- Collapses all information into a single stat

### **2.2 Intel as Direct Mission Unlocking**

Investigation → unlock mission

**Why it failed**

- Turns investigation into gatekeeping
- Encourages mandatory pre-mission prep loops
- Makes Intel feel required instead of strategic
- Creates linear progression structure

### **2.3 Intel as Counter-Puzzle System**

Investigation → discover counter → solve mission

**Why it failed**

- Causes content explosion (tags, counters, conditions)
- Turns gameplay into puzzle matching
- Reduces systemic depth to combinatorics
- Becomes “bring correct answer” gameplay

### **2.4 NPC-Centric Intelligence Model**

Named individuals with secrets and interactions

**Why it failed (at scale)**

- Character explosion risk
- Management complexity grows exponentially
- Too granular for institution-level strategy game
- Pushes toward simulation game instead of strategy abstraction

## **3. Key Design Shift (Core Insight)**

**Intel is NOT:**

- a resource
- a currency
- a progression layer
- a mission unlock system

**Intel IS:**

Knowledge about the structure of the world

More precisely:

Facts about institutions, relationships, and states

## **4. Final Ontological Model**

### **4.1 World is made of Institutions (primary entities)**

Examples:

- Police Department
- Union
- Church
- Port Authority
- Criminal Network

No focus on individual NPC simulation.

## **4.2 Institutions contain FACTS**

Facts are structured truths about the world:

**Internal facts**

- corruption
- debt
- instability
- factional conflict

**Relationship facts**

- Police hostile to Union
- Church allied with Nobles
- Mayor controls Police

Facts are:

- not consumable
- not resources
- not inventory items

They represent reality.

### **4.3 Facts DO NOT directly create rewards**

Facts do not give:

- bonuses
- currency
- direct missions

They enable interpretation of the world state.

### **4.4 Facts change AVAILABLE ACTION SPACE**

Facts influence what actions become logically valid or effective.

They do NOT:

- unlock missions explicitly
- spawn content items

They modify *what the world allows you to attempt meaningfully*.

## **5. Core Gameplay Loop**

### **5.1 Investigation Loop (mechanical definition)**

**Choose:**

- Institution target
- Focus domain
- Method (assets used)

**Resolve:**

- cost (time, wealth, asset usage)
- risk (heat, exposure)
- output (partial facts)

**Output format:**

- structured facts
- uncertain / partial / probabilistic
- attached to institutions (not inventory)

### **5.2 Fact Storage**

Facts are stored:

On Institutions (world state)

Example:

Police Department:

- financial irregularities (known)
- internal rivalry (suspected)

Player does NOT store facts as items.

### **5.3 Missions (separate layer)**

Missions are NOT unlocked.

They are continuously derived from world state:

World state → determines viable actions

### **5.4 Exploitation Layer (what player does with facts)**

Facts enable **missions or operations such as**:

- Blackmail institution/actor
- Support faction
- Expose corruption
- Manipulate relationships
- Sabotage operations

These are NOT unlocks.
They are **context-sensitive available operations**.

## **6. Key System Insight**

**Investigation is NOT:**

- mission generation
- reward loop
- puzzle solving system

**Investigation IS:**

A constrained action that converts uncertainty into structured world knowledge.

## **7. Tradeoffs in Investigation System**

### **7.1 Depth vs Exposure**

- deeper investigation → more precise facts
- higher heat / risk

### **7.2 Breadth vs Specificity**

- broad → many weak signals
- focused → fewer but actionable facts

### **7.3 Asset Allocation**

Assets define:

- what domains you can access
- what kinds of facts you are likely to uncover
- how risky investigation is

### **7.4 Opportunity Cost**

Investigation competes with:

- expansion
- missions
- reactive gameplay

Intel is not free progression.

## **8. Role of Assets (Clarified)**

Assets do NOT:

- add flat investigation power

Assets DO:

- provide access channels (perspective)
- define information domain coverage
- influence type of facts discovered

Examples:

- informants → street-level facts
- political contacts → institutional facts
- corrupt officials → internal facts

## **9. Key System Relationships**

- Investigation → produces Facts
- Facts → modify world state understanding
- World state → defines available meaningful actions
- Actions (missions/operations) → change world state

## **10. What Works Well in This Direction**

- No NPC explosion (institution-level abstraction)
- No Intel currency system
- No direct mission unlocking
- No puzzle-based counters
- Strong systemic clarity (facts → world state → actions)
- Scalable content model (institution archetypes + fact types)

## **11. Remaining Design Sensitivity (not yet solved, but scoped)**

- Exact granularity of “facts” per institution
- How frequently facts decay or change (if at all)
- How visible partial knowledge is to the player UI
- How derived actions are presented without feeling like unlocks
- Ensuring missions feel distinct from “derived options list”

## **12. Final Conclusion**

**Intel is:**

- A structured representation of partial truth about institutions,
- revealed through constrained investigations,
- used to reshape the space of meaningful actions in the world.

**Investigation is:**

- A risky, resource-constrained operation that trades time, exposure, and assets
- for structured knowledge about institutional reality.

**Missions are:**

- Continuously available actions whose effectiveness and viability
- depend on the current known state of the world.
