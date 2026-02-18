# Skill /lp-research-proof — Recherche social proof & temoignages

## Usage
```
/lp-research-proof [client]
```

## Instructions

Tu recherches toutes les preuves sociales disponibles sur le client pour enrichir le brief LP.

### Sources a explorer (via EXA MCP — `web_search_exa`)

1. **Temoignages sur le site client** : `includeDomains: ["[domaine]"]`, query: "temoignage OR avis OR client OR case study"
2. **Google Avis** : query: "[client] avis"
3. **Trustpilot** : `includeDomains: ["trustpilot.com"]`, query: "[client]"
4. **G2** : `includeDomains: ["g2.com"]`, query: "[client]"
5. **Capterra** : `includeDomains: ["capterra.fr", "capterra.com"]`, query: "[client]"
6. **Articles presse / mentions** : query: "[client] [secteur] avis OR review OR test"

### Informations a extraire

Pour chaque source :
- **Verbatims** : les meilleures citations clients (mot pour mot)
- **Notes** : score moyen sur chaque plateforme (ex: 4.7/5 sur G2, 87 avis)
- **Themes recurrents** : quels aspects sont les plus apprecies ? (support, facilite, ROI...)
- **Logos clients** : noms des entreprises clientes mentionnees
- **Cas clients chiffres** : resultats concrets (ex: "+30% de productivite", "ROI en 3 mois")
- **Secteurs clients** : dans quels secteurs sont les clients satisfaits

### Output

Sauvegarder dans `~/Documents/[client]/assets/recherches/social-proof-[date].md`

Format :
```markdown
# Social Proof — [Client]

## Scores plateformes
- G2 : X/5 (N avis)
- Trustpilot : X/5 (N avis)
- Capterra : X/5 (N avis)
- Google : X/5 (N avis)

## Top verbatims (pour la LP)
1. "[Citation]" — Prenom Nom, Poste, Entreprise
2. "[Citation]" — ...

## Themes apprecies
- [Theme 1] : [explication]
- [Theme 2] : ...

## Cas clients chiffres
- [Entreprise] : [resultat]
- ...

## Logos clients identifies
[Liste]
```

### Validation

Presenter au consultant :
- "J'ai trouve X temoignages sur Y plateformes. Voici les plus percutants pour la LP :"
- Montrer les 3-5 meilleurs verbatims
- Demander : "Tu as d'autres temoignages ou cas clients a ajouter ?"
