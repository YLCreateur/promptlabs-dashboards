# Template — Devis Phase 2 (Famille B ou C)

Instructions d'usage : ce template est utilisé après le cadrage payant (obligatoire pour B3 et C, recommandé pour B2). Il présente la solution retenue avec chiffrage détaillé setup + récurrent, intègre les clauses infra client + AI Act, et déduit systématiquement le montant du cadrage préalable si signature <60 jours.

---

## Métadonnées

- **Numéro devis** : YLC-[YYYY]-[XXX]
- **Devis de cadrage antérieur** : YLC-[YYYY]-[XXX] du [date] (le cas échéant, à mentionner)
- **Date** : [JJ mois AAAA]
- **Validité** : 30 jours calendaires
- **Nature** : Phase 2 — [Famille + description brève : ex. "Famille C2 — Sales Closer stratégique"]

## Bloc émetteur

**YLC Prompt Labs**
Youri Le Creau, fondateur
[Adresse Martinique]
[Email] · [Téléphone]
SIRET : [à remplir]
TVA non applicable, art. 293 B du CGI

## Bloc client

**[Raison sociale client]**
À l'attention de [Prénom Nom, fonction signataire]
[Adresse complète]
SIRET : [SIRET client si connu]

## Contexte de la mission

[Prose 4-6 lignes rappelant : le cadrage antérieur, la variante retenue par le client, la nature de la solution proposée, la temporalité de mise en œuvre.]

Exemple type :
> À l'issue du cadrage préalable YLC-[NN] remis le [date], [Raison sociale] a retenu la variante [Variante N] présentée dans le livrable de cadrage. Le présent devis engage YLC Prompt Labs sur la conception, le développement et le déploiement de [description synthétique de la solution] selon les termes définis ci-après. Le cadrage antérieur étant signé dans les 60 jours calendaires, son montant est intégralement déduit du setup ci-dessous, conformément à la clause de déductibilité du devis YLC-[NN].

## Solution retenue

**Famille et palier** : [ex. Famille C2 — Agent autonome complexe]

