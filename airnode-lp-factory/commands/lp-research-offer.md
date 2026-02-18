# Skill /lp-research-offer — Recherche offre & positionnement client

## Usage
```
/lp-research-offer [client] [url]
```

## Instructions

Tu analyses en profondeur l'offre et le positionnement du client pour alimenter le brief LP.

### Sources (via EXA MCP — `web_search_exa`)

Lancer des recherches EXA avec `includeDomains: ["[domaine-client]"]` pour trouver :

1. **Pages offre / produit** : fonctionnalites, benefices, cas d'usage
2. **Page about / a propos** : histoire, mission, valeurs, equipe
3. **Page pricing** : plans, modele tarifaire, freemium/premium
4. **Pages process / methodo** : comment ca marche, onboarding, accompagnement
5. **Pages ressources** : blog, guides, webinaires (pour comprendre l'expertise)

### Informations a extraire

Pour chaque source trouvee, extraire et synthetiser :

- **Proposition de valeur** : en 1-2 phrases, qu'est-ce que le client vend et pourquoi c'est different ?
- **Offre detaillee** : les produits/services, leurs noms, ce qu'ils couvrent
- **Process de vente / d'accompagnement** : les etapes (demo, essai, onboarding...)
- **Certifications et badges** : ISO, labels, reconnaissances sectorielles
- **Chiffres cles** : nombre de clients, annees d'existence, CA, croissance, volumes traites
- **Differenciateurs revendiques** : ce que le client met en avant vs la concurrence
- **Ton et vocabulaire** : comment le client parle de lui-meme (registre, termes recurrents)

### Output

Sauvegarder dans `~/Documents/[client]/assets/recherches/offre-positionnement-[date].md`

### Validation

Presenter la synthese au consultant :
- "Voici ce que j'ai compris de l'offre de [client]..."
- Lister les points cles
- Demander : "C'est juste ? Tu veux completer ou corriger quelque chose ?"
- Integrer les retours du consultant dans le fichier
