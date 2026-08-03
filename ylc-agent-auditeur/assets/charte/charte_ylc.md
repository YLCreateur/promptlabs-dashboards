# Charte graphique YLC — documents commerciaux

Utilise cette charte pour tout document DOCX/PDF produit pour un client YLC ou pour un usage interne YLC. Deux variantes existent : **INTERNE** (documents doctrinaux, briefs stratégiques, rapports non-client) et **CLIENT** (devis, propositions commerciales, rapports d'audit remis au client).

## Palette de couleurs (hex)

| Élément | Hex | Usage |
|---|---|---|
| Navy YLC | `1E2A4A` | Titres H1/H2/H3, en-têtes de tableau, texte fort |
| Mid-blue YLC | `3B82C4` | Barres accent H2, séparateurs, header rule |
| Amber accent | `F59E0B` | Bordure des callouts |
| Amber background | `FEF3C7` | Fond des callouts |
| Row alt | `E8EDF5` | Ligne alternée des tableaux |
| Table header text | `FFFFFF` | Texte sur navy |
| Body text | `111827` | Corps de texte |
| Muted grey | `6B7280` | Légendes, notes de bas de page |
| Rule grey | `D1D5DB` | Séparateurs subtils |

## Typographie

- **Police** : Calibri (fallback Arial)
- **Corps** : 11pt (22 half-points)
- **H1** : 16pt bold navy, avec bordure basse navy 18/8pt d'épaisseur
- **H2** : 13pt bold navy, avec bordure gauche mid-blue 18/8pt (accent bar)
- **H3** : 11pt bold navy
- **Notes** : 10pt muted grey italique
- **Header** : 9pt, "YLC Prompt Labs — [titre du document]" aligné à droite avec bordure basse mid-blue
- **Footer** :
  - INTERNE : "Document interne — Confidentiel — Ne pas diffuser hors YLC Prompt Labs" + numérotation page
  - CLIENT : "YLC Prompt Labs · Youri Le Creau · Martinique · SIRET [à remplir] · TVA non applicable, art. 293 B du CGI" + numérotation page

## Structure des tableaux

- Bordures externes : navy 4pt épaisseur
- Bordures internes : rule grey 2pt
- Ligne d'en-tête : fond navy, texte blanc bold 10pt
- Lignes alternées : fond `E8EDF5` (impaires)
- Marges cellules : 100/100/120/120 dxa
- Alignement vertical : centré
- Première colonne : bold

## Callouts (encadrés amber)

- Fond : `FEF3C7`
- Bordure gauche : amber 32pt (accent principal)
- Bordures autres : amber 8pt
- Marges internes : 200 dxa
- Titre bold navy 11pt
- Corps 10.5pt navy body

## Structure des devis client

### En-tête (première page)

1. Logo YLC en haut à gauche (si dispo, sinon "YLC PROMPT LABS" en mid-blue 10pt)
2. Titre principal navy 26pt : "Devis n° [YLC-YYYY-XXX]"
3. Sous-titre italique muted 12pt : "[Nature de la prestation]"
4. Bloc client (droite) : nom entité / contact signataire / adresse / SIRET
5. Bloc émetteur (gauche) : YLC Prompt Labs / Youri Le Creau / Martinique / contact

### Corps

1. Contexte de la mission (courte prose)
2. Périmètre détaillé (bullets ou tableau)
3. Livrables listés
4. Chiffrage (tableau détaillé HT)
5. Total HT en grand (bandeau navy)
6. Mentions TVA : "TVA non applicable, article 293 B du CGI"
7. Modalités de paiement
8. Conditions particulières (60 jours déductibilité pour cadrage, infra client pour B/C, AI Act pour C)
9. Validité de l'offre (30 jours par défaut)
10. Zone de signatures (client + YLC)

### Pied de page

- YLC Prompt Labs · Youri Le Creau · Martinique
- SIRET [à remplir par Youri]
- TVA non applicable, art. 293 B du CGI
- Numéro de page

## Marges de page

- Haut : 1200 dxa (~2 cm)
- Bas : 1440 dxa (~2.5 cm pour le footer)
- Gauche/droite : 1200 dxa

## Règles éditoriales

- Aucun mot "décote", "rabais", "remise" dans un document client
- Toujours mentionner "franchise en base TVA" pour légitimité fiscale
- Fourchettes larges dans propositions, précises dans devis fermés
- Ligne "infrastructure sur comptes client" mentionnée dans tout devis B2/B3/C
- Ligne "conformité AI Act" mentionnée dans tout devis Famille C
- Clause de déductibilité 60 jours dans tout devis de cadrage
