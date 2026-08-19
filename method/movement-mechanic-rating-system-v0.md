# Movement Mechanic Rating System (v0)

Purpose: create a reusable way to rate movement mechanics, rituals, and persuasion structures without collapsing them into one dumb score.

Mission context:
This is part of the movement-DNA research program. The goal is to understand **what works, how it works, when it works, what it costs, and what it risks**.

This is **not** an Apotheosis implementation doc.

Project role:
- score mechanics after extraction so the database can compare them across targets
- separate raw potency from strategic usefulness and risk load
- produce reusable mechanic profiles that may later inspire Monolith design choices without turning this file into direct Monolith design work

---

## Core principle

Do **not** ask:
- “Is this mechanic effective?”

Ask instead:
- Effective **for what**?
- Effective **under what conditions**?
- Effective **at what cost**?
- Effective **for how long**?
- Effective **for whom**?

A ritual or mechanic can be:
- extremely potent,
- strategically useful in some contexts,
- weak in others,
- and dangerously unstable overall.

So each mechanic gets a **profile**, not a single grade.

---

# 1) Scoring model

Use a **1–5 scale** for each dimension.

## Score meanings
- **1 = very low / weak / rare / negligible**
- **2 = low**
- **3 = moderate**
- **4 = high**
- **5 = very high / core-defining / dominant**

Use half-steps only if truly helpful (`2.5`, `3.5`, etc.).
Default to whole numbers.

---

# 2) Layer One — Functional efficacy

These scores rate **what job the mechanic does** inside a movement.

## 2.1 Attraction Power
How strongly does it pull people in at the edge?

Questions:
- does it create curiosity, taboo, prestige, safety, novelty, or longing?
- is it easy to pitch or show?

## 2.2 Conversion Power
How strongly does it move a person from observer to participant?

Questions:
- does it help people cross a threshold fast?
- does it produce “I’m in” energy?

## 2.3 Bonding Power
How strongly does it create closeness, belonging, or social glue?

Questions:
- does it make members feel bonded to each other?
- does it create emotional memory with others present?

## 2.4 Identity-Installation Power
How strongly does it alter self-concept?

Questions:
- does it make the person feel remade, seen differently, renamed, chosen, purified, upgraded, or newly initiated?

## 2.5 Retention Power
How strongly does it keep people returning or staying loyal?

Questions:
- does it reinforce repeat participation?
- does leaving feel costly?

## 2.6 Zeal / Evangelism Power
How strongly does it make members preach, recruit, defend, or spread?

Questions:
- does it create witness energy?
- does it turn members into missionaries?

## 2.7 Status-Generation Power
How strongly does it create hierarchy, aspiration, or visible advancement?

Questions:
- does it create winners, ranks, inner circles, badges, or closeness-to-center?

## 2.8 Operator-Formation Power
How strongly does it help create leaders, coaches, sponsors, missionaries, or enforcers?

Questions:
- does it naturally produce a next layer of people who maintain the system?

## 2.9 Distribution Power
How strongly does it help the movement spread itself?

Questions:
- does it generate shareable proof, inviting behavior, referral loops, or ritualized recruiting?

## 2.10 Durability of Effect
How long do the effects tend to last?

Questions:
- is it mostly a temporary high?
- or does it compound into durable identity and behavior?

---

# 3) Layer Two — Strategic viability

These scores rate **how practical the mechanic is as part of a system**.

## 3.1 Scalability
How easily does it scale across larger groups, more locations, or digital channels?

## 3.2 Operational Simplicity
How easy is it to run reliably?

High score = simple, repeatable, low-overhead.
Low score = complex, facilitator-heavy, fragile, high-overhead.

## 3.3 Founder Independence
How well does it function without a singular charismatic center?

High score = works even without founder presence.
Low score = dependent on one person’s charisma, body, voice, or aura.

## 3.4 Modularity
How easily can it plug into a broader system?

Questions:
- can it combine with doctrine, rank, recurring meetings, local nodes, digital distribution?
- or is it a very specialized one-off?

## 3.5 Observability / Debuggability
How easy is it to understand, measure, and tune the mechanic?

