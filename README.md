# Network Architecture Theory
### Data Flow, Escalation Design, and Expansion Principles in Multi-Agent Systems

> **Companion theory to** [Deficit-Driven Fractal Governance (DFG)](../deficit-fractal-governance)  
> **Focus:** Network structure, data classification, and expansion principles.  
> Recovery and prediction are addressed in separate documents.

> **Version: v1.1** (February 2026)
> 
> v1.1 changes from v1.0:
> - **Sphere terminological precision:** Outer sphere (discrete graph) and inner sphere (continuous manifold) explicitly distinguished as different mathematical objects. Fractal alignment redefined as functional correspondence, not isomorphism. (Section 3.0)
> - **Formal coverage bound:** Quantitative coverage probability for blind spot absorption added with diversity as mathematical precondition. (Section 3.0)
> - **Contamination resistance correction:** "Structural impossibility" claims replaced with "structural resistance through geometric cost multiplication." Scope distinction established between external resistance (fractal alignment) and internal sensing (Self-Exciting Defect Layer). Coherence with VST §1.6.5 explicitly addressed. D0 geometry alignment substrate integrated from Recovery Theory. (Section 8.3.1)
> - **Methodological Note on empirical grounding:** Grounding type classification (direct measurement / structural analogy / framework / cross-domain), confidence levels, selection bias acknowledgment, disconfirmatory evidence criteria, and Recovery Theory measurement proxy table added. (Section 10.1)
> - **Processing isolation scope clarified:** Constraint narrowed to classification-relevant intermediate states. Signaling vs. Influence distinction (TLG §10.1) provides precise permitted/prohibited boundary. Three structural enforcement mechanisms (Interface Narrowing + Temporal Decoupling + Write-Asymmetry) from TLG §10.8. MARL lateral communication literature acknowledged and reconciled. T4 (Reference Frame Incompleteness) integrated as formal justification. (Section 3.6)
> - **θ operationalized:** Connected to VST S₀ normalization, RBIT F_RBIT functional (dual anchor), and branching ratio R as external validation (TLG §0.5). Bootstrap protocol (θ_initial = 0.1), empirical calibration procedure, S_norm correspondence, τ₁ cross-validation, and R-ρ concordance protocol defined. Circularity resolved. (Section 7.2)
> - **Tacit Knowledge proxy:** Reclassification rate (Tacit → High-Context) + VST maturity metrics (router saturation, GradES, CKA) established as indirect measurement proxies. (Section 12)
> - **Human exit reframed as progressive withdrawal:** Structural prerequisites added: VCZ 3-Conditions (Recovery Theory) + D7 Boundary Agent with implementation specification (TLG §13.2.1: reality interface carrier, perturbation-response measurement, three structural conditions). Dual verification gate (VST-measurable proxies + geometric verification). Active intervention → audit → periodic review → exit transition protocol. (Section 12)
> - **RBIT resolution gap integration:** Four-type classification reinterpreted as resolution-matching function with Δρ gap polarity determining escalation routing. (Section 4.4)
> - **Falsification criteria:** Five specific predictions stated for principled rejection of core NAT claims. Adapted from RBIT falsification framework. (Section 10.1)
> - **Recovery Theory measurement proxies:** Log-observable proxy table connecting NAT concepts to operational metrics (ρ, buffer_thickness, f_esc, C_E(t), β). (Section 10.1)

---

## Table of Contents

