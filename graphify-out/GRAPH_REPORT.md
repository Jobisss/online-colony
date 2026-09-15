# Graph Report - online-colony  (2026-09-15)

## Corpus Check
- Corpus is ~17,240 words - fits in a single context window. You may not need a graph.

## Summary
- 89 nodes · 116 edges · 12 communities (10 shown, 2 thin omitted)
- Extraction: 78% EXTRACTED · 20% INFERRED · 2% AMBIGUOUS · INFERRED: 23 edges (avg confidence: 0.82)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Core Systems and Research
- Traceability and Consistency
- Research Education and Core Loop
- Research Decisions
- Governance and Autonomy
- Policy Model
- Time and Open Questions
- Health and Skills
- Sector Policies
- Planning Documents
- Colony
- Policy Matrix

## God Nodes (most connected - your core abstractions)
1. `Frontier` - 10 edges
2. `Combat` - 9 edges
3. `Research` - 9 edges
4. `Production` - 8 edges
5. `Autonomy and Execution` - 5 edges
6. `Consistency Audit` - 5 edges
7. `Regional fauna` - 5 edges
8. `Education` - 5 edges
9. `Job System` - 5 edges
10. `Policy` - 5 edges

## Surprising Connections (you probably didn't know these)
- `Graph traceability project instruction` --references--> `Graph Traceability`  [EXTRACTED]
  AGENTS.md → docs/architecture/graph-traceability.md
- `Graph traceability project instruction` --references--> `Incremental impact graph update`  [EXTRACTED]
  AGENTS.md → docs/architecture/graph-traceability.md
- `Production–Energy–Education Core Loop` --rationale_for--> `Research and Specialization`  [INFERRED]
  docs/product/discovery.md → docs/systems/policy-matrix.md
- `Policy-to-Outcome Pipeline` --implements--> `Policy`  [INFERRED]
  docs/systems/policy-matrix.md → docs/systems/colony-governance.md
- `Real-time game clock and bounded action durations` --conceptually_related_to--> `Open interaction decisions`  [AMBIGUOUS]
  docs/product/discovery.md → docs/product/interaction-inventory.md

## Hyperedges (group relationships)
- **Consistency Audit Requirements** — agents_consistency_audit, contradiction_checking, resolved_open_decision_conflicts, cross_community_connections, ambiguous_relation_review, affected_files_reporting [EXTRACTED 1.00]

## Communities (12 total, 2 thin omitted)

### Community 0 - "Core Systems and Research"
Cohesion: 0.16
Nodes (18): Autonomy and Execution, Frontier, Logistics and Transport, Sector Policies, Production, Real-Time 1:1 Clock, Interaction Inventory, Colony Governance (+10 more)

### Community 1 - "Traceability and Consistency"
Cohesion: 0.17
Nodes (15): Graph traceability project instruction, Graph Traceability, Incremental impact graph update, Regional fauna, Combat, PendingDecision, Fauna interactions, CombatEntity (+7 more)

### Community 2 - "Research Education and Core Loop"
Cohesion: 0.19
Nodes (13): Colony Research Capability, Research, Single Research Queue, Neurology, Policy Capability, Research as Policy Expansion and Specialization, Individual Skill Formation, One Active Research at a Time (+5 more)

### Community 3 - "Research Decisions"
Cohesion: 0.31
Nodes (9): Unresolved Active Capacity Redistribution, docs_systems_colony_governance_document, docs_systems_policy_matrix_document, Limited Research Capacity and Specialization Trade-off, No Direct Research Transfer Through Contracts or Trade, Permanent Acquired Knowledge, Production-Energy-Education Pilot, Single Research Queue and One Active Research (+1 more)

### Community 4 - "Governance and Autonomy"
Cohesion: 0.39
Nodes (8): Affected Files Reporting, Consistency Audit, AMBIGUOUS Relation Review, Contradiction Checking, Cross-Community Connections, docs_architecture_graph_traceability, Impact Traversal, Resolved-vs-Open Decision Conflicts

### Community 5 - "Policy Model"
Cohesion: 0.29
Nodes (7): Research queue and permanent knowledge, Policy, PriorityRule, StockGoal, Single research queue interaction, Common Policy Contract, Research specialization and limited capacity

### Community 6 - "Time and Open Questions"
Cohesion: 0.50
Nodes (5): Real-time game clock and bounded action durations, Open product questions, Game-time durations in interactions, Open interaction decisions, Policy Matrix cross-document reference

### Community 7 - "Health and Skills"
Cohesion: 0.40
Nodes (5): Production–Infrastructure–Energy–Education core loop, Production–Energy–Education Core Loop, Initial Production–Infrastructure–Energy–Education chain, Production → Infrastructure → Energy → Education Chain, Production + Energy + Education Pilot

### Community 8 - "Sector Policies"
Cohesion: 0.50
Nodes (4): Health sequencing after the initial core loop, Individual Colonist, Health as basic support in the first cycle, Health policy

### Community 9 - "Planning Documents"
Cohesion: 0.67
Nodes (3): Frontier Product Discovery, Frontier Interaction Inventory, Frontier Policy Matrix

## Ambiguous Edges - Review These
- `Unresolved Active Capacity Redistribution` → `Production-Energy-Education Pilot`  [AMBIGUOUS]
  docs/systems/policy-matrix.md · relation: conceptually_related_to
- `Real-time game clock and bounded action durations` → `Open interaction decisions`  [AMBIGUOUS]
  docs/product/interaction-inventory.md · relation: conceptually_related_to

## Knowledge Gaps
- **3 isolated node(s):** `Policy Matrix`, `Frontier Product Discovery`, `Frontier Policy Matrix`
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 24 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **2 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Unresolved Active Capacity Redistribution` and `Production-Energy-Education Pilot`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Real-time game clock and bounded action durations` and `Open interaction decisions`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `Research` connect `Research Education and Core Loop` to `Core Systems and Research`, `Traceability and Consistency`, `Policy Model`?**
  _High betweenness centrality (0.219) - this node is a cross-community bridge._
- **Why does `Combat` connect `Traceability and Consistency` to `Sector Policies`, `Core Systems and Research`, `Research Education and Core Loop`?**
  _High betweenness centrality (0.115) - this node is a cross-community bridge._
- **Are the 3 inferred relationships involving `docs_architecture_graph_traceability` (e.g. with `Contradiction Checking` and `Resolved-vs-Open Decision Conflicts`) actually correct?**
  _`docs_architecture_graph_traceability` has 3 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Policy Matrix`, `Frontier Product Discovery`, `Frontier Policy Matrix` to the rest of the system?**
  _3 weakly-connected nodes found - possible documentation gaps or missing edges._