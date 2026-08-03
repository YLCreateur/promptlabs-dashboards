# Graph Report - /workspace  (2026-07-24)

## Corpus Check
- cluster-only mode — file stats not available

## Summary
- 17 nodes · 14 edges · 4 communities (3 shown, 1 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Martinique Accounting Prospects
- YLC Agent Auditeur
- Radar IA Remote 8 juillet 2026
- Doctrine Commerciale YLC Prompt Labs v2.0

## God Nodes (most connected - your core abstractions)
1. `Dashboard Experts Comptables Martinique` - 5 edges
2. `YLC Agent Auditeur` - 5 edges
3. `Radar IA Remote 8 juillet 2026` - 2 edges
4. `Radar IA Remote 13 juillet 2026` - 2 edges
5. `Doctrine Commerciale YLC Prompt Labs v2.0 (Condensé)` - 2 edges
6. `Grille Tarifaire YLC v2.0` - 2 edges
7. `Email Prospect Deloitte Martinique` - 1 edges
8. `Email Prospect Mazars Martinique` - 1 edges
9. `Email Prospect FIDUCIAL Fort-de-France` - 1 edges
10. `PromptLabs Dashboard Opportunités IA` - 1 edges

## Surprising Connections (you probably didn't know these)
- `Email Prospect Deloitte Martinique` --references--> `Dashboard Experts Comptables Martinique`  [EXTRACTED]
  preview_campagne_martinique.html → experts_comptables_martinique.html
- `Email Prospect FIDUCIAL Fort-de-France` --references--> `Dashboard Experts Comptables Martinique`  [EXTRACTED]
  preview_campagne_martinique.html → experts_comptables_martinique.html
- `Email Prospect Mazars Martinique` --references--> `Dashboard Experts Comptables Martinique`  [EXTRACTED]
  preview_campagne_martinique.html → experts_comptables_martinique.html
- `Radar IA Martinique 21 juillet 2026` --references--> `Dashboard Experts Comptables Martinique`  [EXTRACTED]
  radar_ia_martinique_lundi_20260721.html → experts_comptables_martinique.html
- `Séquence Prospection Experts Comptables Martinique` --references--> `Dashboard Experts Comptables Martinique`  [EXTRACTED]
  sequence_prospection_experts_comptables.html → experts_comptables_martinique.html

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **YLC Families A, B, C and sublevels** — ylc_agent_auditeur_references_doctrine_v2 [EXTRACTED 1.00]
- **Cadrage Payant Process and Deliverables** — ylc_agent_auditeur_references_doctrine_v2, ylc_agent_auditeur_assets_templates_devis_cadrage [EXTRACTED 1.00]
- **Phase 2 Devis Process and Clauses** — ylc_agent_auditeur_references_doctrine_v2, ylc_agent_auditeur_assets_templates_devis_phase2 [EXTRACTED 1.00]

## Communities (4 total, 1 thin omitted)

### Community 0 - "Martinique Accounting Prospects"
Cohesion: 0.33
Nodes (6): Dashboard Experts Comptables Martinique, Email Prospect Deloitte Martinique, Email Prospect FIDUCIAL Fort-de-France, Email Prospect Mazars Martinique, Radar IA Martinique 21 juillet 2026, Séquence Prospection Experts Comptables Martinique

### Community 1 - "YLC Agent Auditeur"
Cohesion: 0.40
Nodes (6): YLC Agent Auditeur, Template Devis Audit Express, Template Devis Cadrage Payant, Template Devis Phase 2 Famille B ou C, Doctrine Commerciale YLC Prompt Labs v2.0 (Condensé), Grille Tarifaire YLC v2.0

### Community 2 - "Radar IA Remote 8 juillet 2026"
Cohesion: 0.50
Nodes (4): PromptLabs Dashboard Opportunités IA, Radar IA Remote 8 juillet 2026, Radar IA Remote 13 juillet 2026, Radar IA Remote 20 juillet 2026

## Knowledge Gaps
- **11 isolated node(s):** `Email Prospect Deloitte Martinique`, `Email Prospect Mazars Martinique`, `Email Prospect FIDUCIAL Fort-de-France`, `PromptLabs Dashboard Opportunités IA`, `Radar IA Martinique 21 juillet 2026` (+6 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What connects `Email Prospect Deloitte Martinique`, `Email Prospect Mazars Martinique`, `Email Prospect FIDUCIAL Fort-de-France` to the rest of the system?**
  _11 weakly-connected nodes found - possible documentation gaps or missing edges._