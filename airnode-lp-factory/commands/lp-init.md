# Skill /lp-init — Initialisation client

## Usage
```
/lp-init [client] [url]
```

## Instructions

Tu initialises le workspace pour un nouveau brief LP.

### Etape 1 — Collecter les infos

Si `[client]` ou `[url]` ne sont pas fournis, demander au consultant :
- "Quel est le slug client ?" (minuscules, ex: `sindup`)
- "Quelle est l'URL du site client ?"
- "Quel est l'objectif de la LP ?" (capture leads, demo, devis, telechargement...)
- "Quelle est la cible principale ?" (DRH, DSI, dirigeant PME...)
- "Quels mots-cles AdWords sont cibles ?" (optionnel)
- "Quel type de CTA ?" (formulaire, appel, prise de RDV, telechargement)

### Etape 2 — Check GitHub

Verifier si le repo `Agence-Anode/[client]` existe via `gh repo view Agence-Anode/[client]` (bash).

**Si le repo existe** :
1. S'assurer que `~/Documents/[client]/` est a jour
2. Lister les fichiers existants : `assets/branding.md`, `assets/recherches/`, `briefs/declinaisons/`
3. Resumer au consultant ce qui existe deja
4. Demander : "Tu veux une nouvelle declinaison ou on reprend un brief existant ?"

**Si le repo n'existe pas** :
1. Creer la structure locale :
```bash
mkdir -p ~/Documents/[client]/assets/recherches ~/Documents/[client]/briefs/declinaisons ~/Documents/[client]/.claude
```
2. Creer le `CLAUDE.md` client minimal (pointe vers `~/Documents/airnode/CLAUDE.md`)
3. Creer `assets/config-client.md` avec les infos collectees
4. Informer le consultant : "Workspace cree, on peut passer a l'extraction branding."

### Etape 3 — Resume

Afficher un recap clair :
```
Client : [client]
URL : [url]
Objectif : [objectif]
Cible : [audience]
CTA type : [cta_type]
Mots-cles : [mots-cles]
Branding : [existe/a extraire]
Briefs existants : [liste ou "aucun"]
```

Demander confirmation au consultant avant de passer a la suite.