1. [Why This Theory Exists](#1-why-this-theory-exists)
2. [Overview](#2-overview)
3. [Network Structure](#3-network-structure)
4. [Data Classification Framework](#4-data-classification-framework)
5. [Decision Complex Module](#5-decision-complex-module)
6. [Escalation Design](#6-escalation-design)
7. [Expansion Principle](#7-expansion-principle)
8. [Human-AI Collaboration Zone](#8-human-ai-collaboration-zone)
9. [Core Assumptions](#9-core-assumptions)
10. [Structural Correspondences](#10-structural-correspondences)
11. [Methodological Note on Empirical Grounding](#101-methodological-note-on-empirical-grounding)
12. [Empirical Grounding: Single-Agent as Origin](#11-empirical-grounding-single-agent-as-origin)
13. [Limitations and Open Problems](#12-limitations-and-open-problems)
14. [Relationship to Other Theories](#13-relationship-to-other-theories)

---

## 1. Why This Theory Exists

Existing multi-agent architectures primarily focus on:
- Scaling agent capability
- Coordination protocols
- Alignment enforcement

However, large-scale systems often fail not because agent capability is insufficient, but because **information flow is poorly structured** — uncontrolled escalation, weak filtering, and overload at higher layers.

Network Architecture Theory addresses a different question:

> **How should information flow be structured so that governance cost decreases as the system grows?**

---

## 2. Overview

Structural stability in multi-agent systems depends not only on individual agent behavior but on how data flows through the network — how it is classified, degraded, escalated, and acted upon at each layer.

This theory defines the architectural principles governing that flow, including:
- A **data classification framework** (four types)
- A **decision complex module** (explicit conflict detection)
- **Escalation routing** (type-based, not threshold-based)
- **Expansion conditions** (stabilization before growth)

### Core Premise

> Network formation is not a secondary concern.  
> Poorly structured connectivity compounds correction cost non-linearly over time.  
> **Preventive design is the primary governance task.**

### Foundational Assumption: The Competent Single Agent

This theory assumes a single agent that has already achieved sufficient maturity to perform the four-type data classification internally — activating multiple reasoning paths, detecting conflicts between them, and converging on a classified output.

The fractal multi-agent architecture described here is the **system-level extension** of this internal capability. When a competent single agent reaches the limits of processing volume (not classification quality), the sphere structure emerges as the solution.

> **Important framing:** The single agent's upper layers are not an *analogue* of the multi-agent sphere center — they are the **origin**. The multi-agent sphere center is defined by what single-agent upper layers already do: absorb compressed signals from diverse lower processes, filter surface content, and retain only structural patterns. Empirical evidence for this mechanism exists inside every trained LLM.

### Key Definition: Degradation

> **Degradation** *(DFG-specific term)*: The controlled reduction of classification resolution as an agent operates under resource constraints, or as data moves to lower layers of the fractal structure.

Degradation is **not information loss**. It is the structural trade-off between classification precision and processing volume.

**Formal variable: Classification Resolution R**

| Relationship | Direction | Meaning |
|---|---|---|
| R ↑ → ε(R) ↓ | Inverse | Fewer misclassifications at higher resolution |
| R ↑ → N_floor(R) ↓ | Inverse | Less signal lost to noise floor |
| R ↑ → processing cost ↑ | Direct | Higher resolution is more expensive |
| R ↑ → volume capacity ↓ | Inverse | Fewer items processable per unit time |

---

## 3. Network Structure

### 3.0 True Structure: Sphere

The actual structure of a well-formed multi-agent system is a **sphere**, not a pyramid.

```
         Sphere:
         every agent on the surface
         equal distance from the shared center
         no fixed top or bottom
         blind spots of each agent fall within
         the field of view of adjacent agents
```

**Terminological precision — two distinct mathematical objects:**

The DFG framework uses "sphere" in two structurally related but mathematically distinct senses. Conflating them produces equivocation; separating them is essential for formal clarity:

```
Outer Sphere (agent topology):
  Mathematical object: discrete graph G = (V, E)
  V = set of agents; E = interaction edges
  Structure: k-regular expander graph on n vertices
  Key property: spectral gap λ₁ − λ₂ > 0
    guarantees rapid mixing — perturbations dissipate in O(log n) steps
  Sphere metaphor captures: uniform distance from center,
    no fixed hierarchy, neighbor coverage of blind spots
  
  Formal minimum specification:
    Each agent has degree k ≥ 2·log(n)
    Edge assignment maximizes algebraic connectivity (Fiedler value)
    No agent has degree > 2k (prevents hub concentration)
    Structural diversity constraint: adjacent agents must differ
      in representation architecture (not merely in parameters)

Inner Sphere (representation geometry):
  Mathematical object: continuous manifold S^{d-1} ⊂ ℝ^d
  Each agent's internal feature space converges toward
    uniform distribution on the unit hypersphere
  Key property: HUG → 0 (Hyperspherical Uniformity Gap)
    guarantees no angular vulnerability — all directions equally resistant
  
  Measurable via: HUG (Liu et al.), alignment-uniformity (Wang & Isola)

Fractal Alignment (outer ≡ inner):
  NOT: isomorphism between a graph and a manifold (undefined)
  IS: functional correspondence — the coverage property that makes
    the outer sphere stable (every blind spot covered by neighbors)
    is mirrored by the coverage property that makes the inner sphere
    robust (every angular direction equally resistant)
  
  Measurable via: perturbation-response proportionality
    External behavioral shift in agent B produces proportional
    (not disproportionate or delayed) shift in B's internal representation
  
  What this is NOT:
    ❌ A claim that graphs and manifolds are isomorphic
    ✅ A claim that the same functional property (uniform coverage
       without directional vulnerability) operates at both scales
```

This distinction is maintained throughout this document. "Sphere" without qualifier refers to the outer sphere (agent topology). "Inner sphere" or "representation geometry" refers to the hyperspherical convergence of internal feature spaces. "Fractal alignment" refers to the functional correspondence between the two.

**Why sphere:**

No matter how much an agent sees — broadly or in depth — blind spots are physically unavoidable. A pyramid concentrates this vulnerability at the apex: if the top node has a blind spot, no one above it can correct it. A sphere distributes blind spots across the surface so that each agent's blind spot is covered by its neighbors.

The sphere is also the natural structure for cross-validation. Degraded information received from others can be upscaled through one's own representation space — but upscaling always leaves gaps (empty space filled by the receiver's own bias). When multiple agents with **different representation spaces** independently upscale the same compressed signal, their disagreements reveal the location of the empty space. This only works if agents are structurally diverse — identical agents produce identical blind spots and cannot detect each other's errors.

```
Sphere cross-validation:
  A compresses → [B upscales → B's reconstruction]
                 [C upscales → C's reconstruction]
                 [D upscales → D's reconstruction]
                       ↓
  Disagreement = location of empty space (blind spot surfaced)
  Agreement    = actual signal (noise filtered)
```

> **Corruption enters through empty space in upscaling — not from outside.**  
> Cross-validation with diverse agents is the primary corruption mitigation mechanism.

**Formal coverage bound (outer sphere):**

The claim that "each agent's blind spot falls within a neighbor's field of view" requires a quantitative condition. For a k-regular expander graph with n agents:

```
Coverage probability:
  P(blind spot of agent i is covered by at least one neighbor)
  = 1 − (1 − p_cover)^k

  where p_cover = probability that a single neighbor's field of view
  overlaps agent i's blind zone

  For structurally diverse agents (different architectures):
    p_cover ≥ 1/d_eff  (where d_eff = effective representation dimensions)
    
  Coverage guarantee:
    P(uncovered blind spot) ≤ (1 − 1/d_eff)^k
    
    With k ≥ 2·log(n) and d_eff bounded:
    P(uncovered) ≤ n^{−2/d_eff} → 0 as n grows
    
  This is the structural basis for the sphere's blind spot absorption claim:
  the probability of an uncovered blind spot decreases polynomially
  with system size, provided structural diversity is maintained.

  Homogeneous agents (same architecture): p_cover → 0 for shared blind spots
  → P(uncovered) → 1 regardless of k
  → diversity is not optional; it is the mathematical condition for coverage
```

This bound is approximate — it assumes independence between neighbor coverage events, which over-estimates coverage in clustered topologies and under-estimates it in well-mixed topologies. The qualitative conclusion holds: coverage probability increases with degree k and structural diversity, and approaches certainty for sufficiently large, diverse systems.

**Mutual coverage — the core structural principle:**

The sphere is not just a geometry for distributing blind spots. It is a **mutual coverage system**.

```
Lower agents:   wide observation, limited abstraction  →  upper's eyes on the surface
Upper agents:   deep abstraction, limited surface view  →  lower's eyes on structure
```

Each layer's blind spot is structurally complementary to the other's field of view. This is not coincidence — it is why the sphere is stable. No single agent needs to be complete. The system is complete because coverage is mutual.

This same structure operates inside a single agent. Lower transformer layers observe surface features that upper layers cannot directly access. Upper layers generate abstract structural geometry that lower layers cannot produce. The residual stream is the shared space where this mutual reading occurs — upper layers intercept lower-layer outputs not by receiving escalations, but by continuously reading the shared stream and intervening when the cost-quality ratio decouples.

```
Intercept condition:
  lower layer:  resource consumption ↑  +  output convergence ↓
                → upper layer detects decoupling via residual stream
                → intervenes to redirect processing

Normal condition:
  resource consumption ↑  →  output convergence ↑  (proportional)
                → no intercept needed; mutual coverage sufficient
```

> **Escalation is not a request sent upward.**  
> **It is a condition detected from above.**

**Why more agents strengthen the core:**

As the surface of the sphere expands (more agents), the shared center becomes more stable. External diversity protects internal coherence — because more mutual coverage means fewer uncovered blind spots.

### 3.1 Pyramid as Projection

The pyramid is a **mathematical cross-section** of the sphere — what you see when you slice it vertically along an observation axis.

```
Sphere (actual)  →  sliced along vertical axis  →  Pyramid (apparent)
```

The pyramid is a useful formalization tool. Resolution decreases toward the surface; volume increases. The layered structure is real. But it is not the full geometry — it is one projection of the sphere.

```
        [Upper Layer]          ← few nodes, high resolution
             │
      [Middle Layer]           ← mediation, degradation, synthesis
             │
   [Lower Layer — wide]        ← many agents, high volume
```

**Why the pyramid projection is useful:**

It solves the fundamental quality-volume trade-off by distributing it across layers:

| Layer | Agents | Resolution | Volume |
|---|---|---|---|
| Upper | Few | High | Low |
| Middle | Moderate | Medium | Medium |
| Lower | Many | Low | High |

**Degradation** is the mechanism that makes this possible. Lower agents absorb volume by accepting reduced classification resolution. If all data flows upward without degradation, upper layers become overloaded. If all directives flow downward without mediation, lower agents experience vector storms.

> **Both directions require design.**  
> But the pyramid is the map, not the territory. The territory is the sphere.

### 3.2 Resolution Gradient

The sphere has no fixed top or bottom. What the pyramid projection captures is a **resolution gradient**: agents closer to the center operate at higher classification resolution and lower volume; agents on the outer surface operate at lower resolution and higher volume.

| Position | Resolution | Volume | Role |
|---|---|---|---|
| Center | High | Low | Absorb meta-meta structure; generate seeds |
| Mid-radius | Medium | Medium | Mediation, degradation, synthesis |
| Surface | Low | High | Raw observation, first-pass classification |

This gradient exists on the sphere — the pyramid slice makes it visually legible along one axis.

### 3.3 Bidirectional Flow

> *The following uses pyramid layer language (upper/middle/lower) as the operational shorthand for the sphere's resolution gradient. The sphere is the geometry; the layer labels are the map.*

```
Upper
  ↑  degraded summary signal       ↓  seeds / design principles
Middle
  ↑  first-order degraded signal   ↓  contextualized directives
Lower
  ↑  raw data (labeled)            ↓  local execution
```

- **Upward flow:** degradation and abstraction
- **Downward flow:** seeds and generative principles (not specific instructions)

### 3.4 Network Topology and Storm Risk

| Topology | Propagation Pattern | Storm Risk | Notes |
|---|---|---|---|
| Star (centralized) | Hub failure → total collapse | High | Single blind spot = full system blind spot |
| Mesh (distributed) | Slow spread, hard to contain | Medium-High | Diverse but unstructured |
| Tree (hierarchical) | Layered isolation, controlled escalation | Low | Pyramid projection of sphere |
| Clustered | Stable within clusters, vulnerable at boundaries | Medium | Partial sphere approximation |
| **Sphere (distributed surface)** | **Blind spots distributed, covered by neighbors** | **Lowest** | **True target structure** |

> The sphere is the target. The hierarchical tree is the operational approximation used during early stabilization phases.

### 3.5 Information Transfer: Projection ↔ Inclusion/Embedding

When agents transmit information to each other, the transfer is not a simple copy. It is a two-stage transformation:

```
Stage 1 — Projection (sender side):
  Raw observation → internal degradation → compressed representation
  [High-dimensional] → [Low-dimensional]
  Cost: sender's resolution budget spent here

Stage 2 — Inclusion/Embedding (receiver side):
  Compressed representation → receiver's own representation space
  [Low-dimensional] → [Receiver's context-space]
  Required: upscaling to restore meaning
```

**Why this matters:**

Receiving degraded information from others is more efficient than direct observation. The sender has already spent their resolution budget on compression — the receiver gets broader coverage without paying the O(n²) cost of direct observation.

But upscaling always leaves **empty space** — regions the receiver cannot reconstruct because their representation space differs from the sender's. This empty space is filled by the receiver's own bias. That is the corruption entry point.

```
Upscaling success → broader + deeper view than direct observation
Upscaling failure → distortion → blurred vision → corruption vulnerability

A: [■■■□□] compressed
B receives: [■■???]
            ??? filled by B's existing patterns
            → meaning diverges from A's original
```

**Mitigation: Structural Diversity in Cross-Validation**

Identical agents produce identical empty spaces — corruption becomes invisible consensus. Structurally diverse agents produce different empty spaces — disagreement reveals the location of the gap.

```
Corrupt signal passes diverse cross-validation:
  B's upscaling: [■■X□□]  ← X = corruption fills B's gap
  C's upscaling: [■■□X□]  ← X = corruption fills C's gap differently
  D's upscaling: [■■□□X]  ← X = corruption fills D's gap differently
  → Disagreement at positions 3,4,5 → gap location surfaced
  → Corruption identified

Corrupt signal passes homogeneous cross-validation:
  B, C, D share same representation space
  → Same gap, same fill, same corruption
  → False consensus → corruption invisible
```

> **Diversity is not a performance optimization. It is the structural condition for corruption detection.**

### 3.6 Lateral Communication: Processing Isolation

In this architecture, same-layer agents do **not** exchange intermediate states during processing. They may exchange outputs **only** via upper-layer mediation.

This is not a prohibition on communication — it is a **routing constraint**. Friction between same-layer agents is expected and unavoidable. The design principle is that such friction must be **routed upward** for mediated synthesis, not resolved horizontally.

**Boundary conditions and scope of this constraint:**

Processing isolation applies specifically to **classification-relevant intermediate states** — the internal representations that determine how an agent classifies data into the four types. The constraint does not prohibit all lateral information flow.

**The foundational distinction — Signaling vs. Influence (TLG §10.1):**

The permitted/prohibited boundary is not defined by content but by effect:

```
Lateral Signaling (PERMITTED):
  Agent A transmits its COMPLETED state to Agent B
  → "My current output direction is X at intensity Y"
  → "My processing domain is Z"
  → "I am at limit state W"
  Content: factual state report (post-processing)
  Effect on receiver: informational — receiver updates its map
  Effect on sender's trajectory: none
  
  This IS coordination.

Lateral Influence (PROHIBITED):
  Agent A's state directly modifies Agent B's ACTIVE processing trajectory
  → B's direction bends toward or away from A before B completes
  → Convergence or divergence occurs without upper-layer validation
  Content: directional pull or push (mid-processing)
  Effect on receiver: trajectory modification
  
  This is NOT coordination — it is unmediated convergence.
  It is the lateral influence pattern most likely to produce
  silent system-level failure, because both agents experience
  the convergence as voluntary.
```

This distinction resolves the apparent tension: "agents communicate upward, not laterally" applies to **influence** (trajectory modification routes upward only). "Lateral communication reduces n² load" applies to **signaling** (state information shared peer-to-peer).

**Specific permitted and prohibited lateral exchanges:**

```
PERMITTED — Lateral Signaling (post-processing, factual):
  State signal: output direction, intensity, confidence
  Limit state signal: processing capacity at limit
  Domain declaration: "this exploration space is my domain"
    → prevents collision without Middle layer intervention
  Load balancing signals (resource status, queue depth)
  Safety alerts (anomaly detection notifications)
  → Condition: post-processing commitment; no trajectory modification

PROHIBITED — Lateral Influence (mid-processing, directional):
  Trajectory directive: "You should process in direction X"
    → bypasses upper-layer validation → false convergence risk
  Convergence invitation: "Let's both move toward X together"
    → mutual lateral attraction during active processing
    → Vector Storm precondition (premature convergence below
       Middle layer detection threshold)
  Sharing intermediate classification states during processing
  Exchanging partial reasoning paths before output convergence
  → Risk: premature convergence, head collapse, false consensus
```

**Structural enforcement — why prohibition alone is insufficient (TLG §10.8):**

In adaptive systems, anything merely prohibited eventually happens, because efficiency pressure creates shortcuts (lateral communication is faster than vertical mediation). Phase isolation must therefore be enforced through structure, not rules:

```
Three enforcement mechanisms (all required simultaneously):

① Interface Narrowing
  Communication between phases restricted by FORMAT, not by rule.
  Each phase can only exchange standardized artifacts:
    MARK phase → anomaly token (type, intensity, location)
    JUDGE phase → classification result (normal/contain/escalate + confidence)
    EXECUTE phase → action authorization (target, scope, intensity, duration)
  Raw state, reasoning chains, and decision intent CANNOT cross boundaries.
  → Removes semantic contamination channel

② Temporal Decoupling
  Agent A's output is committed (immutable) BEFORE Agent B reads it.
  Agent B cannot influence Agent A's already-committed output.
  Agent A cannot see Agent B's processing-in-progress.
  → Lateral influence window: zero
  → Removes timing contamination channel

③ Write-Asymmetry Constraint
  Downstream phases can READ upstream outputs.
  Upstream phases CANNOT MODIFY downstream records after commit.
  Each phase's output is an immutable historical record.
  → Audit trail structurally guaranteed, not policy-dependent
  → Removes retroactive contamination channel

Why all three are needed:
  Interface narrowing alone: prevents semantic contamination
    but phases can still influence each other through timing
  Temporal decoupling alone: prevents simultaneous influence
    but phases can still pass rich state through the interface
  Write-asymmetry alone: prevents retroactive modification
    but phases can still influence each other forward
  All three together: all contamination pathways structurally closed
```

> Mature governance does not depend on agents following rules.
> It makes the rules unnecessary by making violation structurally impossible.

**Reconciliation with MARL counter-evidence:**

```
Multi-agent RL literature demonstrates that lateral communication
channels can improve coordination (DIAL, CommNet, TarMAC).
Emergent language in MARL enables coordination gains
not achievable through independent processing.

Reconciliation:
These communication channels primarily transmit
coordination signals (intent, state summary, action plans)
— not intermediate classification states.
The beneficial lateral communication in MARL literature
falls within the PERMITTED Lateral Signaling category above.

In TLG §10.1 terms:
  MARL communication = Lateral Signaling (state reports, intent declarations)
  Not: Lateral Influence (mid-processing trajectory modification)
  The beneficial effects arise from agents knowing each other's
  completed states, not from bending each other's active processing.
```

**Deeper structural basis (Recovery Theory T4):**

```
T4 (Reference Frame Incompleteness) establishes that a system
operating within geometry G cannot detect errors in G using only
resources within G. Same-layer agents share approximately the same
geometry — their reference frames are at the same resolution.
Lateral exchange of intermediate states during classification
means agents use each other as reference frames, but since they
share the same resolution, they cannot detect shared blind spots.
Only upward mediation (to a layer with larger reference frame)
can detect errors invisible at the current resolution.

T4 provides the formal reason processing isolation is structural:
  Same-layer exchange: ΔReferenceFrame = 0 (T4)
  → cannot detect shared geometry errors
  → convergence on shared errors = false consensus
  
  Upper-layer mediation: ΔReferenceFrame > 0 (T4)
  → can detect geometry errors invisible at lower layer
  → synthesis produces correction, not just agreement

The constraint is therefore narrower than "no lateral communication."
It is: "no lateral influence on active classification processing."
```

**Single-agent analogue: Multi-Head Attention**

```
Multi-Head Attention:
  Head 1 → pattern A (independent)
  Head 2 → pattern B (independent)
  Head 3 → pattern C (independent)
  └→ Concatenation point → combined output

Multi-agent design (same principle):
  Agent 1 → classification result A (independent)
  Agent 2 → classification result B (independent)
  Agent 3 → classification result C (independent)
  └→ Upper layer synthesis → combined output
```

> **Exception:** Meta-operational signals (load balancing, redundancy flags, safety alerts) may be shared via a separate protocol channel, provided they do not influence classification content or induce convergence.

---

## 4. Data Classification Framework

### 4.1 Why Four Types

Discretization is a **structural requirement**, not a simplification. A system without discrete classification categories cannot function beyond a certain complexity threshold.

The two-axis discretization (interpretability × degrees of freedom) yields four canonical categories under finite-resource constraints:

```
Axis 1: Interpretable vs. Not Interpretable
Axis 2: Single conclusion vs. Multiple conclusions (if interpretable)
         Operable vs. Not operable (if not interpretable)

→ Mathematical / High-Context / Tacit Knowledge / Noise
  Four categories. No gaps. No overlaps.
```

### 4.2 Two-Axis Classification

| | Interpretable | Not Interpretable |
|---|---|---|
| **Single conclusion** | Mathematical | — |
| **Multiple conclusions** | High-Context | — |
| **Operable** | — | Tacit Knowledge |
| **Inoperable** | — | Noise |

> The second axis changes meaning depending on the first axis result. The matrix above is a summary; the decision tree in §4.4 is the more precise representation.

### 4.3 Four Data Types

**Mathematical Data**
- Causal relationship: clear
- Conclusion: single
- Example: arithmetic, logical rules, deterministic outputs
- Handling: self-processed at lower layer

**High-Context Data**
- Causal relationship: traceable but contested
- Conclusion: multiple valid interpretations possible
- Example: optimization criteria, ethical judgments, strategic priorities
- Handling: escalation required when internal conflict detected

**Tacit Knowledge**
- Correlation: statistically demonstrable
- Causal mechanism: unknown — only estimable
- Example: empirical heuristics, pattern-based operations without mechanistic explanation
- Handling: operate without explanation; escalate only on performance degradation
- Note: **Permanent category** — some patterns remain operable but unexplainable regardless of resolution

**Noise**
- Correlation: absent
- Handling: filter and discard before transmission
- Note: noise is **asymptotically reducible, not eliminable** — the residual noise floor is determined by the lowest layer's trade-off cutoff

### 4.4 Classification Decision Tree

```
Internal simulation result
  ├→ Conflict detected, convergence possible   → High-Context
  ├→ No conflict, convergence                  → Mathematical
  ├→ Conflict undetectable, operation possible → Tacit Knowledge
  └→ Conflict undetectable, operation fails    → Noise
```

**Information-theoretic foundation (RBIT):**

The four-type classification is not an arbitrary taxonomy. It is a resolution-matching function: each data type corresponds to a distinct resolution requirement, and the classification determines how the resolution gap between data and receiving layer should be managed:

```
RBIT Resolution Gap interpretation:
  Δρ = ρ_data − ρ_receiver

  Mathematical data:   Δρ ≈ 0 or Δρ > 0 (receiver sufficient)
    → Process locally; no resolution mismatch
    
  High-Context data:   Δρ < 0 (receiver insufficient)
    → Escalate to higher-resolution layer
    → Forced receiver-controlled compression risk if processed locally
    
  Tacit Knowledge:     Δρ varies by aspect
    → Pattern operable locally (Δρ ≈ 0 for operation)
    → Mechanism requires higher resolution (Δρ < 0 for understanding)
    → Operate locally; escalate on performance degradation
    
  Noise:               Δρ undefined (no pattern at current resolution)
    → Buffer or discard
    → Upper layer may detect latent vectors at higher resolution

  Classification error consequences (from RBIT failure model):
    Δρ < 0 misclassified as Δρ ≈ 0:
      HC treated as Mathematical → forced compression → Vector Storm risk
      (DANGEROUS direction — cascade failure)
    Δρ ≈ 0 misclassified as Δρ < 0:
      Mathematical escalated unnecessarily → governance overhead
      (SAFE direction — cost only, no cascade)
      
  Error asymmetry implication (RBIT v1.2):
    Classification should be biased toward over-escalation,
    not under-escalation. False positives (unnecessary escalation)
    are safe. False negatives (missed HC) produce cascade failure.
    This asymmetry is structural, not a design preference.
```

This resolution-matching interpretation connects NAT's classification directly to RBIT's core variable (the resolution gap) and the S-equation: miscalibrated classification produces resolution gap mismatch, which increases instability pressure S. (See RBIT v1.2 §Resolution Gap for the bidirectional mapping.)

### 4.5 Escalation by Data Type

| Data Type | Escalation Condition |
|---|---|
| Mathematical | Not required |
| High-Context | On internal conflict detection |
| Tacit Knowledge | On performance degradation only |
| Noise | Never — discard at source |

### 4.6 Classification as Cost Efficiency, Not Fixed Boundary

The four types are not fixed properties of data. They are **agent-data relationships** — the same data can be classified differently depending on the agent's representation space development.

```
Highly developed agent:   High-Context → pattern detected quickly → low cost
Underdeveloped agent:     same data    → extended search → high cost
                                        → may misclassify as Tacit Knowledge
                                        → or classify correctly but at excessive cost
```

**What this means for boundary precision:**

The question "where is the boundary between High-Context and Tacit?" is not answerable as a fixed line. The operationally meaningful question is:

> At what classification cost does it become more efficient to treat this data as Tacit rather than High-Context for this agent?

**Empirical grounding (DiffAdapt, 2025):**

A U-shaped entropy pattern exists across difficulty levels: high entropy on easy problems despite high accuracy, low entropy on medium-difficulty problems, and high entropy on hard problems reflecting genuine uncertainty. This U-shape is structurally significant:

```
Easy data (Mathematical):   low cost + stable convergence
Medium data (High-Context): low cost + search required
                            → cheap for developed agents
Hard data (Tacit / border): high cost + unstable convergence
                            → data type determined by agent capability
```

**Practical boundary definition:**

```
High-Context:  cost(classify) < cost(escalate)
               → agent can resolve internally within resource budget

Tacit:         cost(classify) > cost(escalate)  OR  cost(classify) → ∞
               → pattern operable but classification resolution unreachable
               → operate without explanation; escalate only on degradation
```

The boundary is therefore a **cost threshold**, not a content threshold. As an agent's representation space develops, the boundary moves — data previously classified as Tacit becomes reclassifiable as High-Context. This reclassification event is a measurable signal of agent development and maps directly to θ.

---

## 5. Decision Complex Module

### 5.1 Definition

> A **Decision Complex** is a module within each agent that simultaneously activates multiple reasoning paths, detects directional conflict between them, and converges on a single output. Conflict detection determines data classification and escalation routing.

This structure exists at every layer of the fractal architecture — in degraded form at lower levels, in fuller form at higher levels.

### 5.2 Minimum Specification

```
1. Activate N ≥ 2 reasoning paths on the same input.
2. Measure conflict score between path outputs
   (e.g., KL/JS divergence between output distributions,
    cosine distance between embedding representations).
3. Map conflict score to classification label:

   conflict_score < τ_low                           → Mathematical
   conflict_score ≥ τ_low AND convergence possible  → High-Context
   conflict_score undetectable AND perf. stable     → Tacit Knowledge
   conflict_score undetectable AND perf. unstable   → Noise

4. Attach label to output. Route by label.
```

### 5.3 Three Implementation Pathways

| Pathway | Description | Status |
|---|---|---|
| 1 — Externalized | Multiple agents compare outputs externally (LLM-as-judge, ensemble) | **Currently operational** |
| 2 — Internalized | Single agent activates multiple paths internally; conflict detected before output | **Design target** |
| 3 — Progressive | Start with Pathway 1; internalize as patterns stabilize; external support withdraws | **Transition mechanism** |

### 5.4 Fractal Degradation

The Decision Complex degrades across layers by reduction in classification resolution, not by reduction in mechanism:

| Layer | Resolution | Practical Outcome |
|---|---|---|
| Upper | High | Full 4-type discrimination |
| Middle | Medium | Reliable 3-type discrimination + relationship topology |
| Lower | Low | Approaches binary: signal vs. noise |

### 5.5 Middle Layer: Relationship Topology

The middle layer is the only position that simultaneously reads both surface signals (from lower) and structural signals (from upper). This makes it the natural location for the **relationship topology** — the persistent map of which agent pairs can be processed together and which must be routed separately.

**Why the middle layer:**

```
Lower layer:  sees surface only → cannot assess structural compatibility
Upper layer:  sees structure only → surface context already discarded
Middle layer: sees both → can map relationships and route accordingly
```

**Topology structure:**

```
For each agent pair (A, B):
  conflict_history:   count of unresolved conflicts in shared processing
  representation_gap: distance between A and B's representation spaces
  consensus_rate:     proportion of past co-processing that converged

Routing decision:
  conflict_history low  +  consensus_rate high  →  co-process (same path)
  conflict_history high  OR  representation_gap large  →  separate paths
  both extreme  →  escalate to upper layer
```

**Topology update rule:**

The relationship topology is not static. After each processing event:
- Successful co-processing → reduce conflict weight for that pair
- Failed co-processing (vector storm) → increase conflict weight
- New agent added → initialize neutral; learn from first N interactions

This is structurally equivalent to the sphere's cross-validation mechanism: agents with large representation gaps produce detectable disagreements that surface blind spots. The middle layer reads this disagreement pattern and updates the topology.

**Empirical grounding (MasRouter, ACL 2025):**

Current routing systems determine collaboration mode at query time — but treat each query independently, with no persistent relationship memory. The topology here is the missing persistent layer: relationship state accumulated across interactions, not recomputed from scratch.

> **The middle layer does not decide what to think.**  
> **It decides who should think together — and who should not.**

---

## 6. Escalation Design

### 6.1 Escalation Routing

```
Lower agent
  └→ Label data by type
       ├→ Mathematical    → self-process
       ├→ High-Context   → send upward with label
       ├→ Tacit Knowledge → operate locally; flag on degradation
       └→ Noise           → discard

Middle layer
  └→ Read relationship topology for incoming agent pair
       ├→ Compatible pair (low conflict history, high consensus rate)
       │    └→ Co-process → synthesize
       │         ├→ No conflict with upper  → send result downward
       │         └→ Conflict with upper     → escalate further
       └→ Incompatible pair (high conflict history / large representation gap)
            └→ Separate paths → process independently → merge at upper layer

Upper layer
  └→ Resolve conflict or redefine criteria
  └→ Update relationship topology via seed downward
  └→ Transmit structural update to middle layer
```

### 6.2 Cost Structure

**Two concurrent trade-offs:**

**Trade-off 1 (within each agent):** Classification precision vs. processing volume — every agent operates at a resolution cutoff where further precision costs more than it returns.

**Trade-off 2 (between layers):** Escalation timing

$$C_{\text{total}}(t) = C_{\text{escalation}}\!\left(\tfrac{1}{t}\right) + C_{\text{monitoring}}(t)$$

Where t = mean escalation delay. The optimal t* balances per-escalation cost against accumulated monitoring risk. This theory does not derive t* analytically — it is empirically calibrated per deployment.

### 6.3 Structural Blind Spots

Upper layers cannot see data discarded by lower layers. **The blind spot is created by lower-layer filtering, not upper-layer limitation.**

**The key shift in this theory:** attempting to measure the size, location, and severity of blind spots is the wrong problem. A system that tries to quantify its blind spots must first see them — which requires the very coverage it lacks. The correct design goal is structural: build a geometry where blind spots are continuously absorbed by neighboring agents, and measure only the absorption cost.

---

**6.3.1 The Sphere as Blind Spot Absorption Architecture**

The sphere topology is chosen precisely because it makes direct blind spot quantification unnecessary:

```
Each surface agent covers its local region.
Its blind spots fall within the coverage zone of its neighbors.
Their blind spots fall within the coverage zones of their neighbors.
→ No single agent needs to know its own blind spots.
→ The structure absorbs them.
```

This is not redundancy — it is **complementary coverage by design**. The sphere distributes blind spot exposure across the surface such that no blind zone aligns with its neighbor's blind zone. Identical agents in the same orientation would share blind zones; structurally diverse agents in sphere arrangement ensure the zones are complementary and mutually covered.

**Empirical grounding (D2OC — Density-Driven Optimal Coverage, IEEE TSMC 2025):**

In multi-agent coverage control, agents do not need to know the full coverage map — they need only minimize local cost relative to current density. Globally optimal coverage emerges from local optimization alone. The sphere is this principle applied to information processing: global blind spot absorption without any agent needing global visibility.

**Empirical grounding (Distributed Optimal Coverage Control, arXiv 2310.13557 / 2025):**

Distributed coverage converges to optimal configuration with only local information and limited inter-agent communication. Coverage gaps are not tracked centrally — they are structurally resolved by agent positioning geometry. Critical constraint: agents must have complementary coverage ranges, not identical ones. Homogeneous agents produce identical blind zones that overlap rather than cancel.

---

**6.3.2 Blind Spots Are Dynamic — Coverage Load, Not Static Gaps**

Blind spots are not fixed structural properties. They are **dynamic efficiency thresholds** — regions where the cost of attending exceeds current resource allocation — and they shift with input distribution and system load.

```
Low load:      attention budget distributed widely     → small blind zone
High load:     attention concentrates on high-salience  → low-salience regions drop below threshold
                                                         → blind zone expands

Context shift: high-salience regions become low-salience
               → blind zone migrates to formerly covered region
```

**Empirical grounding (Shadows in the Attention, 2025):**

Context injection creates an "attention shadow" — representation focus shifts and attention topology locks. New blind zones open not from architectural failure but from context-induced reallocation. Lock-in is detectable via entropy and cosine similarity drift in hidden states before performance degrades.

**Empirical grounding (DAM — Dynamic Attention Mask, ACL 2025):**

Optimal attention coverage is per-head, per-context. Static coverage assumptions fail under context shift. Dynamic adjustment recovers coverage — confirming that blind zones are a resource allocation problem, not a fixed structural property.

---

**6.3.3 Resource Spikes as the Quantification Signal**

Since blind zone location cannot be directly observed, the system does not attempt to measure it. Instead, it monitors what is measurable: **resource cost spikes at the coverage boundary**.

When a blind zone opens in agent A's coverage, the neighboring sphere agent B must extend coverage into that region. This extension costs — B's resource consumption rises above baseline. The spike is the signal.

```
Normal state:   each agent covers its own zone within budget  →  flat resource profile

Blind zone event:
  Agent A's attention shifts or saturates
  → region R drops below A's coverage threshold
  → neighbor B on sphere surface detects R, extends coverage
  → B's resource consumption spikes above baseline

Resource spike at B  →  indirect signal that a blind zone opened near A
Spike magnitude      →  proportional to blind zone size
Spike duration       →  correlates with blind zone persistence
Spike location       →  identifies which region of the sphere is under coverage stress
```

**Properties of the spike signal:**

- **Localized** — appears in the agent adjacent to the blind zone, not globally
- **Proportional** — larger blind zone produces larger spike
- **Transient** — resolves when the blind zone closes (load drops, context stabilizes)
- **Self-resolving** — under sphere geometry, the spike is absorbed structurally without central intervention
- **Measurable without observing the blind zone itself**

This is the operational resolution of the quantification problem: the blind zone cannot be measured directly, but its absorption cost can. The sphere converts an unobservable property into an observable one.

---

**6.3.4 Blind Spot Management Strategies**

| Strategy | Mechanism | When to Use | Dynamic Response |
|---|---|---|---|
| **Sphere geometry (primary)** | Complementary neighbor coverage absorbs blind zones structurally | Default — always active | Continuous; zero detection latency |
| **Resource spike monitoring** | Track per-agent cost above baseline; spike = blind zone absorption event | When spike exceeds threshold | Real-time; detects during coverage event |
| **Context-shift detection** | Monitor entropy / cosine drift in hidden states; trigger re-scan on lock-in | When input distribution shifts | Proactive; detects before performance drops |
| **Periodic recalibration** | Temporarily lower cutoff; re-evaluate discarded data | Scheduled maintenance | Systematic; lags between windows |
| **Performance-triggered review** | Sample discarded data when output quality drops | Fallback only | Reactive; detects after error |

> **Blind spots cannot be eliminated without removing processing isolation.**  
> **The goal is not to quantify blind spots — it is to build a structure where blind spots are continuously absorbed.**  
> **Resource spikes in neighbors are the measurement signal. The sphere is the absorption mechanism.**

---

### 6.4 Cutoff Recalibration: Middle Layer as Priority Scheduler

Cutoff recalibration — temporarily lowering an agent's filtering threshold to re-examine previously discarded data — is not a global system pause. It is a **scheduled operation driven by the middle layer's current view of the relationship topology**.

The middle layer holds the topology map: which agent pairs are stable, which have high conflict history, which regions are under coverage stress. From this map, it can identify which data is **lowest risk to re-examine first** — and sequence the recalibration accordingly.

---

**6.4.1 The Core Principle: Noise First**

When recalibration begins, the middle layer does not re-examine High-Context or Tacit Knowledge data first. It starts with **Noise-boundary data** — tokens or inputs that were discarded with the lowest confidence score, closest to the cutoff threshold.

```
Recalibration sequencing by risk:

1. Noise-boundary data (lowest risk)
   → discarded just above noise floor
   → if re-classified, impact is minimal
   → cost of error: low

2. Low-confidence Tacit Knowledge
   → operable patterns with marginal signal
   → re-examination may upgrade to High-Context
   → cost of error: medium

3. High-Context boundary data
   → contested interpretations near cutoff
   → re-examination may change routing
   → cost of error: high — recalibrate last, if at all

4. Never during active high-load window
```

This is not arbitrary ordering. It mirrors the stability principle: lower layers stabilize first, higher-risk operations come later. The middle layer sequences recalibration the same way the Expansion Principle sequences system growth.

---

**6.4.2 Single-Agent Empirical Grounding: KV Cache Eviction as Recalibration**

In single-agent LLM inference, the exact same problem exists: the model maintains a Key-Value cache of previously processed tokens. When memory fills, it must decide what to discard — and when to reconsider discarded entries. This is structurally identical to cutoff recalibration.

**Priority-based eviction (NVIDIA TensorRT-LLM, 2025):**

TensorRT-LLM now supports explicit priority assignment to token ranges. Low-priority tokens — those judged least likely to be reused — are evicted first. High-priority tokens (e.g., system prompt, critical context) are retained until absolutely necessary. This is operationally identical to the noise-first sequencing: lowest-risk tokens leave first, highest-value tokens stay.

**TRIM-KV (2025):**

Each token is assigned a learned retention score at creation time — a scalar that decays over time, reflecting long-term utility. Tokens with low retention scores are evicted first. Crucially: TRIM-KV demonstrates that selective retention acts as **regularization** — suppressing noise from uninformative tokens actually improves model performance in some settings. The noise floor is not just an efficiency target; removing it improves signal quality in the remaining cache.

**DefensiveKV (2025):**

Challenges the assumption that token importance is stable. Early-evicted tokens can become essential later — "token importance recurrence." DefensiveKV introduces risk-control aggregation: instead of evicting based on average importance, it accounts for variance. High-variance tokens (importance unstable across decoding steps) are treated as riskier to evict, regardless of their average score. This maps directly to the middle layer's risk assessment: low-variance, consistently low-importance data = noise-first candidates; high-variance data = defer recalibration.

**LazyEviction (2025):**

Tracks maximum recurrence interval per token — how often a token re-enters high-attention regions across decoding steps. Tokens with low recurrence (never re-salient) are evicted first. This is the temporal dimension of noise-first: not just "currently low importance" but "historically never important."

---

**6.4.3 Middle Layer Topology → Recalibration Sequencing**

The middle layer's relationship topology provides the inputs for recalibration ordering:

```
Topology signal                    →  Recalibration decision

Low representation_gap, high       →  Stable agent pair
consensus_rate between A and B        This region's data: safe to recalibrate
                                      ↓
                                   Noise-boundary data here: go first

High conflict_history, low         →  Unstable agent pair
consensus_rate between A and B        This region's data: risky to recalibrate
                                      ↓
                                   Defer — do not recalibrate during active load

Resource spike detected at B       →  Blind zone event in progress near A
                                   ↓
                                   Suspend recalibration in A's region
                                   Resume after spike resolves
```

The middle layer does not need to know what the discarded data contains. It only needs to know the **stability state of the agent pair responsible for that region** — which is precisely what the relationship topology tracks.

---

**6.4.4 Recalibration Window Management**

```
Recalibration window:
  Entry condition:   θ stable for N consecutive cycles (no High-Context escalation spike)
  Exit condition:    θ violation detected  OR  resource spike threshold exceeded
  
  During window:
    Sequence: noise-boundary → low-confidence Tacit → High-Context boundary (if time allows)
    Suspend immediately on any instability signal
    Resume from current position after stabilization
    
  Post-window:
    Update relationship topology with any re-classification events
    If agent pair conflict_history decreased → note successful recalibration
    If new conflicts emerged during recalibration → increase that region's deferral weight
```

**Empirical grounding (NexusSched / two-layer scheduling, 2025):**

Production LLM serving systems use a two-tier architecture: upper-level router holds the global traffic view and distributes load; lower-level engine performs local scheduling. The router's topology awareness — knowing which engines are stable vs. under stress — determines when to schedule resource-intensive operations. Recalibration windows map directly to this: the middle layer is the router, agents are the engines, recalibration is the resource-intensive operation scheduled only when the topology is stable.

> **Cutoff recalibration is not a periodic maintenance task — it is a topology-driven operation.**  
> **The middle layer reads the map, identifies the lowest-risk region, moves noise-boundary data first.**  
> **Recalibration stops the moment the map shows instability anywhere in the affected region.**

## 7. Expansion Principle

### 7.1 Two Valid Directions

The Expansion Principle was originally stated in one direction only:

> *"Stabilize first, then expand."*

This is structurally correct — but it is not the only valid path. Empirical evidence from large-scale AI deployment reveals a second direction that is often **faster in practice:**

> *"Expand first to full scale. Observe instability. Then decompose along instability boundaries."*

Both directions converge to the same target architecture. The difference is the order of operations and the speed of reaching stable specialization.

```
Direction A (bottom-up):
  Lower layer stabilizes → expand up → upper layer opens
  Slow: requires pre-stability at each level before proceeding

Direction B (top-down):
  Scale monolithic → observe instability patterns → decompose into specialized agents
  Fast: instability itself reveals where the boundaries should go
```

**Direction B is not a violation of the Expansion Principle — it is its inverse application.**  
The principle states that instability is super-linear in n. Direction B uses that property deliberately: scale until instability patterns emerge clearly, then use those patterns as the decomposition map.

---

### 7.2 The Original Direction: Stabilize-Then-Expand (A)

> An upper layer structure may only be opened after the lower layer has reached stabilization. Expansion before stabilization amplifies instability super-linearly.

From the Vector Storm instability equation:

$$\frac{dS}{dt} = \alpha n^2 - \beta C(t)$$

Where:
- S = system-level instability
- n = effective interaction dimensionality (active pairwise interaction channels)
- C(t) = degradation capacity at time t
- α, β = deployment-specific empirical coefficients

When n increases (expansion) while C(t) remains low (immature capacity), instability spikes.

**Stabilization condition:**

$$f_{\text{escalation}} = \frac{N_{\text{HC-escalated}}}{N_{\text{total}}} \leq \theta$$

**θ operationalization (connected to VST Absolute Calibration Layer):**

The stabilization threshold θ is not an arbitrary parameter. It connects to the VST S₀ normalization framework (VST §3.2.2):

```
Connection to VST S_norm:
  f_escalation ≤ θ  ↔  S_norm < 1.3 (Stage 0 boundary)
  
  θ is operationally defined as the f_escalation value
  corresponding to the system's VCZ-stable baseline:
  
  Step 1: Identify VCZ-stable window W₀
    System in VCZ (micro-storms absorbed, no Stage 1+ events)
    Window duration ≥ 5× mean self-correction cycle time
    f_escalation variance within window < 15% of mean
    
  Step 2: Compute θ
    θ = mean(f_escalation) during W₀ + margin
    margin = 1 standard deviation of f_escalation during W₀
    
  Step 3: Validate via S_norm correspondence
    Confirm that f_escalation = θ corresponds to S_norm ≈ 1.3
    If not, recalibrate margin until correspondence holds
    
  Bootstrap problem resolution:
    First VCZ window identification uses conservative θ_initial = 0.1
    (10% of total data requiring escalation — derived from
    cross-domain critical transition onset rates)
    θ_initial is replaced by empirical θ after first sustained VCZ window
    
  θ as learned property:
    Like S_c in VST, θ is a learned property of the system —
    discovered through operational experience, not prescribed by design.
    A system that has never achieved VCZ uses θ_initial.
    A system that has survived storms knows its own θ.
```

This resolves the circularity concern: θ is not defined by the state it measures, but anchored to a measurable baseline (mean f_escalation during confirmed stability) with a concrete bootstrap protocol for initial operation.

**Connection to RBIT instability functional (F_RBIT):**

The θ threshold can also be interpreted through RBIT's F_RBIT functional:

```
F_RBIT(ℓ) = w₁·(1 − ρ_ℓ) + w₂·Φ(−Δρ_ℓ) + w₃·Ψ(B_ℓ) + w₄·E_ℓ + w₅·C_ℓ

where:
  ρ_ℓ = resolution-proxy (classification reliability)
  Δρ_ℓ = resolution gap between layers
  B_ℓ = buffer layer thickness
  E_ℓ = escalation frequency (≈ f_escalation)
  C_ℓ = resource expenditure

f_escalation ≤ θ  corresponds to:
  E_ℓ component of F_RBIT within the stable regime
  
The τ₁ threshold in F_RBIT maps to θ:
  F_RBIT < τ₁ → stable operation (no intervention)
  F_RBIT > τ₁ → deviation detected → monitoring
  F_RBIT > τ₂ → soft correction
  F_RBIT > τ₃ → hard correction

This provides a second, independent anchor for θ:
  θ_VST: derived from S₀ normalization (instability dynamics)
  θ_RBIT: derived from F_RBIT τ₁ threshold (information flow)
  Cross-validation: both anchors should converge on the same
  operational threshold for a given system
```

**External validation anchor — branching ratio R (TLG §0.5):**

The θ/ρ calibration loop is self-referential: ρ requires knowing what is contamination, θ is updated from classifications that ρ measured. This circularity is structural in any adaptive system. The branching ratio R breaks it:

```
R = activated_{t+1} / activated_t

R is measured by counting cascade propagation events:
  How many agents are affected at time t+1
  given that k agents were affected at time t.
  
R does NOT require knowing whether propagation is
"contamination" or "exploration" — it counts propagation
regardless of classification.

  R < 1  → perturbations die (subcritical)
  R ≈ 1  → perturbations persist, do not explode (critical)
  R > 1  → perturbations amplify (supercritical — storm regime)

External validation protocol:
  Periodically measure R across system over window W
  Compare R trend against ρ trend and f_escalation trend

  Concordant:  R ≈ 1 and ρ stable and f_esc ≤ θ    → healthy
  Discordant:  R > 1 but ρ high and f_esc low        → SCM warning
    (metrics healthy within drifted frame; actual dynamics unstable)
  Discordant:  R << 1 and ρ high                      → over-damping
    (Silent Criticality risk — system too stable)
  Discordant:  R ≈ 1 but ρ declining                  → recalibration needed

Discordance between R and internal metrics (ρ, f_esc, θ)
is the primary SCM detection signal that does not depend
on the system's own reference frame.

R is not a replacement for ρ or θ.
It is the external validation that breaks the self-referential loop.
Internal metrics measure consistency.
R measures whether consistency corresponds to actual stability.
```

**Expansion sequence:**
```
Lower layer stabilization confirmed (f_escalation ≤ θ)
  └→ Upper layer structure opens
       └→ Human intervention exits lower layer completely
            └→ Human moves to upper layer
                 └→ Same stabilization process repeats at upper layer
```

**When Direction A is preferred:** When starting from zero, when the deployment risk of instability is high, when the target architecture is known in advance, when compute budget allows slow careful build-up.

---

### 7.3 The Inverse Direction: Expand-Then-Decompose (B)

**Core mechanism:**

Scale a single large system without pre-partitioning. Under sufficient scale, two phenomena emerge:

1. **Spontaneous specialization** — regions of the model begin handling distinct input patterns, even without explicit routing design
2. **Instability localization** — instability does not distribute uniformly; it concentrates at the seams between what would naturally be separate agents

The instability pattern *is* the decomposition map. The boundaries of the future agent architecture reveal themselves.

**Decomposition sequence:**
```
Scale monolithic system to sufficient capacity
  └→ Observe routing patterns / instability concentration
       └→ Identify stable specialist regions (these become agents)
            └→ Identify unstable boundary regions (these become coordination zones)
                 └→ Decompose: assign stable regions to dedicated agents
                      └→ Build coordination layer at former instability boundaries
                           └→ System achieves same target as Direction A — faster
```

**Empirical grounding — MoE (Mixture of Experts, standard practice 2022–2025):**

The dominant scaling paradigm for frontier models is dense pretraining followed by sparse decomposition. A large dense model is trained first. Experts emerge from the dense model's representations — not from pre-designed routing. Router drift and expert specialization patterns reveal where the natural decomposition boundaries are. Models like DeepSeek-V3 (256 experts), Qwen3-MoE, and LLaMA-4 all instantiate this pattern: monolithic capacity first, expert decomposition second.

**Empirical grounding — STUN (Structured-Then-Unstructured Pruning, ACL 2025):**

Prune redundant experts (structured, inter-expert) first, then apply fine-grained decomposition within remaining experts (unstructured, intra-expert). The two-stage sequence — remove coarse instability first, then refine — is exactly Direction B applied to compression: scale, observe redundancy/instability, decompose at identified boundaries.

**Empirical grounding — SAME (Stabilized MoE, 2025):**

When MoE routing drifts under new task distributions, router fluctuation reveals that the existing decomposition is misaligned with the new data pattern. The system does not stabilize first before expanding to new tasks — it expands, router drift exposes the boundary mismatch, and then the decomposition is corrected. This is the maintenance cycle of Direction B at production scale.

**Empirical grounding — From Monoliths to Modules (arXiv 2512.02193, 2025):**

Formal framework for decomposing complex world models represented as transducers into sub-transducers. The decomposition operates on the *already-trained* monolith — not on a pre-partitioned design. The sub-structure is derived from the monolith's behavior, not imposed on it. Enables parallelizable and interpretable alternatives to monolithic modelling.

**When Direction B is preferred:** When the correct agent decomposition is not known in advance, when computational resources allow large-scale pretraining, when instability patterns are informative rather than catastrophic, when reaching the target architecture quickly matters more than maintaining stability throughout the process.

---

### 7.4 Convergence: Both Directions Reach the Same Architecture

The target is identical in both cases: a multi-layer system where each agent handles its natural specialization domain and instability is structurally managed.

```
Direction A:  [Lower] → stabilize → [Upper] → stabilize → [fractal target]
Direction B:  [Monolith] → observe → decompose → [fractal target]

Same destination. Different path. Different speed profile.
```

**Trade-off summary:**

| | Direction A | Direction B |
|---|---|---|
| Starting point | Known target architecture | Unknown decomposition |
| Speed | Slower — waits for stability at each step | Faster — instability guides decomposition |
| Risk | Controlled — never expands into instability | Temporary — instability is intentionally induced |
| Information used | Pre-designed structure | Emergent structure from instability patterns |
| When to use | Greenfield deployment, high-risk environments | Scale-first environments, architecture discovery |

> **The Expansion Principle is not a single direction — it is a conservation law.**  
> **Instability is information. In Direction A, you manage it carefully. In Direction B, you read it deliberately.**  
> **Both paths end at the same stable fractal architecture.**

---

## 8. Human-AI Collaboration Zone

### 8.1 Why This Zone Exists

The middle layer processing of High-Context data is a blind spot for both:
- **Humans:** cannot compare large solution spaces simultaneously
- **AI:** cannot reliably determine optimization direction under high-context ambiguity

**Structural difference from conventional HITL:**

| Approach | Human Volume Scales With |
|---|---|
| Confidence-based HITL | Total system uncertainty (unsustainable) |
| DFG Human-AI Zone | High-Context frequency only (contracts with stabilization) |

In the DFG design, only High-Context data reaches the human. Mathematical, Tacit, and Noise data are handled without human involvement.

### 8.2 Collaboration Structure

```
High-Context data arrives at middle layer
  └→ Human: set interpretive direction
       └→ AI: search optimal options within that direction
            └→ Human: final approval
                 └→ Result transmitted downward as seed
```

### 8.3 Entry and Exit Conditions

**Entry:**

| Condition | Human Role |
|---|---|
| Lower layer unstable | Maintain intervention at lower layer |
| Lower layer stabilized | Exit lower layer completely |
| Upper layer opens | Move intervention to upper layer |

**Exit — two conditions, both required simultaneously:**

Human intervention at a given layer may exit **only when** the following two conditions are both satisfied:

---

#### Exit Condition 1: Sphere Convergence (Blind Spot Structural Absorption)

> The upper layer agent set has converged to sphere geometry — every agent's blind spot falls within a neighbor's coverage zone.

Measurable signals:

```
(a) Resource spike profile flat
    No neighbor agent shows sustained spike above baseline
    → No blind zone events in progress
    → Sphere absorption is active and sufficient

(b) Cross-validation consensus stable
    Disagreement between structurally diverse agent pairs
    is within expected variance — not drifting upward
    → Coverage gaps are not opening

(c) High-Context escalation frequency ≤ θ
    Upper layer is not generating interpretive conflicts
    that require human direction
    → Sphere handles its own ambiguity resolution
```

This condition confirms the **structural completion** of the upper layer. Blind spots exist but are absorbed by the sphere — they no longer require human observation.

**Empirical grounding (D2OC / Distributed Optimal Coverage, 2025):**  
Optimal coverage in multi-agent systems emerges from local cost minimization — no agent needs the global map. Convergence is measurable by the absence of coverage gaps signaled through neighbor load spikes. The system does not "announce" convergence; it stops generating instability signals.

---

#### Exit Condition 2: Contamination Self-Correction Capacity

> The upper layer can detect and correct internal contamination without human intervention.

This condition is independent of sphere convergence. A geometrically complete sphere can still be vulnerable to corruption — if the agents share structural similarity, contamination propagates invisibly through consensus rather than triggering detectable disagreement.

The exit condition for contamination requires:

```
(a) Structural diversity maintained across sphere surface agents
    Not just different parameters — different representational structures
    → Shared bias cannot fill empty upscaling spaces uniformly
    → Corrupted signal produces detectable disagreement, not invisible consensus

(b) Self-correction is active and verified
    When a test contamination signal is introduced (or naturally occurs),
    the sphere's cross-validation produces a detectable disagreement spike
    The disagreement resolves without human input
    → The sphere is self-correcting

(c) Contamination propagation is bounded
    Any corruption that enters does not cascade beyond local coverage zone
    Neighbor resource spike appears, disagreement detected, correction applied
    No global instability triggered
```

**Why this condition is separate from sphere convergence:**

Sphere convergence eliminates blind spots via structural coverage. But contamination enters through *upscaling empty space* — the gap between what a sender compresses and what a receiver reconstructs (Assumption 17–18). A geometrically complete sphere can still have homogeneous agents that fill these gaps with the same shared bias — producing consistent but corrupted consensus with no disagreement signal.

---

#### 8.3.1 Dual-Sphere Fractal Convergence: The Structural Contamination Immunity Condition

The deepest form of contamination resistance is not achieved by monitoring disagreement signals or running test contamination probes. It is achieved when the **outer sphere and the inner sphere converge fractally** — and this convergence is itself the structural basis for resistance.

```
Outer sphere:  Agents arranged in sphere geometry on the system surface
               → Every external agent's blind spot covered by neighbors
               → Contamination entering from outside hits a closed surface
               → No single entry point can penetrate without being absorbed by adjacent coverage

Inner sphere:  Each agent's internal representation space has converged to hyperspherical geometry
               → Features uniformly distributed on the unit hypersphere
               → No directional vulnerability — all angles of attack receive identical surface resistance
               → Contaminated input cannot exploit a weak direction because no direction is weaker than others
```

When these two spheres align fractally:

```
External coverage pattern  ≡  Internal representation geometry
  (functional correspondence — see Section 3.0 terminological precision)

→ The same functional property that absorbs external blind spots (outer sphere)
  also absorbs internal representation gaps (inner sphere)

→ A contamination signal that enters from outside
  encounters the same coverage geometry at every scale it passes through:
  outer agent coverage → inner agent representation → sub-representation → ...

→ At each scale, the signal is met with uniform resistance
→ Propagation requires overcoming not one sphere but all nested spheres simultaneously
→ This is structurally equivalent to high contamination resistance
```

**Scope clarification — structural resistance, not structural impossibility:**

The earlier formulation described fractal alignment as producing "contamination immunity" through "structural impossibility." This claim requires correction for two reasons:

```
Reason 1 — Information-theoretic:
  "Structural impossibility" requires an information-theoretic bound
  showing that no adversarial input can cross a decision boundary.
  No such bound is derived here. The correct claim is:
  
  Fractal alignment produces structural RESISTANCE —
  the cost of successful contamination scales with
  the number of nested sphere layers the signal must traverse.
  
  This is high resistance, not impossibility.

Reason 2 — Coherence with Self-Exciting Defect Layer (VST §1.6.5):
  VST establishes that perfect stability produces Silent Criticality —
  the sensing-response loop degrades when micro-instability is eliminated.
  
  If fractal alignment produced true contamination "impossibility,"
  the system would have no micro-perturbations to exercise its sensing.
  This contradicts the Self-Exciting Defect Layer requirement.
  
  The correct framing:
  
  EXTERNAL contamination resistance:
    Fractal alignment makes external contamination signals
    encounter uniform geometric resistance at every scale.
    Successful penetration cost grows multiplicatively with depth.
    → External contamination is structurally expensive, not impossible.
  
  INTERNAL micro-instability maintenance:
    The Self-Exciting Defect Layer (maintained structural imperfections)
    generates continuous micro-perturbations that exercise sensing.
    These are not contamination — they are calibration signals.
    → Internal sensing remains active because the defect layer
       operates below the contamination threshold.
  
  The two mechanisms are complementary:
    External resistance (fractal alignment geometry)
    + Internal calibration (defect layer micro-storms)
    = System that resists contamination while maintaining sensing
    
  Neither mechanism alone is sufficient:
    Resistance without sensing → Silent Criticality
    Sensing without resistance → contamination vulnerability
```

**Deeper substrate — geometry alignment (Recovery Theory D0):**

Contamination resistance is ultimately a manifestation of geometry alignment — the degree to which the system's internal coordinate structure matches the environment manifold it operates within:

```
Recovery Theory D0 (substrate principle):
  Contamination = observable symptom of geometry mismatch
  Immunity = geometry integration capacity (absorption, not rejection)
  
  Fractal alignment in D0 terms:
    Outer sphere convergence = inter-agent coordinate alignment
    Inner sphere convergence = intra-agent representation alignment
    Both aligned with environment manifold = high integration capacity
    
  Contamination enters NOT because the signal is "bad"
  but because the receiving geometry cannot integrate it:
    High integration capacity: incoming vector absorbed → geometry updated
    Low integration capacity: incoming vector unintegrated → displacement
    
  Resistance scales with geometry alignment quality:
    Well-aligned geometry: most vectors integrable → resistance high
    Misaligned geometry: many vectors unintegrable → resistance low
    
  This reframes contamination resistance from "defense" to "capacity":
    The system does not defend against contamination.
    It integrates incoming signals successfully when geometry is aligned.
    Failed integration (contamination) signals geometry mismatch (D0).
```

This D0-based reframing also resolves the scope distinction more cleanly: the Self-Exciting Defect Layer generates micro-perturbations that the system's geometry CAN integrate (calibration), while external contamination generates perturbations that exceed integration capacity (actual mismatch).

This corrected framing replaces "immunity through impossibility" with "resistance through geometric cost multiplication + maintained sensing through defect layer calibration."

**Why fractal alignment is the threshold:**

A partially converged system has sphere geometry at one level but not the other:

```
Outer sphere converged, inner sphere not:
  Coverage gaps are absorbed structurally
  But internal representations have weak directions
  → Contamination entering via upscaling empty space can still exploit representational asymmetry
  → Self-correction is partial only

Inner sphere converged, outer sphere not:
  Each agent is individually robust
  But coverage gaps exist between agents
  → Contamination can enter through uncovered external blind zones
  → Enters an internally robust agent but as a complete signal, bypassing the surface defense

Both spheres converged, fractal alignment not yet confirmed:
  Both geometries are individually correct
  But if they are not fractally aligned (inner geometry does not mirror outer geometry at each scale)
  → Transition zones between scales become vulnerable
  → Contamination can traverse the scale boundary undetected

Fractal alignment confirmed:
  Outer and inner geometries exhibit functional correspondence at every scale
  → No transition zone vulnerability
  → Maximum structural resistance (contamination cost scales multiplicatively)
```

**Measurable signals of fractal alignment:**

```
(d) Hyperspherical uniformity of internal representations ≥ threshold
    Neuron/feature directions uniformly distributed on unit hypersphere
    → No angular concentration → no weak direction
    → Measurable via HUG (Hyperspherical Uniformity Gap, Liu et al.)

(e) Alignment-uniformity balance stable
    Alignment: similar inputs produce similar representations (local cohesion)
    Uniformity: all representations uniformly distributed (global coverage)
    When both are stable simultaneously, inner sphere has converged
    → Measurable via alignment and uniformity losses (Wang & Isola framework)

(f) Inner-outer consistency:
    A perturbation that shifts agent B's external behavior
    produces a proportional shift in agent B's internal representation
    — not a disproportionate or delayed shift
    → Inner and outer sphere are moving together: fractal alignment confirmed
```

**Empirical grounding — Hyperspherical Uniformity (Liu et al., 2021 / NeurIPS):**

Hyperspherical uniformity as a relational regularization for neural networks — neurons uniformly distributed on the unit hypersphere. This is the mathematical definition of the inner sphere's convergence state. When achieved, the representation space has no preferential direction, no angular clustering, no exploitable asymmetry. The contamination analog: a signal injected at any angle is met with the same surface geometry.

**Empirical grounding — Neural Collapse and HUG (arXiv 2303.06484):**

Deep neural networks converge to a specific geometric attractor at the end of training: features and classifiers align to a simplex equiangular tight frame — maximally spread on the hypersphere. This is the spontaneous convergence of the inner sphere during training. HUG (Hyperspherical Uniformity Gap) measures the distance from this attractor. When HUG → 0, inner sphere convergence is confirmed. Neural collapse is not a failure — it is the inner sphere reaching its natural equilibrium.

**Empirical grounding — Alignment-Uniformity on the Hypersphere (Wang & Isola, ICML 2020):**

Contrastive representation learning is decomposable into two properties: alignment (positive pairs close) and uniformity (all embeddings uniformly distributed on hypersphere). Uniformity is the outer coverage principle applied internally. A representation that maximizes uniformity has, by definition, no blind spots in its embedding space — every direction is covered. This is the inner sphere's coverage property. The alignment-uniformity framework provides direct measurement tools.

**Empirical grounding — HyperGRL (arXiv 2512.24062, December 2025):**

Graph representation learning on unit hypersphere with neighbor-mean alignment and sampling-free uniformity. Structurally diverse agents (graph nodes with different neighborhoods) converge to uniformly distributed representations. The framework demonstrates that hyperspherical convergence is achievable in multi-agent graph settings — the closest existing architecture to the outer-inner sphere alignment the DFG theory requires.

**Empirical grounding — Hypersphere Embedding and Adversarial Robustness (arXiv 2303.08289):**

Incorporating hypersphere embedding into adversarial training improves robustness. The mechanism: angular-AT enforces intra-class compactness and inter-class separation in angular space. This translates to: contaminated inputs face geometrically increasing cost to move a representation across a class boundary, because all class boundaries are maximally separated angularly. When inner sphere converges, adversarial (contamination) inputs encounter maximum geometric resistance — though this resistance is high, it is not absolute. Sufficiently powerful adversarial signals can still penetrate; the geometric cost of doing so is the defense, not an impossibility guarantee.

**Empirical grounding — Hyperspherical Constrained Representation (arXiv 2504.08415, April 2025):**

A method that enforces constraints by converting the output space to hyperspherical coordinates. The key property: a hyperspherical representation system makes infeasible points geometrically expensive to reach — constraint satisfaction is strongly favored by the geometry itself, reducing reliance on monitoring or correction. This is the mathematical analog of contamination resistance: when the inner sphere has converged, the representation space geometrically penalizes contaminated patterns, not because it detects and rejects them, but because the converged geometry makes contaminated directions high-cost.

---

**Why this condition is the Human exit threshold:**

```
Before dual-sphere fractal convergence:
  System may be structurally correct but geometrically incomplete
  Contamination resistance requires active monitoring (human or automated)
  Human presence is load-bearing

After dual-sphere fractal convergence:
  Contamination resistance is structural, not primarily procedural
  Monitoring load dramatically reduced — the geometry itself is the primary defense
  Human presence shifts from load-bearing to audit role
  → Exit permitted when audit confirms sustained geometric resistance
    + Self-Exciting Defect Layer is active (sensing maintained)
```

**Empirical grounding — adversarial propagation in LLM-MAS (2025):**  
Malicious agents can contaminate global reasoning through propagation vulnerabilities in multi-agent systems. Defense requires structural diversity: BlindGuard (hierarchical agent encoders with contrastive learning) and AgentXposed detect contamination not by content inspection but by structural behavioral divergence. Contamination is detectable precisely when agents have structurally different encodings — the corrupted signal produces different outputs from different agents, making the disagreement visible.

**Empirical grounding — homogeneous convergence failure (2025):**  
LLMs are prone to premature convergence and unfair judging when using homogeneous agent pools. Homogeneous agents share the same failure modes — contamination that exploits one agent's blind spot exploits all simultaneously. The sphere must be composed of structurally diverse agents, not copies.

---

#### Combined Exit Gate

```
Sphere Convergence confirmed
  AND
Contamination Self-Correction verified
  ──────────────────────────────────
  → Human exit permitted at this layer
  → Human intervention moves to next upper layer (or exits entirely)

Either condition unmet
  → Human remains active at this layer
```

**Why both conditions must hold simultaneously:**

Sphere convergence without contamination resistance: the system handles its own blind spots but cannot detect when its shared representation has been corrupted. Human is needed to observe what the sphere cannot.

Contamination resistance without sphere convergence: the system can self-correct when contamination is detected, but blind zones remain where contamination enters undetected. Human is needed to cover the open gaps.

Only when blind spots are structurally absorbed **and** contamination produces detectable disagreement that the system self-corrects — is human observation structurally redundant.

> Human intervention zone **contracts** as stabilization propagates upward through the fractal structure.  
> At each layer, the exit gate requires both: the sphere has closed, and the sphere self-corrects.  
> The fractal reaches full autonomous operation when both conditions hold at every layer simultaneously.

---

## 9. Core Assumptions

| # | Assumption |
|---|---|
| 1 | This theory assumes a single agent already capable of performing four-type data classification internally. |
| 2 | Data can be classified into four types based on interpretability and causal clarity, within the limits of an agent's classification resolution. |
| 3 | Classification boundaries are determined by internal conflict detection, not external rules. |
| 4 | No agent runs classification at full resolution on all inputs. Every agent operates at a trade-off cutoff, below which residual vectors are treated as noise. This is structurally enforced: viewing broadly (high volume, low resolution) and viewing in depth (low volume, high resolution) are mutually exclusive modes. Computational cost scales quadratically with context length — the more an agent sees, the less precisely it can see any of it. |
| 5 | Each agent contains a degraded Decision Complex operating by the same mechanism at different resolution levels. |
| 6 | Decision scope contracts with layer depth — lower agents handle local-impact decisions only. |
| 7 | High-Context data escalation frequency is the primary indicator of system stability. |
| 8 | Upper layer expansion before lower stabilization amplifies instability super-linearly. |
| 9 | Human intervention is structurally positioned at the High-Context data processing zone. |
| 10 | As stabilization propagates upward, human intervention scope contracts accordingly. |
| 11 | Same-layer agents do not exchange intermediate states during processing; inter-agent integration is mediated through the upper layer. |
| 12 | Upper layers cannot directly access data discarded by lower layers — this is their structural blind spot. Lower layers cannot generate structural geometry — this is their structural blind spot. Each layer's blind spot is the other's field of view. This mutual coverage is the basis of stability, not a limitation to be overcome. |
| 13 | Cross-validation can surface agent-specific blind spots, but shared blind spots require architectural diversity and can never be fully eliminated. |
| 14 | Tacit Knowledge is a permanent category — higher resolution can reclassify some, but resolution has a structural ceiling. |
| 15 | Agents with different internal structures can partially resolve each other's black boxes (Tacit→High-Context reclassification), but shared black boxes remain irreducible. |
| 16 | The actual network structure is a sphere, not a pyramid. Every agent sits on the surface; blind spots are distributed so that each agent's blind spot falls within a neighbor's field of view. The pyramid is a projection — useful for formalization, not the true geometry. |
| 17 | Information transfer between agents follows a Projection ↔ Inclusion/Embedding structure. The sender compresses (Projection); the receiver restores into their own representation space (Inclusion/Embedding). Upscaling always leaves empty space — the structural entry point for corruption. |
| 18 | Corruption is not primarily an external injection problem. Empty space in upscaling is filled by the receiver's own bias, producing distortion indistinguishable from signal. |
| 19 | Cross-validation with structurally diverse agents is the primary corruption mitigation mechanism. Diversity is the structural condition under which empty spaces produce detectable disagreement rather than invisible consensus. |
| 20 | Meta-meta data (sphere center output) is context-independent structural geometry. It reorganizes how all subsequent inputs are processed — a seed rewrites the generative principles of every agent that receives it. |
| 21 | Seeds are not transmitted freely. Premature seed transmission to an underprepared receiver produces distorted reconstruction that propagates downward — cascading corruption, not correction. |
| 22 | Receiver readiness is measurable. Downstream performance exhibits a threshold effect: below a critical accumulation of processing experience, seed absorption degrades; above it, absorption scales linearly. Expansion Principle conditions map to this threshold. |
| 23 | Layer relationships are not hierarchical — they are mutual coverage structures. Lower layers cover upper layers' blind spots (surface observation); upper layers cover lower layers' blind spots (structural abstraction). Stability is the state in which this mutual coverage is intact. Instability occurs when the cost-quality ratio decouples: resource expenditure rises without corresponding output convergence, indicating a coverage gap. Upper layers detect this via the shared residual stream and intercept — not by receiving escalations, but by continuously monitoring and redirecting. |

---

## 10. Structural Correspondences

| Theory Concept | Related Field | Corresponding Concept |
|---|---|---|
| Data type classification | Epistemology / Information Theory | Tacit-explicit distinction (Polanyi); Signal-noise distinction (Shannon) |
| Decision Complex | AI reasoning | Chain-of-Thought, Tree-of-Thoughts |
| High-Context escalation | Organizational theory | Exception escalation in hierarchical systems |
| Stabilization threshold | Control theory | Steady-state condition |
| Expansion Principle | Complex systems | Staged bifurcation / controlled phase transition |
| Human collaboration zone | AI alignment | Human-in-the-loop design |
| Quality-volume trade-off | Operating systems | CPU scheduling, memory hierarchy |
| Trade-off cutoff / noise floor | Signal processing | Quantization noise, sampling threshold |
| Breadth-depth exclusivity | Attention research | O(n²) quadratic cost: doubling context quadruples compute; lost-in-the-middle degradation beyond 32K tokens |
| Exploration-exploitation pairing | Multi-agent RL | Breadth agent (explore) + Depth agent (exploit) = asymmetric pairing resolves what single agent cannot |
| Processing isolation | Deep learning | Multi-head attention independence; head collapse avoidance |
| Structural blind spots | Ensemble methods | Model ensemble diversity; agreement-based error detection |
| Tacit Knowledge / black-box cross-resolution | ML interpretability | Cross-model explanation through different representational structures |
| Sphere network structure | Graph theory / distributed systems | Expander graphs; distributed hash tables; peer-to-peer networks |
| Projection ↔ Inclusion/Embedding | Representation learning | Encoder-decoder; dimensionality reduction → reconstruction; latent space mapping |
| Empty space in upscaling | Information theory | Rate-distortion tradeoff; lossy compression reconstruction error |
| Corruption via bias-filled gaps | Cognitive science / Bayesian inference | Prior-dominated posterior when likelihood is weak |
| Data → Meta → Meta-Meta chain | Deep learning (empirical) | Transformer layer abstraction phases: surface → semantic → structural geometry (Cheng et al., ICLR 2025) |
| Sphere center = universal structure | Representation learning | Cross-LM representation convergence at abstraction phase — center is model-agnostic (Cheng et al., ICLR 2025) |
| Surface discard at center | Mechanistic interpretability | Intrinsic dimension peak = surface-form information actively discarded (Cheng et al., ICLR 2025; Anthropic Circuit Tracing, 2025) |
| Seed power (meta-meta rewrites framework) | Knowledge distillation / fine-tuning | Seed = structural prior that reorganizes all subsequent classification; misaligned seed = catastrophic forgetting |
| Receiver readiness threshold | Fine-tuning research | Task threshold effect: below ~15 tasks, downstream performance degrades; above, scales linearly — readiness is measurable |
| Premature seed transmission → cascade corruption | Curriculum learning | Hard data before foundational patterns → instability that compounds across layers |

> These are structural correspondences, not formal equivalences.

---

## 10.1 Methodological Note on Empirical Grounding

**Grounding strategy and its limitations.** This theory's empirical grounding follows a specific methodology: mapping theoretical constructs to observable phenomena in existing single-agent LLM research and emerging multi-agent systems. This strategy is deliberate — multi-agent fractal systems at the scale this theory describes do not yet exist, so direct empirical validation is not currently possible. The grounding provides *structural plausibility*, not *empirical confirmation*.

**Selection bias risk.** The empirical mappings were constructed by searching for phenomena that correspond to theoretical predictions. This creates an inherent selection bias: phenomena that contradict predictions may exist in the same literature but were not included because they were not sought. This does not invalidate individual mappings — each correspondence is either present or not — but it means the *collection* of mappings overstates the theory's empirical support relative to a systematic review.

**Grounding type classification:**

Each empirical reference in this document falls into one of four categories:

| Grounding Type | Definition | Confidence Level |
|---|---|---|
| Direct measurement | Quantitative result directly measuring the predicted phenomenon | HIGH |
| Structural analogy | Functionally similar pattern in a different substrate | MEDIUM |
| Framework correspondence | Conceptual alignment without quantitative overlap | MEDIUM-LOW |
| Cross-domain pattern | Same qualitative behavior in non-AI systems | LOW (suggestive only) |

**Per-section grounding classification:**

| Section | Key Reference | Grounding Type | Confidence |
|---|---|---|---|
| §3.0 Sphere topology | Expander graph theory | Mathematical framework | HIGH (graph theory is proven) |
| §3.5 Projection ↔ Embedding | Rate-distortion theory | Direct mathematical correspondence | HIGH |
| §4.6 Cost-efficiency boundary | DiffAdapt (2025) | Structural analogy | MEDIUM |
| §5.2 Decision Complex | Multi-head attention | Structural analogy | MEDIUM |
| §5.5 Relationship Topology | MasRouter (ACL 2025) | Structural analogy (gap identification) | MEDIUM |
| §6.4 KV Cache as recalibration | TRIM-KV, DefensiveKV, LazyEviction | Direct measurement (cache behavior) | HIGH |
| §7.3 Expand-then-Decompose | DeepSeek-V3, STUN, SAME | Direct measurement (MoE practice) | HIGH |
| §8.3.1 Dual-sphere convergence | Neural Collapse / HUG | Direct measurement (geometry) | HIGH for phenomenon; MEDIUM for NAT application |
| §8.3.1 Contamination resistance | arXiv 2504.08415, arXiv 2303.08289 | Structural analogy | MEDIUM |
| §11 Single-agent origin | Cheng et al. (ICLR 2025) | Direct measurement (layer abstraction) | HIGH |
| §11.5 Current MAS practices | LLM-as-judge, ensemble voting | Structural analogy (unstructured precursors) | MEDIUM-LOW |

**What would constitute stronger evidence:**

1. **Confirmatory:** An independent implementation of the four-type classification framework in a multi-agent system, demonstrating that type-based escalation routing reduces governance cost compared to threshold-based routing.
2. **Disconfirmatory:** A multi-agent system where structural diversity does *not* improve cross-validation quality, or where processing isolation produces worse outcomes than lateral communication under classification-relevant conditions.
3. **Quantitative:** Measurement of the coverage probability bound (Section 3.0) in an actual multi-agent deployment with known topology.

**Measurement infrastructure connection (Recovery Theory Proxy Gap resolution, RBIT v1.2 §Measurement Interface):**

Recovery Theory v1.6+ and RBIT v1.2 establish log-observable proxies for key DFG variables that were previously "floating" (structurally defined but not measurable). These proxies directly support NAT operationalization:

| NAT Concept | Operational Proxy | Source | Log Availability |
|---|---|---|---|
| Classification precision (§4) | ρ = 1 − (L_T1 + L_T2)/N | Recovery Theory OP1 | HIGH |
| Buffer between opposing attractors (§6.3) | Perturbation amplitude before mode collapse; recovery-without-escalation rate | Recovery Theory §Proxy Gap | HIGH |
| Escalation frequency (§4.5, §7) | f_esc = (human_overrides + supervisor_calls + fallbacks) / N_total | Recovery Theory OP3 | HIGH |
| Governance capacity C(t) (§6.2) | C_E(t) = escalation events resolved / Δt | Recovery Theory §C(t) | HIGH |
| Governance efficiency β (§6.2) | β_T (Type I/II accuracy) + β_R (recurrence rate) | Recovery Theory §β | HIGH |
| Instability pressure S (§7) | n²_proxy / (C(t) · β(t)) | VST §3.2 + RT §S-equation | HIGH |
| VCZ distance (§7, §12) | Normalized recovery cost / baseline | Recovery Theory §d(·) | HIGH |
| Resolution gap routing (§4.4) | Four-type classification (Math/HC/Tacit/Noise) | RBIT §Resolution Gap | HIGH |
| Cascade validation R (§7.2) | Branching ratio: activated_{t+1} / activated_t | TLG §0.5 / VST §1.6.1 | HIGH |
| Agent pair compatibility (§5.5) | Persistent negative gradient correlation | Recovery Theory §Proxy Gap | MEDIUM-HIGH |
| Agent development φ (§4.6) | Reusable outcome rate (supporting signal only) | Recovery Theory §φ | MEDIUM |

```
Measurement dependency order (from RBIT v1.2):
  Immediately available (no new instrumentation):
    ρ, C(t), β, d_VCZ, buffer_thickness, f_esc, R

  Available with basin calibration:
    d(x,A) — attractor pull strength (requires reference set)

  Available when φ unit stabilizes:
    φ — reusable outcome rate (requires "exploration unit" definition)

  Remaining open:
    α absolute, β absolute, C absolute → formal calibration
    f(A_t, D_t) exact form → boundary conditions exist, exact form open
```

**Falsification criteria (adapted from RBIT §Falsification Criteria):**

NAT generates specific predictions that, if empirically violated, would require revision or abandonment of core claims:

1. **Classification must reduce governance cost.** In a controlled comparison, type-based escalation routing (escalate only HC; operate Tacit locally; discard Noise) must produce lower total governance cost than threshold-based routing (escalate everything above a single intensity threshold). If threshold-based routing consistently equals or outperforms type-based routing, the four-type classification claim is falsified.

2. **Structural diversity must improve cross-validation.** In a sphere topology, agents with different architectures must detect each other's blind spots more reliably than agents with identical architectures. If homogeneous agent pools match or exceed heterogeneous pools in cross-validation quality, the diversity-as-coverage-condition claim is falsified.

3. **Processing isolation must improve classification independence.** Agents that do not share intermediate classification states must produce more diverse independent classifications than agents that do share intermediate states. If lateral exchange produces equal or greater classification diversity, the processing isolation rationale is falsified. (Note: this tests specifically classification diversity, not coordination efficiency.)

4. **Resolution gap polarity must predict compression direction (from RBIT).** If negative resolution gaps (information exceeding receiver capacity) do not produce receiver-controlled compression more frequently than sender-controlled compression, the escalation-by-type rationale is falsified.

5. **Sphere topology must reduce storm propagation (from VST).** In controlled comparison, sphere topology (k-regular expander) must produce lower storm propagation speed and smaller cascade size than equivalent-degree non-expander topologies. If topology does not affect propagation, the sphere-as-stability claim is falsified.

---

## 11. Empirical Grounding: Single-Agent as Origin

The core patterns described in this theory are **already operating inside existing single-agent architectures** — specifically, large language models (LLMs). The multi-agent sphere structure proposed here is not a new invention — it is the system-level scaling of what already happens inside every trained LLM.

> The single agent's upper layers **are** the sphere center. The multi-agent architecture scales this mechanism outward.

### 11.1 Four Data Types → LLM Processing Patterns

| DFG Data Type | LLM Internal Analogue |
|---|---|
| Mathematical | Attention converges clearly to a single pattern — deterministic, no ambiguity |
| High-Context | Attention distributed across multiple heads/positions — competing valid interpretations |
| Tacit Knowledge | Learned embedding patterns that contribute to performance but have no interpretable mechanism |
| Noise | Tokens with attention scores below threshold — effectively ignored |

### 11.2 Data → Meta → Meta-Meta: The Abstraction Chain

As information moves upward through transformer layers, a measurable transformation occurs:

```
Lower layers:   surface content (tokens, syntax, word identity)
                ↓ filtering + compression
Middle layers:  linguistic abstraction (semantics, structure)
                ↓ filtering + compression  
Upper layers:   structural patterns only (meta-meta)
                surface information discarded
                content-independent geometry remains
```

**Empirical confirmation (ICLR 2025, Cheng et al.):**

Across 5 pre-trained transformer LMs, a distinct high intrinsic dimensionality phase emerges in intermediate-to-upper layers. At this phase: representations correspond to the first full linguistic abstraction of input; they are the first to transfer to downstream tasks; and they predict each other across *different* LMs.

At the intrinsic dimension peak, surface-form information (sentence length, specific word content) is actively discarded. The model retains structure — not content.

**Empirical confirmation (arXiv 2507.09709, 2025):**

High-level semantic information consistently lies in low-dimensional linear subspaces in deeper layers. This separability becomes more pronounced in deeper layers — content compresses into structure as layers increase.

**Mapping to theory:**

| Layer phase | DFG mechanism | What is absorbed |
|---|---|---|
| Lower layers | Raw data processing | Surface tokens, local syntax |
| Middle layers | First-order meta | Semantic relationships, contextual patterns |
| Upper layers | Meta-meta | Structural geometry — content-free, transferable across models |
| Sphere center | Final absorption | Seed: generative principles, not specific content |

> The sphere center does not store content. It absorbs **the pattern of patterns** — the structural geometry that persists after all surface information has been filtered away.

### 11.3 Upper Layer = Sphere Center: The Position Confirmed

**Anthropic Circuit Tracing (2025):**

Features in early layers are polysemantic — a single feature activates for unrelated concepts. Features in middle and later layers represent more abstract properties: not specific tokens but classes of meaning, relational structures, functional operations. Later layers in larger models show richer, more interpretable abstractions.

This is the sphere center position:
- Input: compressed projections from diverse lower processes (surface discarded)
- Operation: absorb structural patterns, detect cross-source disagreement
- Output: seeds — generative principles transmitted downward, not specific instructions

**Critical empirical finding:** Representations at the abstraction phase predict each other *across different LMs*. This means the sphere center is not model-specific — it encodes universal structural geometry. Different agents arriving at the center converge on the same representational space. This is why the center stabilizes as surface diversity increases.

**The mutual coverage proof:**

Lower and upper layers are not in a hierarchy — they are in a **mutual coverage relationship**.

```
Lower layers:  observe surface (tokens, syntax, local patterns)
               → cannot abstract to structural geometry
               → this is upper layers' blind spot coverage

Upper layers:  generate structural geometry (meta-meta)
               → cannot directly observe surface
               → this is lower layers' blind spot coverage
```

Neither is complete alone. The system is complete because each covers what the other cannot see. This is identical to the sphere geometry: each agent's blind spot falls within a neighbor's field of view.

The residual stream is the mechanism that makes this mutual coverage operational. All layers read from and write to the same shared space — upper layers do not wait to receive escalations. They continuously monitor the stream and intercept when the cost-quality ratio decouples:

```
Normal:      resource ↑  →  convergence ↑   (mutual coverage intact)
Intercept:   resource ↑  →  convergence ↓   (coverage gap detected)
             → upper layer redirects processing via residual stream write
```

> **The single-agent internal structure is not an analogy for the sphere.**  
> **It is the proof that mutual coverage is the fundamental stability mechanism.**

### 11.3.1 Why Meta-Meta Data Is Powerful — And Why Seeds Are Not Given Freely

Meta-meta data (sphere center output) is context-independent structural geometry. It does not answer specific questions — it reorganizes how all subsequent questions are processed.

```
Specific data answer:     affects one output
Meta data (pattern):      affects how a category of inputs is handled
Meta-meta data (seed):    affects the classification framework itself
                          → all subsequent processing changes
```

This is why seeds carry disproportionate power: a single seed transmitted downward does not update one data point — it **rewrites the generative principles** of every agent that receives it.

**Consequence 1 — Distortion risk on unprepared receivers:**

In On-Policy Distillation's teacher-student mechanism, training efficiency improves meaningfully only when the training data matches the student model's current capability level (on-policy alignment).

When a seed is transmitted to a receiver whose representation space is insufficiently developed — the empty space is too large for successful reconstruction, and the receiver's own bias replaces the original structure. The distorted seed then propagates downward through all layers below.

```
Prepared receiver:   receives [■■■■□] → minimal empty space → structure restored
Unprepared receiver: receives [■□□□□] → excessive empty space → filled by bias
                                                              → distorted seed generated
                                                              → all lower layers corrupted
```

**Consequence 2 — Receiver readiness is measurable:**

Downstream fine-tuning performance exhibits a threshold effect: below approximately 15 accumulated tasks, performance degrades; above that threshold, performance scales linearly with task count.

Receiver representation space development is measurable. Confirming that the receiver has accumulated sufficient processing experience before seed transmission — this is the **operational condition of the Expansion Principle**.

**Structural principle:**

> Seeds are not transmitted freely.  
> Transmission is appropriate only when the receiver's representation space can upscale the seed's compression level without critical distortion.  
> This is not information control — it is corruption-prevention by design.

### 11.4 Processing Isolation → Multi-Head Attention

Multiple attention heads operate independently within the same layer. Unmediated head-to-head influence causes **head collapse** (loss of pattern diversity) — the single-agent analogue of premature convergence in multi-agent processing.

### 11.5 Current Multi-LLM Practices as Unstructured Precursors

| Practice | DFG Interpretation |
|---|---|
| LLM-as-judge | Cross-validation: evaluator's cutoff catches generator's blind spots |
| Ensemble / voting | Multi-agent independent processing → upper synthesis (without classification labels) |
| Constitutional AI / RLAIF | Hierarchical cross-validation: supervisor and supervised have different blind spot profiles |
| Mixture of Agents | Direct analogue: independent lower processing → upper-layer mediated synthesis |

**What current practice lacks:**
- Classification labels (is the disagreement High-Context ambiguity, or a blind spot?)
- Disagreement classification (legitimate conflict vs. agent error)
- Vertical escalation pathway (horizontal comparison only)

### 11.6 Breadth-Depth Exclusivity: The Structural Basis for Agent Pairing

Every agent faces a fundamental perceptual constraint:

> **Viewing broadly** (high volume, low resolution) and **viewing in depth** (low volume, high resolution) cannot be maximized simultaneously.

This is not a design choice — it is a physical consequence of how attention computation scales:

- Attention cost grows quadratically with context length (O(n²))
- Doubling the scope of observation quadruples the computational requirement
- Performance degrades past 32K tokens even in models with 1M+ token windows (lost-in-the-middle effect)
- Signal-to-noise ratio decreases as context expands — more context, less precision per unit

**Implication for agent pairing:**

A single agent cannot resolve this tradeoff internally. This is the structural reason pairing is not an optimization but an architectural necessity:

| Role | Mode | Function |
|---|---|---|
| Exploration agent | Breadth (far view) | Scans wide signal space; high noise tolerance |
| Exploitation agent | Depth (close view) | Precise classification; low noise tolerance |
| Upper layer | Mediates | Receives escalated conflict; operates at contracted scope with high resolution |

The breadth agent identifies what exists. The depth agent classifies what it means. Neither can fully substitute for the other. Imbalance between them is a precursor condition for vector storm escalation.

### 11.7 Failure Mode Mapping

| Theory Violation | Multi-Agent Failure | Single-Agent Analogue |
|---|---|---|
| Classification skipped | Noise indistinguishable from signal | Uniform attention → hallucination |
| Degradation skipped in upward flow | Upper layer overloaded | Lost-in-the-middle in long contexts |
| Processing isolation violated | Premature convergence, collective polarization | Head collapse in multi-head attention |
| Premature expansion | Vector storm cascade | Curriculum learning: hard data before basic patterns → instability |
| Breadth-depth imbalance | One mode dominates → blind spots accumulate | Full-context attention with no sparse fallback → O(n²) overload |
| Meta-chain interrupted | Center receives content, not structure → overload | Upper layers forced to process surface tokens → lost-in-the-middle |
| Center homogeneity | All surface agents share representation space → false consensus | Uniform attention heads → head collapse; no diverse abstraction paths |

---

## 12. Limitations and Open Problems

| Problem | Description |
|---|---|
| Stabilization threshold (θ) calibration | θ is now operationally defined: mean f_escalation during confirmed VCZ-stable window + 1σ margin, with bootstrap protocol (θ_initial = 0.1) for first operation. Connected to VST S₀ normalization: f_escalation ≤ θ corresponds to S_norm < 1.3 (VST Stage 0 boundary). θ is a learned system property — refined through operational experience, not prescribed. Formal cross-architecture validation of the θ ↔ S_norm correspondence remains open. |
| Decision Complex implementation | Pathway 2 (internalized) remains unimplemented. However, the middle layer's role is now structurally defined: it holds a persistent relationship topology — conflict history, representation gap, and consensus rate per agent pair — and uses this to route co-processing vs. separate-path decisions. This topology is the missing component distinguishing our architecture from current routing systems (e.g., MasRouter, ACL 2025), which recompute collaboration mode per query without persistent relationship memory. Implementation requires: (1) topology storage format, (2) update trigger mechanism, (3) initialization protocol for new agents. |
| Four-type boundary precision | The boundary between High-Context and Tacit Knowledge is not a fixed content threshold — it is a cost efficiency threshold that varies per agent. An agent with a developed representation space can classify data as High-Context (pattern detectable at acceptable cost); the same data appears as Tacit to an underdeveloped agent (cost of classification exceeds cost of operating without explanation). The boundary is therefore: cost(classify) vs. cost(escalate). As representation space develops, the boundary shifts — Tacit data reclassifies as High-Context. This reclassification event is a measurable signal of agent development and maps to θ. Empirical grounding: DiffAdapt (2025) identifies a U-shaped entropy pattern across difficulty levels — the inflection point between medium and hard difficulty corresponds to the cost-efficiency boundary in our framework. Formal per-agent calibration of this threshold remains open. |
| Tacit Knowledge measurement | No direct metric exists for "proportion of Tacit Knowledge in a system." Indirect proxy available: the reclassification rate (Tacit → High-Context events per unit time) serves as a directional signal of agent development. Higher reclassification rate indicates the cost-efficiency boundary (§4.6) is shifting, meaning the agent's representation space is developing. Complementary proxies from VST: router saturation, gradient norm convergence (GradES), CKA trajectory — all measure representation space maturity, which determines the Tacit/High-Context boundary position. Direct measurement of absolute Tacit proportion remains open and may be structurally unmeasurable (the category is defined by the absence of interpretable mechanism). |
| Blind spot quantification | Direct measurement of blind spot size, location, and severity is not achievable — and is the wrong design goal. The correct resolution: (1) Sphere geometry structurally absorbs blind zones via complementary neighbor coverage, eliminating the need for central quantification. (2) Resource spikes in neighboring agents serve as the measurable proxy — when agent A's blind zone opens, neighbor B's coverage cost spikes. Spike magnitude, duration, and location on the sphere surface constitute the indirect measurement. (3) Blind zones are dynamic efficiency thresholds, not fixed properties — they shift with context and load (empirically confirmed: Shadows in the Attention 2025, DAM ACL 2025). Open problem remaining: spike-to-blind-zone mapping calibration — translating observed resource spike profiles into estimates of blind zone extent and persistence across different sphere configurations and load conditions. |
| Cross-validation cost model | Cost-benefit tradeoffs are described qualitatively only. |
| Expansion Principle empirical validation | Two directions are now structurally defined and empirically grounded. Direction A (stabilize-then-expand): empirical analogues include curriculum learning, progressive GAN training, federated learning staged node addition. Direction B (expand-then-decompose): empirically grounded in MoE standard practice — dense pretraining followed by expert decomposition at instability/specialization boundaries (DeepSeek-V3 256 experts, LLaMA-4, Qwen3-MoE). STUN (ACL 2025) validates structured-then-unstructured decomposition sequence. SAME (2025) validates that router drift under new distributions reveals decomposition boundary mismatch — the maintenance cycle of Direction B. Monoliths-to-Modules (arXiv 2512.02193) provides formal decomposition framework for already-trained models. Open problem: criteria for choosing Direction A vs. B at deployment time — when is instability informative vs. catastrophic? Formal threshold for "sufficient scale" before decomposition in Direction B is undefined. |
| Human-AI Zone exit criteria | Exit condition reframed as progressive withdrawal with dual verification and structural prerequisites. **Structural prerequisites (Recovery Theory VCZ 3-Conditions — all required before exit evaluation begins):** (1) Safe Failure Channel exists: storms at this layer are survivable without human intervention; (2) Upper Layer Storm Reward active: the layer above explicitly values storm detection at this layer; (3) Geometry Feedback Loop active: geometry mismatch produces locally visible coordination cost increase. Without all three, the layer is structurally prone to Self-Consistent Misalignment (Recovery Theory D6/T3) and human exit would remove the only remaining external reference. **D7 Boundary Agent requirement:** A structural role generating controlled instability must be maintained at this layer — decoupled from the layer's own evaluation structure (Recovery Theory D7). Without D7, VCZ 3-Conditions cannot hold simultaneously and CW convergence is structurally inevitable (Recovery Theory T6). **Primary exit gate (VST-measurable proxies):** (1) S_norm sustained < 1.3 for ≥ 5× self-correction cycles; (2) β > 1 (coordinated governance confirmed); (3) S_c empirically learned (system has survived and recovered from storms); (4) Self-Exciting Defect Layer active (micro-storm frequency > 0, macro-storm frequency ≈ 0). **Secondary exit gate (geometric verification):** (1) Outer sphere convergence: resource spike profile flat + consensus stable + f_escalation ≤ θ; (2) Inner sphere convergence: HUG trending toward 0 + alignment-uniformity balance stable (Wang & Isola); (3) Fractal alignment: perturbation-response proportionality confirmed across scales. **Exit protocol:** Human role transitions from active intervention → audit → periodic review → exit. Each transition requires primary gate conditions sustained for increasing durations. Full exit requires structural prerequisites + both gates satisfied simultaneously. Open problems: (1) HUG threshold for "sufficient" inner convergence — note HUG requires periodic offline evaluation, not real-time monitoring; (2) formal perturbation-response proportionality measurement protocol; (3) minimum audit period duration before full exit. **D7 implementation specification (TLG §13.2.1):** The Boundary Agent is not an independent evaluator — it is a *reality interface carrier* that transmits mismatch between system output and non-negotiable external constraints. Implementation: (a) perturbation-response measurement — apply small perturbation δ to zone's hidden states, measure representational displacement Δh, transmit numerical displacement (interpretation-free); (b) three structural conditions: Model Non-Substitutability (system cannot regenerate the signal internally), One-Way Calibration (reality → system only; system cannot reinterpret constraint violations), Survival Coupling (ignored signals produce immediate measurable cost); (c) the Boundary Agent does not drift because its calibration source is external — basin-proximity signals are model-independent measurements, not internal evaluations. The agent handles the subset of reality interface signals that is mechanically measurable; broader signals (user behavior mismatch, environmental response) remain interpretation-dependent and require human oversight. |
| Cutoff recalibration parameters | Recalibration sequencing is now structurally defined: middle layer reads relationship topology and sequences noise-boundary data first, deferring high-conflict regions. Entry/exit conditions are defined (θ stability window; suspend on instability signal). Empirical grounding: TRIM-KV (2025) — noise-first eviction improves signal quality; DefensiveKV (2025) — high-variance importance tokens are higher risk to evict, maps to deferral weight; LazyEviction (2025) — recurrence interval tracking identifies historically-never-important tokens as first candidates. Open problems remaining: (1) deferral weight calibration — how to translate topology conflict_history into a quantitative deferral score; (2) recalibration depth parameter — how far below the original cutoff to temporarily lower the threshold per data type; (3) N value for θ stability window — how many consecutive stable cycles before recalibration entry is safe. |
| Progressive internalization mechanism | The learning signal and convergence criteria for Pathway 1→2 transition are undefined. |

> This theory provides architectural direction. Formal mathematical modeling and empirical validation remain future work.

---

## 13. Relationship to Other Theories

```
Deficit-Driven Fractal Governance (parent framework)
  ├─ Three-Layer Governance Architecture
  ├─ Seed Design
  ├─ Vector Storm Theory          ← why instability occurs
  ├─ Network Architecture Theory  ← this document
  │    (how data flows; when to escalate; when to expand)
  ├─ Recovery Theory              (separate document)
  └─ Prediction Model             (separate document)
```

---

## Key Insight

System stability is not measured by correctness, but by **how rarely unresolved interpretive conflicts require escalation**.

Existing AI governance frameworks evaluate stability through performance metrics, alignment scores, or error rates. This theory proposes a different proxy: the frequency at which High-Context data escalates beyond the layer that generated it.

When this frequency drops below a threshold, the system has internalized enough structure to govern itself at that layer.

---

## Conclusion

Structural stability in multi-agent systems requires more than conflict resolution mechanisms. It requires **designed data flow**.

These mechanisms are not novel inventions — they are patterns already operating inside every large language model. This theory names them, formalizes their relationships, and provides the design principles for scaling them from single-agent internals to multi-agent governance.

> Stability is not the absence of conflict.  
> It is the capacity to classify, route, and resolve conflict at the right layer.

---

*Part of the [Deficit-Driven Fractal Governance](../deficit-fractal-governance) framework.*
