# Skill /lp-wireframe — Generation wireframe HTML

## Usage
```
/lp-wireframe [client]
```

## Pre-requis

Le brief enrichi doit etre termine. Lire :
- `~/Documents/[client]/briefs/declinaisons/[slug].md` (brief enrichi)
- `~/Documents/[client]/assets/branding.md`

## Instructions

Tu generes un wireframe HTML noir et blanc a partir du brief enrichi, en utilisant le template wireframe.

### Etape 1 — Lire le template

Lire le fichier `~/Documents/airnode/templates/wireframe.html`

### Etape 2 — Remplacer les placeholders

Creer une copie du template dans `~/Documents/[client]/briefs/wireframe-[slug].html`

Remplacer tous les `{{PLACEHOLDER}}` par le contenu reel du brief :

| Placeholder | Source dans le brief |
|-------------|---------------------|
| `{{CLIENT}}` | Metadata → client |
| `{{DATE}}` | Date du jour |
| `{{FRAMEWORK}}` | Metadata → framework |
| `{{CTA_TYPE}}` | Metadata → cta_type |
| `{{CTA_TEXT}}` | Messages Cles → Texte CTA |
| `{{HERO_EYEBROW}}` | Strategie → eyebrow |
| `{{HERO_HEADLINE}}` | Messages Cles → Headline |
| `{{HERO_SUBHEADLINE}}` | Messages Cles → Sous-titre |
| `{{LOGO_CLOUD_TITLE}}` | "Ils nous font confiance" ou equivalent |
| `{{FEATURES_*}}` | Features Cles (titre, desc pour chaque) |
| `{{STATS_*}}` | Chiffres cles extraits des recherches |
| `{{TESTIMONIAL_*}}` | Cas Client / Social Proof |
| `{{CTA_MID_*}}` | Reprendre le message CTA avec variante |
| `{{FAQ_*}}` | FAQ du brief |
| `{{CTA_FINAL_*}}` | CTA de cloture |
| `{{CTA_REASSURANCE}}` | Phrase de reassurance (ex: "Sans engagement") |
| `{{YEAR}}` | Annee en cours |

### Etape 3 — Adapter la structure

Le template est une base. Selon le brief, tu peux :
- **Ajouter des sections** : si le brief contient plus de features, plus de temoignages, des pricing...
- **Supprimer des sections** : si le brief ne contient pas de FAQ ou de stats
- **Reordonner** : selon le framework copy choisi (ex: BAB met les benefices avant les features)

Consulter `~/Documents/airnode/specs/tailwind-plus/INDEX.md` pour les regles de composition (alternance backgrounds, coherence layout).

### Etape 4 — Validation

Informer le consultant :
- "Le wireframe est genere : `~/Documents/[client]/briefs/wireframe-[slug].html`"
- "Tu peux l'ouvrir dans ton navigateur avec `open ~/Documents/[client]/briefs/wireframe-[slug].html`"
- Demander : "La structure te convient ? Des sections a reordonner ou modifier ?"