**Description fonctionnelle**
[Prose 5-10 lignes décrivant ce que fait la solution, ses cas d'usage, les intégrations, les points d'interaction avec l'écosystème client.]

**Architecture technique**
[Bullets décrivant la stack technique, les outils utilisés, l'infrastructure requise]
- Orchestration : [ex. n8n self-hosted]
- Modèles LLM : [ex. API Anthropic Claude Sonnet]
- Base vectorielle : [ex. Pinecone / Weaviate / Postgres pgvector]
- Intégrations : [liste des outils client à intégrer]

**Livrables**
- [Bullet 1 : livrable technique concret]
- [Bullet 2 : documentation associée]
- [Bullet 3 : formation des utilisateurs internes]
- [Bullet 4 : notice de transparence AI Act le cas échéant]
- [Bullet 5 : période de recette]

**Hors périmètre**
- [Ce qui n'est pas inclus, à distinguer clairement]

## Chiffrage

### Setup — investissement initial

| Poste | Montant HT |
|---|---|
| Setup [Palier retenu] | [MONTANT] € HT |
| Ligne conformité AI Act (Famille C uniquement, à moduler selon palier) | [MONTANT ou "Inclus"] |
| Sous-total setup | **[SOUS-TOTAL] € HT** |
| Déduction cadrage antérieur YLC-[NN] (signature <60 jours) | -[MONTANT CADRAGE] € HT |
| **Total setup à régler** | **[TOTAL FINAL] € HT** |

**Application des fourchettes** (à consulter dans `grille_tarifaire.md`) :
- Fourchette territoriale YLC si client Martinique/Guadeloupe TPE-PME
- Fourchette référence marché européen sinon

### Récurrent mensuel — accompagnement

| Poste | Montant HT/mois |
|---|---|
| Récurrent mensuel [Palier retenu] — supervision + itérations + corrections | **[MONTANT] € HT/mois** |

Note : le récurrent YLC couvre exclusivement la prestation d'accompagnement. Les coûts d'infrastructure sont portés directement par le client sur ses propres comptes (voir clause dédiée ci-dessous).

**Engagement minimum recommandé** : 12 mois. Une clause de sortie mutuelle à 6 mois peut être prévue sur demande, avec préavis de 30 jours.

TVA non applicable, article 293 B du CGI.

## Modalités de paiement

**Setup** — échelonnement en trois versements :
- **30 % à la signature** du présent devis (déclenche le démarrage des travaux)
- **40 % à mi-parcours** (validation d'une étape clé définie en début de mission)
- **30 % à la livraison finale** (recette validée)

**Récurrent** — facturation mensuelle
- Facturation le 1er de chaque mois pour le mois en cours
- Règlement par virement bancaire sous 15 jours calendaires à réception de facture
- Prélèvement SEPA disponible sur demande

Coordonnées bancaires : [RIB YLC à joindre en annexe]

## Calendrier prévisionnel

- **Semaine 0** : signature devis + acompte 30 %
- **Semaines 1 à [N-2]** : conception + développement itératif
- **Semaine [N-1]** : recette client
- **Semaine [N]** : mise en production
- **Mois +1** : premier mois de récurrent, période d'ajustement fin

Durée totale estimée : **[X à Y semaines]** (voir grille : C1 3-5 sem, C2 6-8 sem, C3 8-12 sem).

## Clauses techniques et juridiques

### Infrastructure sur comptes client

Conformément à la doctrine YLC Prompt Labs et aux termes explicités lors du cadrage préalable, **le client porte l'intégralité des coûts d'infrastructure sur ses propres comptes** :

- API LLM (comptes Anthropic, OpenAI, Mistral selon architecture retenue)
- Hébergement de la plateforme d'orchestration (VPS, cloud ou n8n Cloud)
- Base vectorielle et stockage associé
- Plateforme agréée de facturation électronique le cas échéant
- Tout autre service tiers nécessaire au fonctionnement de la solution

Une estimation prévisionnelle des coûts mensuels d'infrastructure a été détaillée dans le livrable de cadrage antérieur. YLC accompagne la création des comptes et le paramétrage initial ; le client conserve la propriété et l'administration de ses environnements.

YLC ne peut être tenu responsable des interruptions de service liées à un défaut de règlement des services d'infrastructure côté client.

### Conformité AI Act (Famille C uniquement)

La solution proposée relève du règlement européen sur l'intelligence artificielle (AI Act). YLC intègre les livrables de conformité suivants :

- Notice de transparence utilisateur (Article 50) applicable au 2 novembre 2026 le cas échéant
- Documentation technique du système IA
- Journalisation des interactions conformément aux exigences RGPD et AI Act
- Point de supervision humaine documenté

Le statut juridique de chaque partie a été qualifié lors du cadrage : [Raison sociale] en tant que [déployeur / fournisseur] et YLC Prompt Labs en tant que [fournisseur / prestataire technique].

### Propriété intellectuelle

Le code source, les configurations, les prompts et les artefacts techniques développés dans le cadre de la présente mission sont livrés au client à la fin de la mission. Le client dispose d'un droit d'usage complet sur ces éléments. YLC conserve le droit de réutiliser les méthodologies, patterns et briques techniques génériques développés à l'occasion de la mission.

### Confidentialité

YLC s'engage à respecter la confidentialité de toute information communiquée dans le cadre de la mission, pendant toute la durée de la relation contractuelle et pendant 3 ans après son terme.

### Résiliation

- Le récurrent mensuel peut être résilié par l'une ou l'autre des parties avec un préavis de 30 jours calendaires, à compter du 7e mois si engagement 12 mois retenu
- En cas de résiliation par le client avant la fin de l'engagement minimum, les mensualités restantes ne sont pas dues, mais le récurrent en cours reste facturé jusqu'à la fin du mois de préavis
- En cas de résiliation par YLC pour motif grave (défaut de paiement, atteinte à la réputation), aucun remboursement n'est dû

## Signatures

| Pour YLC Prompt Labs | Pour [Raison sociale client] |
|---|---|
| Youri Le Creau | [Nom du signataire] |
| Fondateur | [Fonction] |
| Date : | Date : |
| Signature (précédée de "Bon pour accord") : | Signature (précédée de "Bon pour accord") : |

---

## Instructions pour l'Agent Auditeur lors de la génération DOCX

1. Génère un fichier .docx dans `/mnt/user-data/outputs/Devis_Phase2_[NomClient]_[Palier]_[YYYYMMDD].docx`
2. Applique strictement la charte YLC
3. Le **tableau de chiffrage** doit faire apparaître visuellement la déduction du cadrage antérieur (ligne rouge/muted)
4. Les **clauses infrastructure client** et **AI Act** doivent être mises en avant (callout amber pour la clause infra client, encart navy pour AI Act)
5. Ne mentionne jamais "décote" ou "rabais"
6. Génère aussi le PDF miroir via LibreOffice
7. Livre les deux fichiers via `present_files`
