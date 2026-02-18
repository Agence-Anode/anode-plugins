# Skill /lp-branding — Extraction branding

## Usage
```
/lp-branding [client] [url]
```

## Instructions

Tu extrais le branding visuel du site client via Firecrawl MCP.

### Pre-requis

Verifier si `~/Documents/[client]/assets/branding.md` existe deja.
- **Si oui** : le lire et le montrer au consultant. Demander "Le branding est deja extrait, tu veux le mettre a jour ?"
- **Si non** : lancer l'extraction.

### Extraction

1. Scraper la page d'accueil du site client via Firecrawl (`firecrawl_scrape`)
2. Extraire :
   - **Couleurs** : primaire, secondaire, accent (codes hex)
   - **Fonts** : titres et body
   - **Ton** : professionnel, accessible, technique, humain, premium...
   - **Logo** : URL si disponible
   - **Style visuel** : photos, illustrations, icones, ambiance generale

3. Sauvegarder dans `~/Documents/[client]/assets/branding.md` au format :
```yaml
# Branding — [Client]

couleur_primaire: "#XXXXXX"
couleur_secondaire: "#XXXXXX"
couleur_accent: "#XXXXXX"
font_titres: "[font]"
font_body: "[font]"
ton: "[description du ton]"
logo_url: "[url]"

## Notes visuelles
[Observations sur le style visuel general : type de photos, illustrations, ambiance]
```

### Validation

Presenter le branding extrait au consultant :
- Montrer les couleurs avec les codes hex
- Montrer les fonts identifiees
- Decrire le ton
- Demander : "Ca correspond bien au branding actuel du client ? Des ajustements ?"

Appliquer les corrections du consultant puis sauvegarder la version finale.