High score = easy to inspect, teach, improve, evaluate.
Low score = black-box, charisma-dependent, hard to isolate.

---

# 4) Layer Three — Risk / shadow profile

These are not moral side notes. They are core analytic dimensions.

## 4.1 Abuse Susceptibility
How easily can the mechanic become coercive, exploitative, manipulative, or predatory?

## 4.2 Reputation Fragility
How likely is the mechanic to trigger outsider backlash, scandal, mockery, or public collapse?

## 4.3 Legal / Regulatory Exposure
How likely is the mechanic to create civil, criminal, licensing, labor, safety, or consent issues?

## 4.4 Psychological Destabilization Risk
How likely is the mechanic to dysregulate, overwhelm, dissociate, traumatize, or destabilize participants?

## 4.5 Integration Burden
How much aftercare, context, or ongoing support is needed for the mechanic to remain stabilizing rather than damaging?

High score = requires substantial integration/support.
Low score = light integration needs.

---

# 5) Layer Four — Mechanism tags

Each mechanic should also be tagged by **what kind of force it uses**.

Possible tags:
- **aesthetic**
- **social**
- **ritual**
- **confessional**
- **sexual**
- **chemical**
- **ordeal**
- **status**
- **linguistic**
- **mythic**
- **economic**
- **synchrony-based**
- **authority-based**
- **distribution-based**

A mechanic can have multiple tags.

---

# 6) Composite views

After individual dimensions are scored, calculate three summary views.

## 6.1 Raw Potency
How powerful is the mechanic at creating immediate movement force?

Suggested ingredients:
- Attraction
- Conversion
- Bonding
- Identity Installation
- Zeal

## 6.2 Strategic Usefulness
How useful is the mechanic inside a durable movement architecture?

Suggested ingredients:
- Retention
- Operator Formation
- Distribution
- Durability
- Scalability
- Founder Independence
- Modularity

## 6.3 Risk Load
How heavy is the danger/shadow burden?

Suggested ingredients:
- Abuse Susceptibility
- Reputation Fragility
- Legal Exposure
- Psychological Destabilization
- Integration Burden

Important:
- a mechanic can have **very high Raw Potency** and **very low Strategic Usefulness**
- a mechanic can be powerful and still be a bad bet

---

# 7) Rating template

Use this block per mechanic.

```md
## Mechanic: <name>
Tags: <list>

### Description
<What the mechanic is and how it typically appears>

### Why it works
<Core causal explanation>

### Functional efficacy (1-5)
- Attraction:
- Conversion:
- Bonding:
- Identity Installation:
- Retention:
- Zeal / Evangelism:
- Status Generation:
- Operator Formation:
- Distribution:
- Durability:

### Strategic viability (1-5)
- Scalability:
- Operational Simplicity:
- Founder Independence:
- Modularity:
- Observability / Debuggability:

### Risk / shadow profile (1-5)
- Abuse Susceptibility:
- Reputation Fragility:
- Legal / Regulatory Exposure:
- Psychological Destabilization Risk:
- Integration Burden:

### Composite read
- Raw Potency:
- Strategic Usefulness:
- Risk Load:

### Notes
<Best conditions, failure modes, contrasts>
```

---

# 8) First-pass example ratings

These are working examples, not final truth.

## 8.1 Testimony / witness narrative
Tags: social, confessional, mythic, distribution-based

### Why it works
It creates self-recognition, social proof, emotional reality, and a script for transformation.

### Functional efficacy
- Attraction: 4
- Conversion: 4
- Bonding: 4
- Identity Installation: 4
- Retention: 4
- Zeal / Evangelism: 5
- Status Generation: 2
- Operator Formation: 3
- Distribution: 5
- Durability: 4

### Strategic viability
- Scalability: 5
- Operational Simplicity: 5
- Founder Independence: 5
- Modularity: 5
- Observability / Debuggability: 4

### Risk / shadow profile
- Abuse Susceptibility: 3
- Reputation Fragility: 2
- Legal / Regulatory Exposure: 1
- Psychological Destabilization Risk: 2
- Integration Burden: 2

### Composite read
- Raw Potency: high
- Strategic Usefulness: very high
- Risk Load: low-moderate

