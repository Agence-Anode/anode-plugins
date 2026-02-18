# Skill /lp-research-competitors — Benchmark concurrents

## Usage
```
/lp-research-competitors [client] [secteur]
```

## Instructions

Tu analyses les LP concurrentes et le positionnement des concurrents pour identifier les angles differenciants.

### Etape 1 — Identifier les concurrents (Perplexity MCP — `perplexity_ask`)

Demander a Perplexity :
- "Quels sont les principaux concurrents de [client] dans le secteur [secteur] ?"
- "Quelles alternatives a [client] existent sur le marche francais ?"

### Etape 2 — Analyser les LP concurrentes (EXA MCP — `web_search_exa`)

Pour les 2-3 principaux concurrents, rechercher leurs landing pages :
- Query : "[concurrent] landing page OR demo OR essai gratuit"
- `includeDomains: ["[domaine-concurrent]"]`

Pour chaque LP concurrente, analyser :
- **Headline** : quel message d'accroche ?
- **Framework copy** : PAS, AIDA, BAB, autre ?
- **Arguments cles** : quels benefices mis en avant ?
- **CTA** : quel type ? quel wording ?
- **Social proof** : quels elements de preuve ?
- **Design/ton** : premium, accessible, technique ?
- **Points forts** : ce qui fonctionne bien
- **Points faibles** : ce qui manque ou est mal fait

### Etape 3 — Synthese

Identifier :
- Les **angles deja pris** par les concurrents (a eviter ou a depasser)
- Les **angles inexploites** (opportunites pour [client])
- Les **bonnes pratiques** a reprendre
- Le **positionnement differenciateur** possible pour la LP de [client]

### Output

Sauvegarder dans `~/Documents/[client]/assets/recherches/benchmark-concurrents-[date].md`

### Validation

Presenter au consultant :
- "Voici le paysage concurrentiel : [liste concurrents]"
- "Les angles deja utilises sont : [liste]"
- "Je recommande de se positionner sur : [angle differenciateur]"
- Demander : "Tu vois d'autres concurrents a analyser ? L'angle te parle ?"
