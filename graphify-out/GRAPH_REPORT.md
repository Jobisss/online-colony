# Graph Report - online-colony  (2026-09-15)

## Corpus Check
- Corpus is ~16,982 words - fits in a single context window. You may not need a graph.

## Summary
- 69 nodes · 88 edges · 11 communities (9 shown, 2 thin omitted)
- Extraction: 78% EXTRACTED · 19% INFERRED · 2% AMBIGUOUS · INFERRED: 17 edges (avg confidence: 0.83)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Traceability Fauna Policies
- Health Combat Colonists
- Frontier Governance Time
- Research Decisions
- Autonomy and Production
- Research Model
- Time and Open Questions
- Core Loop Production-Energy-Education
- Planning Documents
- Colony
- Policy Matrix

## God Nodes (most connected - your core abstractions)
1. `Frontier` - 10 edges
2. `Combat` - 9 edges
3. `Production` - 8 edges
4. `Research and Technology` - 7 edges
5. `Autonomy and Execution` - 5 edges
6. `Job System` - 5 edges
7. `Regional fauna` - 5 edges
8. `Policy` - 5 edges
9. `Logistics and Transport` - 4 edges
10. `Demand System` - 4 edges

## Surprising Connections (you probably didn't know these)
- `Policy-to-Outcome Pipeline` --implements--> `Policy`  [INFERRED]
  docs/systems/policy-matrix.md → docs/systems/colony-governance.md
- `Graph traceability project instruction` --references--> `Graph Traceability`  [EXTRACTED]
  AGENTS.md → docs/architecture/graph-traceability.md
- `Graph traceability project instruction` --references--> `Incremental impact graph update`  [EXTRACTED]
  AGENTS.md → docs/architecture/graph-traceability.md
- `Real-time game clock and bounded action durations` --conceptually_related_to--> `Open interaction decisions`  [AMBIGUOUS]
  docs/product/discovery.md → docs/product/interaction-inventory.md
- `Frontier` --references--> `Interaction Inventory`  [EXTRACTED]
  docs/product/discovery.md → docs/product/interaction-inventory.md

## Hyperedges (group relationships)
- **Research Decision Traceability Across Governance and Policy Matrix** — docs_systems_colony_governance_document, docs_systems_policy_matrix_document, permanent_acquired_knowledge, no_direct_research_transfer [EXTRACTED 1.00]
- **Pilot Scope for Production Energy and Education** — production_energy_education_pilot, single_active_research_queue, permanent_acquired_knowledge [INFERRED 0.75]
- **Specialization and Active Research Capacity Constraints** — limited_research_capacity, single_active_research_queue, capacity_redistribution_unresolved, skill_recovery_unresolved [INFERRED 0.85]

## Communities (11 total, 2 thin omitted)

### Community 0 - "Traceability Fauna Policies"
Cohesion: 0.22
Nodes (11): Graph traceability project instruction, Graph Traceability, Incremental impact graph update, Regional fauna, Fauna interactions, Energy Policy, Fauna policy, Production Policy (+3 more)

### Community 1 - "Health Combat Colonists"
Cohesion: 0.22
Nodes (10): Health sequencing after the initial core loop, Colonist, Combat, Logistics and Transport, PendingDecision, Health as basic support in the first cycle, CombatEntity, Ownership, Custody and Reservation (+2 more)

### Community 2 - "Frontier Governance Time"
Cohesion: 0.24
Nodes (10): Frontier, Sector Policies, Research and Technology, Real-Time 1:1 Clock, Interaction Inventory, Colony Governance, Directive, Offline Operation (+2 more)

### Community 3 - "Research Decisions"
Cohesion: 0.31
Nodes (9): Unresolved Active Capacity Redistribution, docs_systems_colony_governance_document, docs_systems_policy_matrix_document, Limited Research Capacity and Specialization Trade-off, No Direct Research Transfer Through Contracts or Trade, Permanent Acquired Knowledge, Production-Energy-Education Pilot, Single Research Queue and One Active Research (+1 more)

### Community 4 - "Autonomy and Production"
Cohesion: 0.31
Nodes (9): Autonomy and Execution, Production, BuildPlan, ColonyOrder, Governance Explanation, Demand System, Job System, Production Interactions (+1 more)

### Community 5 - "Research Model"
Cohesion: 0.29
Nodes (7): Research queue and permanent knowledge, Policy, PriorityRule, StockGoal, Single research queue interaction, Common Policy Contract, Research specialization and limited capacity

### Community 6 - "Time and Open Questions"
Cohesion: 0.50
Nodes (5): Real-time game clock and bounded action durations, Open product questions, Game-time durations in interactions, Open interaction decisions, Policy Matrix cross-document reference

### Community 7 - "Core Loop Production-Energy-Education"
Cohesion: 0.67
Nodes (3): Production–Infrastructure–Energy–Education core loop, Initial Production–Infrastructure–Energy–Education chain, Production, Energy and Education pilot

### Community 8 - "Planning Documents"
Cohesion: 0.67
Nodes (3): Frontier Product Discovery, Frontier Interaction Inventory, Frontier Policy Matrix

## Ambiguous Edges - Review These
- `Unresolved Active Capacity Redistribution` → `Production-Energy-Education Pilot`  [AMBIGUOUS]
  docs/systems/policy-matrix.md · relation: conceptually_related_to
- `Real-time game clock and bounded action durations` → `Open interaction decisions`  [AMBIGUOUS]
  docs/product/interaction-inventory.md · relation: conceptually_related_to

## Knowledge Gaps
- **3 isolated node(s):** `Policy Matrix`, `Frontier Product Discovery`, `Frontier Policy Matrix`
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 22 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **2 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Unresolved Active Capacity Redistribution` and `Production-Energy-Education Pilot`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Real-time game clock and bounded action durations` and `Open interaction decisions`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `Frontier` connect `Frontier Governance Time` to `Traceability Fauna Policies`, `Health Combat Colonists`, `Autonomy and Production`?**
  _High betweenness centrality (0.135) - this node is a cross-community bridge._
- **Why does `Combat` connect `Health Combat Colonists` to `Traceability Fauna Policies`, `Frontier Governance Time`?**
  _High betweenness centrality (0.128) - this node is a cross-community bridge._
- **Why does `Research and Technology` connect `Frontier Governance Time` to `Health Combat Colonists`, `Autonomy and Production`, `Research Model`?**
  _High betweenness centrality (0.113) - this node is a cross-community bridge._
- **What connects `Policy Matrix`, `Frontier Product Discovery`, `Frontier Policy Matrix` to the rest of the system?**
  _3 weakly-connected nodes found - possible documentation gaps or missing edges._