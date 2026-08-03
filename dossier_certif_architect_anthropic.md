# Préparation Certification Claude Certified Architect — Dossier Notebook LM
# Compilé par Hermes Agent × PromptLabs — 30 juillet 2026

---

## SOURCE 1 : Four role-based certifications (Anthropic Blog — 23 juillet 2026)
Source : https://claude.com/blog/four-role-based-claude-certifications

Anthropic lance 4 certifications :
- Claude Certified Associate: Foundations — usage quotidien de Claude pour tous
- Claude Certified Developer: Foundations — ingénieurs, API Claude, tool use, agents
- Claude Certified Architect: Professional — architecture intégration, gouvernance, évaluation, scale entreprise
- Claude Certified Architect: Foundations — conception d'agents avec Claude

⚠️ Important : Le parcours Architect a DEUX niveaux :
1. Architect FOUNDATIONS (design et build agents)
2. Architect PROFESSIONAL (architecture entreprise, gouvernance, évaluation)

36 000 consultants certifiés, 1 300 organisations, 400 000 personnes formées en 2026.

---

## SOURCE 2 : Getting good at Claude — A research-backed curriculum
Source : https://claude.com/resources/tutorials/getting-good-at-claude-a-research-backed-curriculum

### Le "signature move" par produit
- **Chat** : ITÉRER. Les utilisateurs qui raffinent par des tours de suivi performent mieux sur TOUS les indicateurs.
- **Claude Code / Cowork** : CLARIFIER L'OBJECTIF. Énoncer clairement le but avant que Claude ne commence.

### Le spectre Description (compétences qui se développent naturellement)
Les compétences de Description (spécifier le format, définir le style, décomposer les tâches) se développent de façon organique et non-linéaire avec le temps.

### Le spectre Evaluation (compétences qui nécessitent un enseignement délibéré)
Les compétences d'Évaluation (vérification critique, détection d'erreurs, test des sorties) ne se développent PAS naturellement. Elles doivent être ENSEIGNÉES activement.

### Modèle de curriculum recommandé
1. Enseigner le "signature move" d'abord (itérer sur Chat, clarifier sur Code)
2. Laisser les compétences de Description se développer naturellement
3. Enseigner ACTIVEMENT les compétences d'Évaluation (vérification, test)
4. Introduire les cas d'usage avancés progressivement

---

## SOURCE 3 : Claude Code Overview
Source : https://docs.anthropic.com/en/docs/claude-code/overview

Claude Code = outil de coding agentic (lit le codebase, édite des fichiers, exécute des commandes, s'intègre aux outils de dev).

### Installation
macOS/Linux/WSL : `curl -fsSL https://claude.ai/install.sh | bash`
Windows PowerShell : `irm https://claude.ai/install.ps1 | iex`
Homebrew : `brew install --cask claude-code`

### Key concepts
- Compréhension du codebase entier
- Édition multi-fichiers
- Exécution de commandes shell
- Intégration IDE (VS Code, JetBrains)
- Mode agent autonome
- CLAUDE.md pour configuration projet

---

## SOURCE 4 : Concepts clés pour l'examen Architect

### Architecture Claude
- Claude API (Anthropic SDK) : messages, streaming, tool use
- Claude Code : agent de coding en terminal
- Claude Cowork : intégration entreprise (Google Workspace, etc.)
- Claude Chat : interface conversationnelle

### Bonnes pratiques API
- Prompt engineering structuré (system prompt + user messages)
- Tool use / function calling
- Prompt caching pour réduire les coûts
- Gestion des tokens et contexte
- Rate limiting et retry logic
- Streaming vs batch processing

### Gouvernance et sécurité (Architect Professional)
- Gestion des clés API
- Data residency
- Audit logging
- RBAC (Role-Based Access Control)
- Content filtering / safety
- Évaluation et testing

### Patterns de conception
- RAG (Retrieval-Augmented Generation)
- Agents multi-étapes (tool use en chaîne)
- Prompt chaining
- Human-in-the-loop
- Fallback et graceful degradation

---

## SOURCE 5 : Questions probables à l'examen Architect

1. Quel est le "signature move" pour Claude Code ?
2. Quelles compétences se développent naturellement vs nécessitent un enseignement ?
3. Différence entre token, prompt caching et context window ?
4. Comment structurer un appel API avec tool use ?
5. Quels sont les 4 rôles de certification Anthropic ?
6. Quelle est la différence entre Architect Foundations et Professional ?
7. Comment configurer un CLAUDE.md dans un projet ?
8. Quels mécanismes de sécurité pour les déploiements entreprise ?
9. Comment évaluer la qualité d'un système basé sur Claude ?
10. Patterns pour le déploiement d'agents autonomes ?

---

## Planning d'étude recommandé (1 semaine)

| Jour | Contenu | Durée |
|---|---|---|
| LUN | Lire ce dossier + écouter Audio Overview Notebook LM | 1h30 |
| MAR | Getting good at Claude + signature moves | 2h |
| MER | Claude Code overview + pratique CLI | 2h30 |
| JEU | API Claude + tool use + prompt caching | 3h |
| VEN | Gouvernance, sécurité, patterns Architect | 2h |
| SAM | Simulateur d'examen (20 questions) + révision | 2h |
| DIM | Examen certifiant | 1h |

---

Note : Ce dossier couvre ~70% du programme Architect. Les 30% restants se trouvent dans les cours Skilljar (accessibles après inscription).