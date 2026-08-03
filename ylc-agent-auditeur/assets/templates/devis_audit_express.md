# Template — Devis Audit Express

Instructions d'usage : ce template guide la génération d'un DOCX. Remplace les `[PLACEHOLDER]` par les données client réelles. Applique automatiquement la colonne territoriale si client Martinique/Guadeloupe TPE-PME. Suis strictement la charte YLC (`charte_ylc.md`).

---

## Métadonnées

- **Numéro devis** : YLC-[YYYY]-[XXX]
- **Date** : [JJ mois AAAA]
- **Validité** : 30 jours calendaires à compter de la date d'émission
- **Nature** : Audit Express IA

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
SIRET : [SIRET client si connu, sinon "à préciser"]

## Contexte de la mission

[Prose 3-5 lignes reprenant : origine du contact / problématique verbalisée par le client / posture de YLC comme conseil en IA / justification du niveau Audit Express au regard de la taille de la structure et de la nature du besoin.]

Exemple type :
> À l'issue de nos échanges du [date], [Raison sociale] souhaite obtenir un diagnostic initial de ses opportunités d'automatisation et d'intelligence artificielle sur son périmètre [métier concerné]. Compte tenu de la taille de la structure ([X salariés]) et du nombre de processus identifiés comme prioritaires ([1-2 processus]), YLC Prompt Labs propose la mise en œuvre d'un Audit Express, format calibré pour les TPE et PME souhaitant un premier engagement structurant avant tout déploiement.

## Périmètre de l'audit

L'Audit Express YLC couvre le périmètre suivant.

**Format**
- 1 semaine calendaire de mise en œuvre
- 8 à 10 heures de travail effectif
- 2 entretiens : le dirigeant et 1 collaborateur clé
- Cartographie de 1 à 2 processus métier prioritaires

**Livrables**
- Rapport d'audit structuré de 10 à 15 pages, format PDF + DOCX éditable
- Identification de 3 à 5 quick wins avec estimation d'impact
- Recommandations classées selon la taxonomie YLC (Famille A / B / C)
- Roadmap opérationnelle à horizon 3 à 6 mois
- Restitution orale de 45 minutes (visioconférence ou présentiel selon localisation)

**Hors périmètre**
- Développement d'agents, d'automatisations ou d'intégrations techniques
- Formation approfondie des équipes
- Accompagnement au déploiement (fait l'objet d'une phase 2 séparée le cas échéant)

## Chiffrage

| Prestation | Montant HT |
|---|---|
| Audit Express IA — [Raison sociale] | **[MONTANT] € HT** |

**Application tarifaire**
- Si client Martinique/Guadeloupe TPE-PME (<50 salariés) : appliquer fourchette territoriale **1 200 à 2 000 € HT**
- Sinon : appliquer fourchette référence marché européen **1 500 à 2 500 € HT**
- Placer le montant dans la fourchette selon la complexité observée (voir `grille_tarifaire.md` — règles de calibration)

**Total HT : [MONTANT] € HT**
TVA non applicable, article 293 B du CGI

## Modalités de paiement

- **Acompte** : 50 % à la signature du présent devis
- **Solde** : 50 % à la remise du rapport d'audit
- Règlement par virement bancaire sous 15 jours calendaires à réception de facture
- Coordonnées bancaires : [RIB YLC à joindre en annexe]

## Prolongements possibles (mentionnés à titre indicatif)

À l'issue de l'audit, les recommandations peuvent déboucher sur :
- Une recommandation SaaS (Famille A) accompagnée d'une mise en place
- Une automatisation ciblée (Famille B) — setup 960 à 7 200 € HT selon complexité (fourchette territoriale) ou 1 200 à 9 000 € HT (référence marché)
- Un agent autonome sur mesure (Famille C) — cadrage payant préalable obligatoire (1 200 à 2 800 € HT territorial ou 1 500 à 3 500 € HT référence marché)

Les phases suivantes font systématiquement l'objet d'un devis séparé après restitution de l'audit.

## Conditions particulières

- Le présent devis est valable 30 jours à compter de sa date d'émission
- La signature du devis vaut acceptation des conditions générales de vente YLC Prompt Labs (disponibles sur demande)
- YLC s'engage à respecter la confidentialité de toute information communiquée dans le cadre de la mission
- Le client s'engage à donner accès aux collaborateurs et documents nécessaires à la bonne conduite de l'audit

## Signatures

| Pour YLC Prompt Labs | Pour [Raison sociale client] |
|---|---|
| Youri Le Creau | [Nom du signataire] |
| Fondateur | [Fonction] |
| Date : | Date : |
| Signature (précédée de "Bon pour accord") : | Signature (précédée de "Bon pour accord") : |

---

## Instructions pour l'Agent Auditeur lors de la génération DOCX

1. Génère un fichier .docx dans `/mnt/user-data/outputs/Devis_Audit_Express_[NomClient]_[YYYYMMDD].docx`
2. Applique strictement la charte YLC (navy H1 avec rule, mid-blue accent H2, tableaux navy avec alternance, callout amber si mention légale importante)
3. Ne mentionne jamais "décote" ou "rabais" — le tarif territorial est le tarif
4. Génère aussi le PDF miroir via LibreOffice
5. Livre les deux fichiers via `present_files`