### Notes
AA is a strong example of testimony used as a durable healthy-control mechanic.

---

## 8.2 Sponsor / disciple / dyadic accountability bond
Tags: social, authority-based, confessional

### Why it works
It personalizes doctrine, creates direct accountability, and turns the system into a relationship rather than just content.

### Functional efficacy
- Attraction: 2
- Conversion: 4
- Bonding: 5
- Identity Installation: 4
- Retention: 5
- Zeal / Evangelism: 4
- Status Generation: 3
- Operator Formation: 5
- Distribution: 3
- Durability: 5

### Strategic viability
- Scalability: 3
- Operational Simplicity: 3
- Founder Independence: 5
- Modularity: 5
- Observability / Debuggability: 4

### Risk / shadow profile
- Abuse Susceptibility: 4
- Reputation Fragility: 2
- Legal / Regulatory Exposure: 2
- Psychological Destabilization Risk: 3
- Integration Burden: 3

### Composite read
- Raw Potency: high
- Strategic Usefulness: very high
- Risk Load: moderate

### Notes
Extremely strong for retention and operator formation. Shadow risk rises fast if authority is unbounded.

---

## 8.3 Daily ordeal / discipline challenge
Tags: ordeal, status, ritual

### Why it works
It converts identity into repeated proof, produces visible seriousness, and creates a simple binary standard.

### Functional efficacy
- Attraction: 4
- Conversion: 4
- Bonding: 3
- Identity Installation: 5
- Retention: 4
- Zeal / Evangelism: 4
- Status Generation: 3
- Operator Formation: 2
- Distribution: 4
- Durability: 4

### Strategic viability
- Scalability: 5
- Operational Simplicity: 5
- Founder Independence: 4
- Modularity: 4
- Observability / Debuggability: 5

### Risk / shadow profile
- Abuse Susceptibility: 2
- Reputation Fragility: 2
- Legal / Regulatory Exposure: 1
- Psychological Destabilization Risk: 3
- Integration Burden: 2

### Composite read
- Raw Potency: high
- Strategic Usefulness: very high
- Risk Load: low-moderate

### Notes
Strong example: 75 HARD style systems.

---

## 8.4 Secret mission / hidden knowledge
Tags: mythic, authority-based, linguistic, status

### Why it works
It creates elite identity, raises stakes, and turns sacrifice into service to something larger and hidden.

### Functional efficacy
- Attraction: 4
- Conversion: 3
- Bonding: 4
- Identity Installation: 5
- Retention: 5
- Zeal / Evangelism: 5
- Status Generation: 5
- Operator Formation: 4
- Distribution: 3
- Durability: 4

### Strategic viability
- Scalability: 4
- Operational Simplicity: 4
- Founder Independence: 2
- Modularity: 5
- Observability / Debuggability: 2

### Risk / shadow profile
- Abuse Susceptibility: 5
- Reputation Fragility: 4
- Legal / Regulatory Exposure: 3
- Psychological Destabilization Risk: 4
- Integration Burden: 3

### Composite read
- Raw Potency: very high
- Strategic Usefulness: high but unstable
- Risk Load: very high

### Notes
One of the strongest escalators in cultic systems.

---

## 8.5 Sexual ritual / eroticized initiation
Tags: sexual, ritual, bonding, status

### Why it works
It fuses taboo, intimacy, vulnerability, and embodied memory into a powerful adhesive event.

### Functional efficacy
- Attraction: 5
- Conversion: 4
- Bonding: 5
- Identity Installation: 4
- Retention: 4
- Zeal / Evangelism: 3
- Status Generation: 5
- Operator Formation: 2
- Distribution: 2
- Durability: 3

### Strategic viability
- Scalability: 2
- Operational Simplicity: 1
- Founder Independence: 1
- Modularity: 2
- Observability / Debuggability: 2

### Risk / shadow profile
- Abuse Susceptibility: 5
- Reputation Fragility: 5
- Legal / Regulatory Exposure: 5
- Psychological Destabilization Risk: 5
- Integration Burden: 5

### Composite read
- Raw Potency: very high
- Strategic Usefulness: low-moderate
- Risk Load: extreme

