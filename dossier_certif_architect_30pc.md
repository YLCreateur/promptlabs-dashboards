# Certification Claude Architect — Les 30% restants
# À ajouter à ton Notebook LM après le premier dossier
# Compilé par Hermes × PromptLabs — 30 juillet 2026

---

## MODULE 1 : Claude API Masterclass (10% du programme)

### Les 3 modes d'appel API
- **Messages API** : envoi simple, réponse unique
- **Streaming** : réponse mot par mot (meilleure UX)
- **Batch** : traitement asynchrone, 50% moins cher

### Tool Use / Function Calling
Claude peut appeler des fonctions externes. Flux :
1. Vous décrivez les outils disponibles (nom, description, schéma JSON)
2. Claude décide SI et QUEL outil appeler
3. Vous exécutez l'outil et renvoyez le résultat
4. Claude intègre le résultat dans sa réponse

Pièges classiques exam :
- Toujours valider les arguments avant exécution
- Gérer le cas où Claude n'appelle PAS d'outil
- Limiter le nombre d'appels en boucle (max_turns)

### Prompt Caching
- Réduit les coûts de 90% sur les longs prompts
- Marquer les blocs récurrents avec `cache_control: {"type": "ephemeral"}`
- Points d'ancrage : min 1024 tokens, max 4 blocs
- Valable 5 minutes, réinitialisé à chaque appel

### Token Management
- 1 token ≈ 0.75 mot en anglais, 0.5 mot en français
- Modèles : Haiku (rapide/pas cher), Sonnet (équilibré), Opus (puissant)
- Context window : nombre max de tokens que Claude peut traiter (200K pour Sonnet)
- Max output tokens : limite configurable de la réponse

### Rate Limiting & Retry
- Erreur 429 = rate limit
- Stratégie : exponential backoff (1s, 2s, 4s, 8s…)
- Utiliser `max_retries` dans le SDK
- Gérer les erreurs 5xx (service unavailable)

---

## MODULE 2 : Agents & Systems Design (10% du programme)

### Architecture d'un agent Claude
```
User → Orchestrator → Claude (plan) → Tool 1 → Claude (analyse) → Tool 2 → Response
```

### Patterns essentiels
- **Prompt Chaining** : sortie Claude 1 → entrée Claude 2
- **Router** : un Claude classifie → aiguille vers le bon sous-agent
- **Parallelization** : plusieurs Claude travaillent simultanément
- **Orchestrator-Workers** : un chef + des exécutants
- **Evaluator-Optimizer** : un Claude produit, un autre évalue

### Human-in-the-Loop
- Arrêter l'agent avant une action destructive (delete, send email, publish)
- Demander confirmation pour les montants > seuil
- Logguer toutes les décisions pour audit

### Memory & State
- Court terme : conversation history
- Long terme : base vectorielle (RAG), base SQL, file system
- Session state : variables persistantes entre appels

---

## MODULE 3 : Évaluation & Testing (5% du programme)

### Comment évaluer un système Claude
- **Accuracy** : la réponse est-elle correcte ?
- **Hallucination rate** : % de faits inventés
- **Tool selection accuracy** : le bon outil est-il choisi ?
- **Latency** : temps de réponse (P50, P95, P99)
- **Cost per request** : tokens in + tokens out

### Méthodes d'évaluation
- **Golden dataset** : 50-200 questions avec réponses attendues
- **LLM-as-judge** : Claude Opus évalue les réponses de Claude Haiku
- **A/B testing** : comparer deux prompts ou modèles
- **Human eval** : échantillon vérifié manuellement

### Prompt Evaluation Framework
```
1. Définir la tâche (classification, extraction, génération…)
2. Créer 20+ exemples variés
3. Définir les critères de succès (binaire ou score 1-5)
4. Runner le prompt sur tous les exemples
5. Calculer le accuracy score
6. Itérer sur le prompt → réévaluer
```

---

## MODULE 4 : Déploiement Entreprise (5% du programme)

