# Skill /lp — Orchestrateur LP Factory v2

## Usage
```
/lp [client] [url] — [objectif]
```

Exemples :
```
/lp sindup https://sindup.com — capture leads demo
/lp adrec https://adrec.fr — demande devis fleet management
```

## Instructions

Tu orchestres le workflow complet de creation de brief LP, etape par etape, avec validation du consultant a chaque phase.

**REGLE ABSOLUE** : ne jamais passer a la phase suivante sans validation explicite du consultant.

### Phase 0 — Init (`/lp-init`)

1. Parser les arguments (client, url, objectif)
2. Check repo GitHub `Agence-Anode/[client]`
3. Check dossier local `~/Documents/[client]/`
4. Si nouveau client → creer la structure
5. Collecter les infos manquantes (cible, mots-cles, CTA type)
6. **VALIDATION** : presenter le recap, attendre confirmation

### Phase 1 — Branding (`/lp-branding`)

1. Verifier si `assets/branding.md` existe
2. Si non → scraper via Firecrawl MCP
3. **VALIDATION** : presenter le branding, attendre confirmation

### Phase 2A — Offre client (`/lp-research-offer`)

1. Recherche EXA sur le domaine client (offre, about, pricing, process)
2. Synthese : proposition de valeur, features, chiffres, differenciateurs
3. **VALIDATION** : presenter la synthese, attendre confirmation/complements

### Phase 2B/2C/2D — En parallele (apres validation 2A)

Lancer simultanement :
- **2B** (`/lp-research-proof`) : temoignages, avis, social proof
- **2C** (`/lp-research-competitors`) : benchmark LP concurrentes
- **2D** (`/lp-research-market`) : contexte marche, pain points audience

**VALIDATION** : presenter chaque bloc de resultats, attendre confirmation sur chacun

### Phase 3 — Strategie copy (`/lp-strategy`)

1. Synthetiser toutes les recherches
2. Proposer 2-3 options de framework + angle + hero section complete
3. Chaque option = ~15 lignes de description du flow + wording hero complet
4. **VALIDATION** : le consultant choisit son option (ou mixe)

### Phase 4 — Brief enrichi (`/lp-brief`)

1. Rediger le brief complet selon le template
2. Toutes les sections remplies avec contenu reel
3. **VALIDATION** : relecture consultant, ajustements

### Phase 5 — Wireframe HTML (`/lp-wireframe`)

1. Generer le wireframe HTML a partir du brief
2. Utiliser le template `~/Documents/airnode/templates/wireframe.html`
3. Remplacer les placeholders par le contenu reel
4. Sauvegarder dans `~/Documents/[client]/briefs/wireframe-[slug].html`
5. **VALIDATION** : consultant ouvre dans le navigateur, confirme la structure

### Phase 6 — Handoff (`/lp-handoff`)

1. Demander confirmation explicite au consultant
2. Git push
3. Slack #lftf-airnode
4. Ticket ClickUp
5. Resume final

## Regles MCPs

- **EXA** : recherche contenu (pages client, temoignages, concurrents)
- **Firecrawl** : branding uniquement (scrape HTML/CSS)
- **Perplexity** : syntheses et analyses (marche, audience, tendances)
- **Slack** : handoff uniquement, apres confirmation
- **ClickUp** : ticket integrateur uniquement, apres confirmation
- **Netlify** : pas dans ce workflow (c'est le deploiement, pas le brief)

## En cas de lancement partiel

Le consultant peut aussi lancer chaque skill independamment :
- `/lp-init`, `/lp-branding`, `/lp-research-offer`, `/lp-research-proof`
- `/lp-research-competitors`, `/lp-research-market`, `/lp-strategy`
- `/lp-brief`, `/lp-wireframe`, `/lp-handoff`

Chaque skill est autonome et peut etre utilise seul sur un client existant.
