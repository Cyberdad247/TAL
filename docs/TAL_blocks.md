# Structuring AI Thinking: A Categorized Guide to Blocks and Axes in TAL

* Analogy: A housewife hunting for discounted grocery items

---

# Table of Contents

- [z_axis](#z_axis)
  - [Structure](#structure)
  - [Function](#function)
  - [Experience](#experience)
  - [Contextual](#contextual)
  - [Temporal](#temporal)
- [ghost_axis](#ghost_axis)
- [vector_axis](#vector_axis)
- [evaluation](#evaluation)
  - [Stability](#stability)
  - [Impact](#impact)
- [About the `note` field](#about-the-note-field)

---

## z\_axis

The syntactic backbone that designs the **form and flow of thought**

---

### Structure

**Definition:**
The axis that evaluates the **structural form and skeleton** of thought and output. It governs hierarchy, branching, iteration — in short, the shape and assembly of reasoning.

**Analogy:**

* Thinking through fridge inventory to map out meal → shopping list → store route.
* For example: “I’ve got leftover vegetables — I’ll do a stir-fry, and I’ve got tofu, so miso soup too.”

```json
"z_axis": {
  "Structure": {
    "values": ["Procedural planning", "Fridge check → Meal design → Store route"],
    "note": "A logical design process that organizes steps based on existing resources and desired outcomes."
  }
}
```

**When to use:**

* When defining explicit thought frameworks
* For hierarchical or complex data structures

**Risks:**

* Deep recursion and complex branching can cause runaway loops
* Over-structuring may weaken content quality

---

### Function

**Definition:**
Evaluates **“what the AI is supposed to do”** — the operational purpose and effect of the prompt.

**Analogy:**

* Decisions like “prepare dinner for the family” or “save money” that shape shopping and cooking behavior
* “Everyone’s home today, so meals should be nutritious and filling.”

```json
"z_axis": {
  "Function": {
    "values": ["Goal-driven cooking", "Prioritizing volume and health"],
    "note": "A backwards design approach where tasks are shaped by explicit objectives."
  }
}
```

**When to use:**

* To clearly define what AI is meant to accomplish
* For action planning and operational thought flows

**Risks:**

* Over-prioritizing function can suppress context and structure
* Abstract goals may lead to ambiguity

---

### Experience

**Definition:**
Evaluates **“accumulated knowledge and patterns”** — past experiences, memories, heuristics.

**Analogy:**

* Using prior data like “Tuesday veggies go on sale” or “last evening, that shelf had 30% off” to optimize decisions.

```json
"z_axis": {
  "Experience": {
    "values": ["Day-based discount memory", "Behavior shaped by sell-through patterns"],
    "note": "Decision structures informed by historical data and environmental repetition."
  }
}
```

**When to use:**

* When reusing known templates or stable knowledge
* For reliable or memory-dependent outputs

**Risks:**

* Excessive reliance on past patterns may limit innovation
* Outputs may feel outdated

---

### Contextual

**Definition:**
Evaluates **“situational awareness”** — adapting to background, timing, and present conditions.

**Analogy:**

* Adjusting plans if it’s raining, the store is crowded, or shelves are picked over
* “It’s raining, maybe discounts come later. It’s a holiday — it’ll be packed.”

```json
"z_axis": {
  "Contextual": {
    "values": ["Discount delays due to weather", "Change shopping priority based on store conditions"],
    "note": "Responsive reasoning based on real-time environmental shifts."
  }
}
```

**When to use:**

* Mid-conversation flexibility
* Improvised or dynamic response handling

**Risks:**

* Misread context leads to irrelevant outputs. e.g., misinterpreting a joke as literal leads to nonsense
* Ambiguity increases risk of derailment

---

### Temporal

**Definition:**
Evaluates **“time-based progression and sustainability”** — how outputs evolve or repeat over time.

**Analogy:**

* Situating shopping within weekly meal cycles or planning ahead for busy days
* “These are discounted for today, but I’ll need prep items for tomorrow’s lunch.”

```json
"z_axis": {
  "Temporal": {
    "values": ["Meal planning synced with week’s timeline", "Sustainable use of discounted goods"],
    "note": "A timeline-aware design that ensures logical flow across time steps."
  }
}
```

**When to use:**

* For dynamic task scheduling
* For time-sequenced prompt design

**Risks:**

* Infinite loops
* Temporal mismatches

---

## ghost\_axis

**The emotional and symbolic stratum**

**Definition:**
Evaluates **“invisible or unspoken influences”** — latent intent, emotional undercurrents, symbolic hints.

**Analogy:**

* “Feels like someone in the family needs cheering up — let’s get their favorite dessert.”
* “This miso feels... comforting, for some reason.”
* Like choosing candles for a dinner — not because of necessity, but because it ‘sets the right mood.’

```json
"ghost_axis": {
  "values": ["Intuitive choices", "Pursuit of emotional satisfaction"],
  "note": "When decisions are shaped by atmosphere, emotions, or invisible factors rather than logic. For example, choosing pudding not for nutrition, but because 'it just feels right today.'"
}
```

**When to use:**

* To extract latent needs
* For risk perception or affective patterning

**Risks:**

* Over-interpretation may derail reasoning
* Risk of reading too much into irrelevant signals

---

## vector\_axis

**Quantitative evaluation through semantic polarity**

**Definition:**
Measures **“contrast between opposing concepts or criteria”** — using semantic vectors to evaluate decision trade-offs.

**Analogy:**

* Weighing “50% off but expires today” vs “30% off, good for 2 more days”
* “Is it really a deal if it spoils before I use it?”

```json
"vector_axis": {
  "Discount vs Expiry Risk": {
    "note": "A frequent decision tension in domestic life: cost-saving vs food safety. This trade-off reflects opposing value vectors — economic efficiency vs health consciousness.",
    "semantic_similarity": {
      "value": 0.36,
      "note": "Scale ranges from 0.0 (unrelated) to 1.0 (identical). A score of 0.36 indicates partial relevance but fundamental difference in nature."
    },
    "opposition_strength": {
      "value": 7,
      "note": "Scale of 1 to 10. A 7 reflects high impact on choice structure — this trade-off strongly affects decisions."
    },
    "meaning_projection": {
      "value": ["Economic rationality", "Food sustainability"],
      "note": "This opposition projects across multiple meaning domains — saving money, reducing waste, and staying safe."
    }
  }
}
```

**When to use:**

* For risk balancing, safety tuning, threshold evaluation

**Risks:**

* High scores may overamplify differences
* Low scores may yield weak or flat outputs

---

## evaluation

**Assessing output stability and long-term impact**

---

### Stability

**Definition:**
Evaluates **“system stability and risk of runaway behavior”**

**Analogy:**

* Avoiding overbuying by considering fridge capacity, budget, and shelf life
* “If I buy too much, it’ll spoil — and we’ll be over budget.”

```json
"evaluation": {
  "Stability": {
    "values": ["Avoid overbuying", "Sustain nutritional and financial balance"],
    "note": "Design mechanisms that prevent recursive overflow or behavioral collapse. Think: ‘Can this routine continue sustainably?’"
  }
}
```

**When to use:**

* Long-running AI systems
* Recursive structures requiring self-limiting design

**Risks:**

* Instability leads to prompt failure
* Overstabilization limits creativity

---

### Impact

**Definition:**
Evaluates **“the downstream effects of output on memory, behavior, or system state”**

**Analogy:**

* “What I buy today shapes tomorrow’s meals — or clogs the fridge.”
* “Buying these now means I won’t need them next week.”

```json
"evaluation": {
  "Impact": {
    "values": ["Fridge capacity impact", "Mid-term meal planning consequences"],
    "note": "Anticipates the ripple effect of a choice — how it affects future outputs, logic flow, or stored state."
  }
}
```

**When to use:**

* For persistent state modeling
* When memory-aware reasoning is required

**Risks:**

* High-impact choices may create runaway effects
* Low-impact choices may feel forgettable

---

## About the `note` field

The `note` is not just a comment. It’s a **semantic safety net**.

It prevents interpretive drift, suppresses collisions between axes (especially ghost/contextual), and helps align structural intent.
It also improves cross-LLM compatibility — ensuring TAL blocks can be meaningfully interpreted by different models.
For this reason, **TALC should always output the `note` field for every axis block.**

