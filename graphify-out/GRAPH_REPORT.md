# Graph Report - online-colony  (2026-09-15)

## Corpus Check
- Corpus is ~17,349 words - fits in a single context window. You may not need a graph.

## Summary
- 102 nodes · 141 edges · 11 communities (9 shown, 2 thin omitted)
- Extraction: 81% EXTRACTED · 17% INFERRED · 2% AMBIGUOUS · INFERRED: 24 edges (avg confidence: 0.82)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Research Education and Transition
- Core Systems
- Core Loop and Health
- Governance and Policy Model
- Traceability and Fauna
- Research Decisions
- Consistency Audit
- Time and Open Questions
- Neurology Capability Flow
- Planning Documents
- Colony

## God Nodes (most connected - your core abstractions)
1. `Research and Technology` - 14 edges
2. `Frontier` - 10 edges
3. `Combat` - 9 edges
4. `Production` - 7 edges
5. `Active Specialization` - 6 edges
6. `Approved Specialization-Switch Rule` - 6 edges
7. `Health` - 5 edges
8. `Initial Core Loop` - 5 edges
9. `Autonomy and Execution` - 5 edges
10. `Individual Colonist` - 5 edges

## Surprising Connections (you probably didn't know these)
- `Health` --conceptually_related_to--> `Active Specialization`  [AMBIGUOUS]
  docs/systems/policy-matrix.md → docs/product/discovery.md
- `Policy` --implements--> `Policy-to-Outcome Pipeline`  [INFERRED]
  docs/systems/colony-governance.md → docs/systems/policy-matrix.md
- `Graph traceability project instruction` --references--> `Graph Traceability`  [EXTRACTED]
  AGENTS.md → docs/architecture/graph-traceability.md
- `Graph traceability project instruction` --references--> `Incremental impact graph update`  [EXTRACTED]
  AGENTS.md → docs/architecture/graph-traceability.md
- `Real-time game clock and bounded action durations` --conceptually_related_to--> `Open interaction decisions`  [AMBIGUOUS]
  docs/product/discovery.md → docs/product/interaction-inventory.md

## Hyperedges (group relationships)
- **Approved Specialization Switch** — docs_product_discovery_specialization_switch_rule, docs_product_discovery_acquired_knowledge, docs_product_discovery_active_specialization, docs_product_discovery_transition_cost_time, docs_product_discovery_old_area_efficiency, docs_product_discovery_new_area_low_efficiency, docs_product_discovery_individual_education [EXTRACTED 1.00]
- **Initial Specialization Core Loop** — docs_product_discovery_core_loop, discovery_production, discovery_energy, discovery_education, docs_product_discovery_research, discovery_health [EXTRACTED 1.00]
- **Research-to-Individual Capability Pipeline** — docs_product_discovery_research, discovery_education, docs_product_discovery_individual_education [EXTRACTED 1.00]

## Communities (11 total, 2 thin omitted)

### Community 0 - "Research Education and Transition"
Cohesion: 0.13
Nodes (22): Health sequencing after the initial core loop, Autonomy and Execution, Individual Colonist, Frontier, Logistics and Transport, Sector Policies, Production, Real-Time 1:1 Clock (+14 more)

### Community 1 - "Core Systems"
Cohesion: 0.22
Nodes (17): discovery_education, Energy, discovery_governance, Health, discovery_production, Acquired Knowledge, Active Specialization, Initial Core Loop (+9 more)

### Community 2 - "Core Loop and Health"
Cohesion: 0.17
Nodes (15): Graph traceability project instruction, Graph Traceability, Incremental impact graph update, Regional fauna, Combat, PendingDecision, Fauna interactions, CombatEntity (+7 more)

### Community 3 - "Governance and Policy Model"
Cohesion: 0.16
Nodes (14): Production–Infrastructure–Energy–Education core loop, Colony Research Capability, Production–Energy–Education Core Loop, Neurology, Policy Capability, Research as Policy Expansion and Specialization, Individual Skill Formation, Initial Production–Infrastructure–Energy–Education chain (+6 more)

### Community 4 - "Traceability and Fauna"
Cohesion: 0.31
Nodes (9): Unresolved Active Capacity Redistribution, docs_systems_colony_governance_document, docs_systems_policy_matrix_document, Limited Research Capacity and Specialization Trade-off, No Direct Research Transfer Through Contracts or Trade, Permanent Acquired Knowledge, Production-Energy-Education Pilot, Single Research Queue and One Active Research (+1 more)

### Community 5 - "Research Decisions"
Cohesion: 0.39
Nodes (8): Affected Files Reporting, Consistency Audit, AMBIGUOUS Relation Review, Contradiction Checking, Cross-Community Connections, docs_architecture_graph_traceability, Impact Traversal, Resolved-vs-Open Decision Conflicts

### Community 6 - "Consistency Audit"
Cohesion: 0.29
Nodes (7): Research queue and permanent knowledge, Policy, PriorityRule, StockGoal, Single research queue interaction, Common Policy Contract, Research specialization and limited capacity

### Community 7 - "Time and Open Questions"
Cohesion: 0.50
Nodes (5): Real-time game clock and bounded action durations, Open product questions, Game-time durations in interactions, Open interaction decisions, Policy Matrix cross-document reference

### Community 8 - "Neurology Capability Flow"
Cohesion: 0.67
Nodes (3): Frontier Product Discovery, Frontier Interaction Inventory, Frontier Policy Matrix

## Ambiguous Edges - Review These
- `Health` → `Active Specialization`  [AMBIGUOUS]
  docs/product/discovery.md · relation: conceptually_related_to
- `Unresolved Active Capacity Redistribution` → `Production-Energy-Education Pilot`  [AMBIGUOUS]
  docs/systems/policy-matrix.md · relation: conceptually_related_to
- `Real-time game clock and bounded action durations` → `Open interaction decisions`  [AMBIGUOUS]
  docs/product/interaction-inventory.md · relation: conceptually_related_to

## Knowledge Gaps
- **3 isolated node(s):** `Policy Matrix`, `Frontier Product Discovery`, `Frontier Policy Matrix`
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 25 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **2 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Health` and `Active Specialization`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Unresolved Active Capacity Redistribution` and `Production-Energy-Education Pilot`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Real-time game clock and bounded action durations` and `Open interaction decisions`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `Research and Technology` connect `Core Systems` to `Research Education and Transition`, `Core Loop and Health`, `Governance and Policy Model`, `Consistency Audit`?**
  _High betweenness centrality (0.286) - this node is a cross-community bridge._
- **Why does `Frontier` connect `Research Education and Transition` to `Core Systems`, `Core Loop and Health`?**
  _High betweenness centrality (0.153) - this node is a cross-community bridge._
- **Why does `Combat` connect `Core Loop and Health` to `Research Education and Transition`, `Core Systems`?**
  _High betweenness centrality (0.129) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `Research and Technology` (e.g. with `Health` and `Real-Time 1:1 Clock`) actually correct?**
  _`Research and Technology` has 2 INFERRED edges - model-reasoned connections that need verification._