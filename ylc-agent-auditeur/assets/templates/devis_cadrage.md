# Template — Devis Cadrage payant

Instructions d'usage : ce template est utilisé quand un projet dépasse la Famille A. Il est **obligatoire** pour B3 et pour toute Famille C. La clause de déductibilité 60 jours est un différenciateur majeur — elle doit toujours apparaître explicitement.

---

## Métadonnées

- **Numéro devis** : YLC-[YYYY]-[XXX]
- **Date** : [JJ mois AAAA]
- **Validité** : 30 jours calendaires
- **Nature** : Cadrage préalable — [description brève : ex. "Cadrage projet automatisation stock + reporting accises"]

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

[Prose 4-6 lignes reprenant : origine du contact / nature du besoin verbalisé / positionnement du cadrage comme préalable à tout engagement de setup / justification de la nécessité de qualifier le périmètre avant chiffrage ferme.]

Exemple type — cas distillerie :
> À l'issue de nos échanges du [date], [Raison sociale] a exprimé un besoin d'automatisation de sa gestion de stock, de son suivi des livraisons et de son reporting réglementaire (accises, DRM, capsules fiscales), assorti d'un chatbot WhatsApp de qualification client. La nature multi-processus de ce périmètre et les contraintes réglementaires spécifiques au secteur imposent une phase de cadrage préalable avant tout engagement de développement. Cette phase permet à YLC Prompt Labs de qualifier précisément le périmètre technique et fonctionnel, d'évaluer les intégrations nécessaires, et de proposer 2 à 3 variantes chiffrées permettant à [Raison sociale] d'arbitrer en connaissance de cause.

## Périmètre du cadrage

Le cadrage payant YLC couvre le périmètre suivant.

**Format**
- [3 à 5 jours ouvrés OU 5 à 7 jours ouvrés selon si standard ou étendu]
- 1 à 2 entretiens complémentaires avec les référents métier
- Cartographie détaillée du ou des processus cibles
- Analyse des outils et intégrations existants côté client

**Livrables**
- Cartographie du ou des processus cibles (inputs, étapes, acteurs, outils, points de friction)
- **2 à 3 variantes conditionnelles chiffrées** de la solution, présentées selon la grille YLC (périmètre, architecture, chiffrage setup + récurrent, délai, conditions de bascule, risques et limites)
- **Analyse de conformité AI Act** appliquée au périmètre : qualification du statut fournisseur / déployeur du client, obligations applicables, échéances à respecter (2 août 2026, 2 novembre 2026)
- **Validation de la Question 4** : évaluation du volume d'activité réel justifiant l'investissement dans la solution retenue
- **Roadmap de déploiement** avec jalons, dépendances techniques, hypothèses explicites
- Liste des comptes d'infrastructure à créer côté client (API LLM, hébergement, orchestration, plateforme agréée le cas échéant) avec estimation prévisionnelle des coûts mensuels

Le livrable est remis en format DOCX éditable et PDF.

## Chiffrage

| Prestation | Montant HT |
|---|---|
| Cadrage préalable — [description brève] | **[MONTANT] € HT** |

**Application tarifaire**

Deux fourchettes existent selon la complexité du périmètre :

*Cadrage standard (1 processus, 1 métier)*
- Territorial YLC : 1 200 à 2 000 € HT
- Référence marché européen : 1 500 à 2 500 € HT
- Durée : 3 à 5 jours ouvrés

*Cadrage étendu (multi-processus ou secteur réglementé)*
- Territorial YLC : 2 000 à 2 800 € HT
- Référence marché européen : 2 500 à 3 500 € HT
- Durée : 5 à 7 jours ouvrés

**Total HT : [MONTANT] € HT**
TVA non applicable, article 293 B du CGI

## ⚠ Clause de déductibilité — élément différenciant

**Le montant du présent cadrage est déductible à 100 % du setup de la solution retenue en phase 2 (Famille B ou Famille C), sous réserve que le devis de phase 2 soit signé dans un délai de 60 jours calendaires à compter de la remise du livrable de cadrage.**

Passé ce délai, la clause de déductibilité tombe, et le cadrage reste acquis à YLC comme livrable autonome. Cette clause est reprise dans le devis de phase 2 qui sera émis à l'issue du cadrage.

## Modalités de paiement

- **Acompte** : 100 % à la signature du présent devis
- Règlement par virement bancaire sous 15 jours calendaires à réception de facture
- Coordonnées bancaires : [RIB YLC à joindre en annexe]

## Prolongements — phase 2 possible

À l'issue du cadrage, [Raison sociale] disposera de 2 à 3 variantes chiffrées entre lesquelles arbitrer. Les fourchettes indicatives selon les familles applicables sont les suivantes (colonne territoriale si éligible, sinon référence marché).

*Famille B — Automatisations sur mesure*
- B1 Simple : 960 à 2 000 € HT territorial / 1 200 à 2 500 € HT référence
- B2 Multi-étapes IA : 2 000 à 4 000 € HT territorial / 2 500 à 5 000 € HT référence
- B3 Complexe : 4 000 à 7 200 € HT territorial / 5 000 à 9 000 € HT référence

*Famille C — Agents autonomes PaaS*
- C1 Mono-fonction : 4 000 à 7 200 € HT territorial / 5 000 à 9 000 € HT référence
- C2 Complexe : 7 200 à 14 400 € HT territorial / 9 000 à 18 000 € HT référence
- C3 Écosystème multi-agents : 14 400 à 40 000 € HT territorial / 18 000 à 50 000 € HT référence

Le chiffrage ferme et définitif de la phase 2 est établi à l'issue du cadrage, sur la base des variantes retenues.

## Conditions particulières

- **Infrastructure sur comptes client** : dans le cadre d'un éventuel déploiement en phase 2 (Familles B2, B3 ou C), le client porte l'intégralité de ses coûts d'infrastructure sur ses propres comptes (API LLM, hébergement, plateformes d'orchestration, bases vectorielles, plateformes agréées). YLC facture exclusivement la prestation de conception, de développement et d'accompagnement. Le livrable de cadrage détaillera précisément les comptes à créer et l'estimation des coûts mensuels associés.
- **Conformité AI Act** : le cadrage inclut la qualification du statut juridique du client au sens du règlement européen sur l'intelligence artificielle (AI Act). Cette qualification est un livrable obligatoire du cadrage dès que le projet touche un système à haut risque au sens de la réglementation.
- **Confidentialité** : YLC s'engage à respecter la confidentialité de toute information communiquée dans le cadre de la mission.
- Le présent devis est valable 30 jours à compter de sa date d'émission.

## Signatures

| Pour YLC Prompt Labs | Pour [Raison sociale client] |
|---|---|
| Youri Le Creau | [Nom du signataire] |
| Fondateur | [Fonction] |
| Date : | Date : |
| Signature (précédée de "Bon pour accord") : | Signature (précédée de "Bon pour accord") : |

---

## Instructions pour l'Agent Auditeur lors de la génération DOCX

1. Génère un fichier .docx dans `/mnt/user-data/outputs/Devis_Cadrage_[NomClient]_[YYYYMMDD].docx`
2. Applique strictement la charte YLC
3. La **clause de déductibilité 60 jours** doit être présentée dans un **callout amber** (fond FEF3C7, bordure gauche amber épaisse F59E0B) pour maximiser sa visibilité — c'est un différenciateur majeur
4. Ne mentionne jamais "décote" ou "rabais"
5. Génère aussi le PDF miroir via LibreOffice
6. Livre les deux fichiers via `present_files`
