# Graph Report - online-colony  (2026-09-15)

## Corpus Check
- Corpus is ~16,421 words - fits in a single context window. You may not need a graph.

## Summary
- 41 nodes · 59 edges · 7 communities (6 shown, 1 thin omitted)
- Extraction: 86% EXTRACTED · 14% INFERRED · 0% AMBIGUOUS · INFERRED: 8 edges (avg confidence: 0.84)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Governance e Produção
- Pesquisa e Especialização
- Fauna e Políticas Setoriais
- Colonos e Consequências
- Núcleo de Governança
- Combate e Defesa
- Colônia

## God Nodes (most connected - your core abstractions)
1. `Frontier` - 10 edges
2. `Combat` - 9 edges
3. `Production` - 8 edges
4. `Research and Technology` - 7 edges
5. `Autonomy and Execution` - 5 edges
6. `Policy` - 5 edges
7. `Job System` - 5 edges
8. `Colonist` - 4 edges
9. `Regional Fauna` - 4 edges
10. `Logistics and Transport` - 4 edges

## Surprising Connections (you probably didn't know these)
- `Frontier` --references--> `Interaction Inventory`  [EXTRACTED]
  docs/product/discovery.md → docs/product/interaction-inventory.md
- `Policy` --implements--> `Policy-to-Outcome Pipeline`  [INFERRED]
  docs/systems/colony-governance.md → docs/systems/policy-matrix.md
- `Policy` --references--> `Research Specialization`  [INFERRED]
  docs/systems/colony-governance.md → docs/systems/policy-matrix.md
- `Colony Governance` --references--> `Policy Matrix`  [INFERRED]
  docs/systems/colony-governance.md → docs/systems/policy-matrix.md
- `Research Interactions` --implements--> `Research and Technology`  [EXTRACTED]
  docs/product/interaction-inventory.md → docs/product/discovery.md

## Hyperedges (group relationships)
- **Policy to Autonomous Execution Chain** — governance_policy, governance_priority_rule, inventory_demand_system, inventory_job_system, docs_product_discovery_colonist [EXTRACTED 1.00]
- **Research Specialization Dependencies** — docs_product_discovery_research, policy_health, policy_education, policy_security, policy_production, policy_energy, docs_product_discovery_logistics [EXTRACTED 1.00]
- **Composable Combat Entity** — inventory_combat_entity, docs_product_discovery_colonist, docs_product_discovery_fauna, inventory_defense, docs_product_discovery_combat [EXTRACTED 1.00]

## Communities (7 total, 1 thin omitted)

### Community 0 - "Governance e Produção"
Cohesion: 0.31
Nodes (9): Autonomy and Execution, Frontier, Logistics and Transport, Sector Policies, Production, ColonyOrder, Governance Explanation, Ownership, Custody and Reservation (+1 more)

### Community 1 - "Pesquisa e Especialização"
Cohesion: 0.25
Nodes (8): Research and Technology, Policy, PriorityRule, StockGoal, Research Interactions, Common Policy Contract, Education Policy, Research Specialization

### Community 2 - "Fauna e Políticas Setoriais"
Cohesion: 0.29
Nodes (7): Regional Fauna, Fauna Interactions, Energy Policy, Fauna Policy, Production Policy, Security Policy, Security Sector

### Community 3 - "Colonos e Consequências"
Cohesion: 0.40
Nodes (6): Colonist, BuildPlan, Demand System, Job System, Health Policy, Policy-to-Outcome Pipeline

### Community 4 - "Núcleo de Governança"
Cohesion: 0.33
Nodes (6): Real-Time 1:1 Clock, Interaction Inventory, Colony Governance, Policy Matrix, Directive, Offline Operation

### Community 5 - "Combate e Defesa"
Cohesion: 0.67
Nodes (4): Combat, PendingDecision, CombatEntity, Defense Interactions

## Knowledge Gaps
- **1 isolated node(s):** `Policy Matrix`
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 15 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Frontier` connect `Governance e Produção` to `Pesquisa e Especialização`, `Fauna e Políticas Setoriais`, `Colonos e Consequências`, `Núcleo de Governança`, `Combate e Defesa`?**
  _High betweenness centrality (0.268) - this node is a cross-community bridge._
- **Why does `Combat` connect `Combate e Defesa` to `Governance e Produção`, `Pesquisa e Especialização`, `Fauna e Políticas Setoriais`, `Colonos e Consequências`, `Núcleo de Governança`?**
  _High betweenness centrality (0.257) - this node is a cross-community bridge._
- **Why does `Research and Technology` connect `Pesquisa e Especialização` to `Governance e Produção`, `Núcleo de Governança`, `Combate e Defesa`?**
  _High betweenness centrality (0.209) - this node is a cross-community bridge._
- **What connects `Policy Matrix` to the rest of the system?**
  _1 weakly-connected nodes found - possible documentation gaps or missing edges._