### Notes
Very strong on taboo attraction and bonding; strategically unstable and scandal-prone.

---

## 8.6 Drug-induced enlightenment / chemically mediated altered state
Tags: chemical, ritual, mythic

### Why it works
Altered states can create awe, revelation, ego disruption, bonding, and intense memory imprinting.

### Functional efficacy
- Attraction: 5
- Conversion: 4
- Bonding: 4
- Identity Installation: 5
- Retention: 3
- Zeal / Evangelism: 4
- Status Generation: 2
- Operator Formation: 2
- Distribution: 2
- Durability: 3

### Strategic viability
- Scalability: 2
- Operational Simplicity: 1
- Founder Independence: 2
- Modularity: 3
- Observability / Debuggability: 1

### Risk / shadow profile
- Abuse Susceptibility: 5
- Reputation Fragility: 4
- Legal / Regulatory Exposure: 5
- Psychological Destabilization Risk: 5
- Integration Burden: 5

### Composite read
- Raw Potency: very high
- Strategic Usefulness: low-moderate
- Risk Load: extreme

### Notes
Powerful experience engine; poor default mechanic for stable scalable architecture.

---

## 8.7 Miracle / proof event
Tags: mythic, authority-based, spectacle

### Why it works
It gives members a memory that feels stronger than argument: “I saw it myself.”

### Functional efficacy
- Attraction: 4
- Conversion: 5
- Bonding: 3
- Identity Installation: 4
- Retention: 4
- Zeal / Evangelism: 5
- Status Generation: 2
- Operator Formation: 1
- Distribution: 4
- Durability: 3

### Strategic viability
- Scalability: 3
- Operational Simplicity: 2
- Founder Independence: 1
- Modularity: 3
- Observability / Debuggability: 1

### Risk / shadow profile
- Abuse Susceptibility: 5
- Reputation Fragility: 5
- Legal / Regulatory Exposure: 4
- Psychological Destabilization Risk: 4
- Integration Burden: 3

### Composite read
- Raw Potency: high
- Strategic Usefulness: unstable
- Risk Load: very high

### Notes
Useful for understanding conversion and anti-doubt, but heavily tied to charisma theater.

---

## 8.8 Visible rank / sash / badge / status marker
Tags: status, social, ritual

### Why it works
It makes hierarchy legible, motivates imitation, and turns advancement into visible aspiration.

### Functional efficacy
- Attraction: 3
- Conversion: 2
- Bonding: 3
- Identity Installation: 4
- Retention: 5
- Zeal / Evangelism: 3
- Status Generation: 5
- Operator Formation: 4
- Distribution: 3
- Durability: 4

### Strategic viability
- Scalability: 5
- Operational Simplicity: 4
- Founder Independence: 4
- Modularity: 5
- Observability / Debuggability: 5

### Risk / shadow profile
- Abuse Susceptibility: 4
- Reputation Fragility: 2
- Legal / Regulatory Exposure: 1
- Psychological Destabilization Risk: 2
- Integration Burden: 1

### Composite read
- Raw Potency: moderate-high
- Strategic Usefulness: very high
- Risk Load: moderate

### Notes
One of the cleanest hierarchy mechanics; shadow risk is humiliation/caste logic.

---

# 9) How to use this system across the corpus

For each target packet, identify and rate:
- its 3–7 strongest mechanics
- its ritual stack
- its operator-producing structures
- its highest-risk shadow mechanics

Then compare across targets.

Questions to answer:
- which mechanics are highest-potency overall?
- which are best for durable retention?
- which produce operator layers most reliably?
- which scale best?
- which create the most danger relative to value?
- which are healthy-control mechanics versus dark-intensity mechanics?

---

# 10) Suggested next artifact

Using this rubric, build:
- `movement-mechanics-matrix-v0.md`

Columns:
- mechanic
- target examples
- raw potency
- strategic usefulness
- risk load
- best use
- failure mode

---

## Bottom line

A mechanic should never be rated with one number.

The real question is always:
- what force does it create,
- how durable is that force,
- how scalable is it,
- and what kind of shadow comes attached.
