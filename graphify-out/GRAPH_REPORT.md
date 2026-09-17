# Graph Report - online-colony  (2026-09-17)

## Corpus Check
- 8 files · ~21,692 words
- Verdict: corpus is large enough that graph structure adds value.
- Unclassified: 1 file(s) not represented in the graph (top: (none) 1)

## Summary
- 125 nodes · 157 edges · 14 communities (10 shown, 4 thin omitted)
- Extraction: 83% EXTRACTED · 15% INFERRED · 2% AMBIGUOUS · INFERRED: 23 edges (avg confidence: 0.82)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Research and Technology
- Frontier
- Education
- Policy
- Combat
- Permanent Acquired Knowledge
- graph-traceability.md
- Real-time game clock and bounded action durations
- Graph traceability project instruction
- Frontier Product Discovery
- Colony
- Macro System Design — World/Time
- Frontier Policy Matrix
- Macro System Design — Autonomy

## God Nodes (most connected - your core abstractions)
1. `Research and Technology` - 12 edges
2. `Macro System Design — Autonomy` - 10 edges
3. `Macro System Design — World/Time` - 10 edges
4. `Frontier` - 10 edges
5. `Combat` - 9 edges
6. `Production` - 7 edges
7. `Approved Specialization-Switch Rule` - 6 edges
8. `Active Specialization` - 5 edges
9. `Autonomy and Execution` - 5 edges
10. `Job System` - 5 edges

## Surprising Connections (you probably didn't know these)
- `Real-time game clock and bounded action durations` --conceptually_related_to--> `Open interaction decisions`  [AMBIGUOUS]
  docs/product/discovery.md → docs/product/interaction-inventory.md
- `Active Specialization` --conceptually_related_to--> `Health`  [AMBIGUOUS]
  docs/product/discovery.md → docs/systems/policy-matrix.md
- `Policy-to-Outcome Pipeline` --implements--> `Policy`  [INFERRED]
  docs/systems/policy-matrix.md → docs/systems/colony-governance.md
- `Health sequencing after the initial core loop` --conceptually_related_to--> `Health policy`  [INFERRED]
  docs/product/discovery.md → docs/systems/policy-matrix.md
- `Production–Infrastructure–Energy–Education core loop` --rationale_for--> `Production + Energy + Education Pilot`  [INFERRED]
  docs/product/discovery.md → docs/systems/policy-matrix.md

## Hyperedges (group relationships)
- **Approved Specialization Switch** — docs_product_discovery_specialization_switch_rule, docs_product_discovery_acquired_knowledge, docs_product_discovery_active_specialization, docs_product_discovery_transition_cost_time, docs_product_discovery_old_area_efficiency, docs_product_discovery_new_area_low_efficiency, docs_product_discovery_individual_education [EXTRACTED 1.00]

## Communities (14 total, 4 thin omitted)

### Community 0 - "Research and Technology"
Cohesion: 0.24
Nodes (14): Energy, Health, Acquired Knowledge, Active Specialization, Initial Core Loop, Individual Education for New Capability, Low Initial Efficiency in New Area, Gradual Efficiency Loss in Old Area (+6 more)

### Community 1 - "Frontier"
Cohesion: 0.14
Nodes (20): Health sequencing after the initial core loop, Autonomy and Execution, Individual Colonist, Frontier, Logistics and Transport, Sector Policies, Production, Real-Time 1:1 Clock (+12 more)

### Community 2 - "Education"
Cohesion: 0.16
Nodes (14): Production–Infrastructure–Energy–Education core loop, Colony Research Capability, Production–Energy–Education Core Loop, Neurology, Policy Capability, Research as Policy Expansion and Specialization, Individual Skill Formation, Initial Production–Infrastructure–Energy–Education chain (+6 more)

### Community 3 - "Policy"
Cohesion: 0.29
Nodes (7): Research queue and permanent knowledge, Policy, PriorityRule, StockGoal, Single research queue interaction, Common Policy Contract, Research specialization and limited capacity

### Community 4 - "Combat"
Cohesion: 0.22
Nodes (11): Regional fauna, Combat, PendingDecision, Fauna interactions, CombatEntity, Defense Interactions, Energy Policy, Fauna policy (+3 more)

### Community 5 - "Permanent Acquired Knowledge"
Cohesion: 0.31
Nodes (9): Unresolved Active Capacity Redistribution, docs_systems_colony_governance_document, docs_systems_policy_matrix_document, Limited Research Capacity and Specialization Trade-off, No Direct Research Transfer Through Contracts or Trade, Permanent Acquired Knowledge, Production-Energy-Education Pilot, Single Research Queue and One Active Research (+1 more)

### Community 6 - "graph-traceability.md"
Cohesion: 0.23
Nodes (11): Affected Files Reporting, Consistency Audit, AMBIGUOUS Relation Review, Contradiction Checking, Cross-Community Connections, Artefatos, Fluxo para mudanças, Graph Traceability (+3 more)

### Community 7 - "Real-time game clock and bounded action durations"
Cohesion: 0.50
Nodes (5): Real-time game clock and bounded action durations, Open product questions, Game-time durations in interactions, Open interaction decisions, Policy Matrix cross-document reference

### Community 11 - "Macro System Design — World/Time"
Cohesion: 0.13
Nodes (14): Interaction Inventory, Colony Governance, Policy Matrix, 1. Objetivo, 2. Escala temporal aprovada, 3.1 Calendário e estações documentais, 3. Dia/noite como Day Event especial, 4. Day Event modular (+6 more)

### Community 13 - "Macro System Design — Autonomy"
Cohesion: 0.17
Nodes (12): 1. Objetivo, 2. Princípios aprovados, 3. Fronteira de controle, 4. Educação como escola, 5.1 Estados mínimos de um job, 5. Pipeline de autonomia, 6.1 Prioridade como decisão estratégica, 6. Políticas e consequências (+4 more)

## Ambiguous Edges - Review These
- `Real-time game clock and bounded action durations` → `Open interaction decisions`  [AMBIGUOUS]
  docs/product/interaction-inventory.md · relation: conceptually_related_to
- `Health` → `Active Specialization`  [AMBIGUOUS]
  docs/product/discovery.md · relation: conceptually_related_to
- `Unresolved Active Capacity Redistribution` → `Production-Energy-Education Pilot`  [AMBIGUOUS]
  docs/systems/policy-matrix.md · relation: conceptually_related_to

## Knowledge Gaps
- **25 isolated node(s):** `Pré-requisito`, `Fluxo para mudanças`, `Artefatos`, `1. Objetivo`, `2. Princípios aprovados` (+20 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 46 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **4 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Real-time game clock and bounded action durations` and `Open interaction decisions`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Health` and `Active Specialization`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Unresolved Active Capacity Redistribution` and `Production-Energy-Education Pilot`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `Frontier` connect `Frontier` to `Research and Technology`, `Macro System Design — World/Time`, `Combat`?**
  _High betweenness centrality (0.290) - this node is a cross-community bridge._
- **Why does `Interaction Inventory` connect `Macro System Design — World/Time` to `Frontier`?**
  _High betweenness centrality (0.259) - this node is a cross-community bridge._
- **Why does `Research and Technology` connect `Research and Technology` to `Frontier`, `Education`, `Policy`, `Combat`?**
  _High betweenness centrality (0.236) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `Research and Technology` (e.g. with `Health` and `Real-Time 1:1 Clock`) actually correct?**
  _`Research and Technology` has 2 INFERRED edges - model-reasoned connections that need verification._