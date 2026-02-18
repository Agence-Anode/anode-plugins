# Brief Enrichi - [Client] [Variant]

## Metadata

```yaml
client: "[slug]"
slug: "[variant]"
date: "[YYYY-MM-DD]"
consultant: "[prenom]"
framework: "PAS|AIDA|BAB|4Ps|PASTOR|QUEST"
cta_type: "form_new|call|rdv|download"
audience: "[cible principale]"
audience_secondaire: "[cible secondaire si applicable]"
```

## Branding

```yaml
couleur_primaire: "[hex]"
couleur_secondaire: "[hex]"
couleur_accent: "[hex]"
font_titres: "[font]"
font_body: "[font]"
ton: "[ex: professionnel, accessible, expert]"
logo_url: "[URL ou chemin]"
```

## Contenu LP

### 1. Positionnement

[Description claire du positionnement du client/produit sur le marche. En quoi il se differencie.]

### 2. Enjeux Adresses

[Les problemes/douleurs de la cible que la LP doit adresser. Lister 3-5 enjeux concrets.]

### 3. Solution / Proposition de Valeur

[Comment le produit/service repond aux enjeux. Proposition de valeur claire et differenciante.]

### 4. Features Cles

| Feature | Benefice |
|---------|----------|
| [Feature 1] | [Benefice associe] |
| [Feature 2] | [Benefice associe] |
| [Feature 3] | [Benefice associe] |
| [Feature 4] | [Benefice associe] |
| [Feature 5] | [Benefice associe] |

### 5. Avantages Competitifs

[En quoi le client se differencie de la concurrence. Points forts vs alternatives du marche.]

### 6. Cas Client / Social Proof

[Au moins 1 cas client concret avec resultats chiffres, ou temoignage, ou logos clients, ou chiffres cles.]

### 7. Messages Cles

- **Headline** : [Titre principal de la LP]
- **Sous-titre** : [Sous-titre explicatif]
- **Texte CTA** : [Texte du bouton principal]

### 8. FAQ

| Question | Reponse |
|----------|---------|
| [Question 1] | [Reponse] |
| [Question 2] | [Reponse] |
| [Question 3] | [Reponse] |

## Contexte Campagne

```yaml
objectif_campagne: "[ex: generation leads, demo, telechargement]"
mots_cles_adwords: "[liste des mots-cles cibles]"
angle_pub: "[angle principal des annonces]"
pages_concurrentes: "[URLs de reference si disponibles]"
```

## Rappels Standards Integrateurs

- Script UTM session storage dans `<head>`
- `base: './'` dans vite.config.js
- CTAs en chemins relatifs avec `?type=`
- IDs HTML conformes (CTA_, NAV_, RES_, EXT_)
- Mobile-first responsive (375px → 768px → 1440px)
- Lighthouse >= 90
- DataLayer form_step a chaque ecran formulaire
- Standards complets : `~/Documents/airnode/specs/lftf-standards.md`