### Gouvernance
- **RBAC** : qui peut utiliser quel modèle, quel budget
- **API Keys** : rotation, scope limité par projet
- **Audit logging** : tracer chaque appel (qui, quand, quel modèle, combien de tokens)

### Sécurité
- **Content filtering** : bloquer les contenus dangereux
- **PII detection** : ne pas envoyer de données personnelles
- **Data residency** : où sont traitées les données (US, EU)
- **Prompt injection** : utiliser le template défensif PromptLabs

### Monitoring
- Dashboards de consommation (tokens, coûts, latence)
- Alertes : pic d'erreurs, dépassement budget
- Health checks : endpoints, taux de succès

### Stratégie de déploiement
1. **Shadow mode** : l'IA tourne sans affecter les utilisateurs
2. **Canary release** : 5% du trafic → 25% → 100%
3. **Rollback** : procédure de retour en arrière
4. **Circuit breaker** : couper automatiquement si taux d'erreur > seuil

---

## MODULE 5 : Cas pratiques type examen (questions scénario)

### Scénario 1 : Migration coûteuse
*Une entreprise dépense $500/jour en appels API. Comment réduire de 70% ?*
→ Prompt caching (90% sur blocs récurrents) + batch processing (50%) + Haiku au lieu de Sonnet pour tâches simples.

### Scénario 2 : Agent qui boucle
*Un agent appelle le même outil 50 fois sans avancer. Comment corriger ?*
→ max_turns=5 + tool description plus précise + prompt qui dit "si tu n'as pas trouvé après 3 essais, demande de l'aide".

### Scénario 3 : Hallucination en prod
*Un client se plaint que Claude invente des chiffres. Quelle solution ?*
→ Ajouter "Cite tes sources" dans le prompt + utiliser RAG avec documents vérifiés + ajouter un evaluator agent.

### Scénario 4 : Déploiement Grande Banque
*Une banque veut déployer Claude pour 5000 employés. Quels points clés ?*
→ Data residency (on-prem ou EU), RBAC par département, audit logging obligatoire, content filtering, PII detection, circuit breaker.

### Scénario 5 : Choix du modèle
*Tâche : classification de 100K emails/heure. Quel modèle ?*
→ Haiku (pas cher, rapide, assez bon pour classification). Batch mode pour -50%.

---

## Quick Review — Les 20 concepts qui tombent à l'examen

| # | Concept | Poids estimé |
|---|---|---|
| 1 | Différence Haiku / Sonnet / Opus | ★★★★★ |
| 2 | Tool use (function calling) | ★★★★★ |
| 3 | Prompt caching (quand, comment) | ★★★★ |
| 4 | Streaming vs Batch | ★★★★ |
| 5 | Token management (context window) | ★★★★ |
| 6 | 4 certifications Anthropic | ★★★★ |
| 7 | Signature moves (Chat=itérer, Code=clarifier) | ★★★★ |
| 8 | Evaluation vs Description skills | ★★★★ |
| 9 | RAG architecture | ★★★ |
| 10 | Agent patterns (Orchestrator-Workers) | ★★★ |
| 11 | Human-in-the-loop | ★★★ |
| 12 | Rate limiting 429 + backoff | ★★★ |
| 13 | Content filtering / safety | ★★★ |
| 14 | RBAC & API key management | ★★★ |
| 15 | LLM-as-judge evaluation | ★★ |
| 16 | Circuit breaker pattern | ★★ |
| 17 | Prompt chaining | ★★ |
| 18 | Data residency (US vs EU) | ★★ |
| 19 | Claude Code vs Claude API vs Chat | ★★ |
| 20 | Golden dataset pour évaluation | ★★ |

---

## Plan d'action final

1. Ajoute ce fichier à ton Notebook LM (2e source)
2. Demande : *« Compare les deux sources et identifie les concepts qui apparaissent dans les deux. Ceux-là tombent à coup sûr à l'examen. »*
3. Demande : *« Génère 25 questions difficiles couvrant les 20 concepts clés. »*
4. Passe l'examen blanc, identifie tes faiblesses
5. Révise UNIQUEMENT les concepts faibles (pas tout)
6. Passe l'examen certifiant