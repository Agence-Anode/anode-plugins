# Skill /lp-handoff — Handoff integrateurs

## Usage
```
/lp-handoff [client]
```

## Pre-requis

Le brief et le wireframe doivent etre valides par le consultant.

## Instructions

Tu geres le handoff vers les integrateurs : Git push + Slack + ClickUp.

### Etape 1 — Confirmation

Demander au consultant : "Le brief et le wireframe sont prets. Je lance le handoff ? (Git push + Slack + ClickUp)"

**Attendre la confirmation explicite.**

### Etape 2 — Git push

```bash
cd ~/Documents/[client]
git add briefs/ assets/
git commit -m "brief: [client] [slug] - [description courte]"
git push origin main
```

### Etape 3 — Notification Slack (MCP Slack)

Envoyer sur `#lftf-airnode` :
```
Nouveau brief LP pret

Client : [client]
Variant : [slug]
Objectif : [objectif]
Audience : [cible]
Framework : [framework]
CTA type : [cta_type]
Brief : https://github.com/Agence-Anode/[client]/blob/main/briefs/declinaisons/[slug].md
Consultant : [prenom]
```

### Etape 4 — Ticket ClickUp (MCP ClickUp)

Creer un ticket :
- **Titre** : `[client] · 1 LP — [sujet court]`
- **Assignee** : Antoine Derouin (user ID : `100696038`)
- **Status** : `READY TO`
- **Start date** : date du jour
- **Due date** : J+2 ouvres
- **Tags** : `airnode`, `lp`, `[client]`
- **Description** : lien brief GitHub, audience, objectif, framework, CTA, headline, consultant, repo

### Etape 5 — Resume

Confirmer au consultant :
- Git push : OK/KO
- Slack : OK/KO
- ClickUp : OK/KO + lien ticket
- Lien brief GitHub
