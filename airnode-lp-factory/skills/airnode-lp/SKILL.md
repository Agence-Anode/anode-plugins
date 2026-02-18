---
name: airnode-lp
description: Workflow complet de creation de brief LP enrichi. Utiliser quand un consultant veut creer une landing page pour un client.
---

# Airnode LP Factory v2

Workflow structure de creation de brief LP, etape par etape, avec validation du consultant a chaque phase.

## Quand utiliser ce skill

- Le consultant mentionne une landing page, LP, ou brief
- Le consultant donne un nom de client et une URL
- Le consultant dit "je veux creer une LP pour..."

## Workflow

Executer les phases dans l'ordre. **Ne jamais passer a la phase suivante sans validation du consultant.**

1. **Init** : check repo GitHub, structure, collecte infos → `resources/lp-init.md` via `/airnode-lp:lp-init`
2. **Branding** : extraction via Firecrawl → `/airnode-lp:lp-branding`
3. **Recherche offre** : scrape pages client via EXA → `/airnode-lp:lp-research-offer`
4. **Recherche social proof** : avis, temoignages via EXA → `/airnode-lp:lp-research-proof`
5. **Recherche concurrents** : benchmark via EXA + Perplexity → `/airnode-lp:lp-research-competitors`
6. **Recherche marche** : tendances, pain points via Perplexity → `/airnode-lp:lp-research-market`
7. **Strategie copy** : 2-3 options framework + hero section → `/airnode-lp:lp-strategy`
8. **Brief enrichi** : redaction complete → `/airnode-lp:lp-brief`
9. **Wireframe HTML** : fichier ouvrable dans le navigateur → `/airnode-lp:lp-wireframe`
10. **Handoff** : git push + Slack + ClickUp → `/airnode-lp:lp-handoff`

## MCPs utilises

| MCP | Usage |
|-----|-------|
| **EXA** | Recherche contenu : pages client, temoignages, concurrents |
| **Firecrawl** | Branding uniquement (scrape HTML/CSS pour couleurs, fonts) |
| **Perplexity** | Syntheses et analyses : marche, audience, tendances |
| **GitHub** | Check/creation repos, push |
| **Slack** | Handoff sur #lftf-airnode (apres confirmation) |
| **ClickUp** | Ticket integrateur (apres confirmation) |

## Regles

1. Ne jamais passer a la phase suivante sans validation du consultant
2. Ne jamais re-scrapper ce qui existe deja
3. Slack et ClickUp : jamais d'envoi automatique, toujours demander confirmation
4. Sauvegarder les recherches dans `~/Documents/[client]/assets/recherches/`
5. Brief dans `~/Documents/[client]/briefs/declinaisons/[slug].md`
6. Wireframe dans `~/Documents/[client]/briefs/wireframe-[slug].html`
