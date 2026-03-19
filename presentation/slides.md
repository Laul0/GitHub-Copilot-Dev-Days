---
theme: default
title: GitHub Copilot Dev Days · Montréal · 19 mars 2026
highlighter: prism
lineNumbers: false
drawings:
  persist: false
colorSchema: dark
transition: none
paginate: true
layout: image-right
image: /assets/github-copilot-dev-days.png
backgroundSize: contain
class: cover-slide
fonts:
  sans: Inter
  mono: Cascadia Code
---

# <span class="maple-leaf">🍁</span> GitHub Copilot Dev Days | Montréal

## 19 mars 2026

9h00 – 12h00 · Session entièrement en **français**

---

# 📋 Programme de la matinée

| Heure | Session |
|-------|---------|
| 9h00  | Accueil & café ☕ |
| 9h15  | **Session 1** — Vue d'ensemble : Copilot pour tous les rôles |
| 9h45  | **Workshop 1** — GitHub Copilot CLI : le terminal augmenté |
| 10h15 | Pause ☕ |
| 10h25 | **Session 3** — GitHub Copilot dans VS Code |
| 10h55 | **Session 4** — Coding Agent : déléguer à votre IA |
| 11h15 | **Workshop 2** — Workflows Agentiques |
| 11h35 | 🎙️ Table ronde — L'IA selon votre rôle |
| 11h50 | Conclusion, ressources & prochaines étapes |

> **Prérequis** : Compte GitHub + Copilot activé → `aka.ms/get-github-copilot-devdays`

---
clicks: 6
---

<!-- Slide 3 — animation: each Next highlights the next card blue -->

# 🎯 Qui êtes-vous ?

*Levez la main quand votre rôle apparaît — les exemples de ce matin sont pour vous.*

<div class="cards">
  <div :class="['card', $clicks >= 1 && $clicks < 2 ? 'blue' : '']">👩‍💻 <strong>Développeur·euse</strong><small>Code, tests, refactoring</small></div>
  <div :class="['card', $clicks >= 2 && $clicks < 3 ? 'blue' : '']">🏗️ <strong>Architecte</strong><small>Design, revue, docs</small></div>
  <div :class="['card', $clicks >= 3 && $clicks < 4 ? 'blue' : '']">📋 <strong>Chef de projet</strong><small>Stories, impact, specs</small></div>
  <div :class="['card', $clicks >= 4 && $clicks < 5 ? 'blue' : '']">⚙️ <strong>DevOps / SRE</strong><small>Pipelines, scripts, logs</small></div>
  <div :class="['card', $clicks >= 5 && $clicks < 6 ? 'blue' : '']">🎓 <strong>Étudiant·e</strong><small>Apprentissage accéléré</small></div>
  <div :class="['card', $clicks >= 6 ? 'blue' : '']">🔍 <strong>Curieux·euse</strong><small>Explorer sans contrainte</small></div>
</div>

---
clicks: 8
---

# 🎲 Bingo des Devs

*Cochez si c'est votre cas. Qui fera un bingo d'ici 12h ?* 🏆

<div class="bingo">
  <div :class="['cell', $clicks >= 1 && $clicks < 2 ? 'hl' : '']">✅ VS Code<br/>au quotidien</div>
  <div :class="['cell', $clicks >= 2 && $clicks < 3 ? 'hl' : '']">😅 10+ onglets<br/>ouverts maintenant</div>
  <div :class="['cell', $clicks >= 3 && $clicks < 4 ? 'hl' : '']">😰 Peur que l'IA<br/>me remplace</div>
  <div :class="['cell', $clicks >= 4 && $clicks < 5 ? 'hl' : '']">🤖 Utilisé Copilot<br/>en production</div>
  <div class="cell center"><span class="maple-leaf">🍁</span><br/>MONTRÉAL<br/>LIBRE</div>
  <div :class="['cell', $clicks >= 5 && $clicks < 6 ? 'hl' : '']">📦 Un side project<br/>jamais terminé</div>
  <div :class="['cell', $clicks >= 6 && $clicks < 7 ? 'hl' : '']">🌙 Codé à<br/>2h du matin</div>
  <div :class="['cell', $clicks >= 7 && $clicks < 8 ? 'hl' : '']">🐛 Débogué 2h+<br/>un truc trivial</div>
  <div :class="['cell', $clicks >= 8 ? 'hl' : '']">🚀 Déployé un<br/>vendredi soir</div>
</div>

---
layout: default
class: section-break
---

# Session 1

## Vue d'ensemble

*GitHub Copilot : votre coéquipier IA, pour tous les rôles*

---

# Pourquoi l'IA, maintenant ?

**La chronologie a été rapide :**

- **2022** — Autocomplétion temps réel (le « Tab magique »)
- **2023** — Copilot Chat : conversation dans l'IDE
- **2024** — Copilot Workspace : workflows agentiques
- **2025–2026** — Coding Agent : délégation asynchrone complète

> *"55 % des développeurs utilisant GitHub Copilot produisent du code plus rapidement."*
> — GitHub Octoverse 2024

**Ce n'est plus un gadget — c'est devenu une compétence professionnelle.**

---

# L'évolution de GitHub Copilot

<div class="cards">
  <div class="card">
    <strong>⌨️ Autocomplétion</strong>
    Vous guidez chaque ligne.
    <small>Résultat : immédiat.</small>
  </div>
  <div class="card blue">
    <strong>💬 Chat</strong>
    Vous conversez.
    <small>Résultat : interactif.</small>
  </div>
  <div class="card green">
    <strong>🤖 Agent</strong>
    Vous déléguez.
    <small>Résultat : une PR complète.</small>
  </div>
</div>

**Aujourd'hui, nous couvrons les trois.**

> *Et ce n'est pas que pour les développeurs.*

---

# Qui profite de GitHub Copilot ?

| Rôle | Cas d'usage concret |
|------|---------------------|
| 👩‍💻 **Développeur·euse** | Génération de code, tests unitaires, refactoring |
| 🏗️ **Architecte** | Analyse de code, documentation auto, revue de design |
| 📋 **Chef de projet** | Résumer des PR, rédiger des user stories, analyser l'impact |
| ⚙️ **DevOps / SRE** | Scripts shell, pipelines CI/CD, interprétation de logs |
| 🎓 **Étudiant·e** | Apprendre par l'exemple, comprendre sans mémoriser |

> *"GitHub Copilot ne remplace pas votre équipe —*
> *il lui ajoute un coéquipier qui ne dort jamais."*

---

# GitHub Copilot — L'écosystème complet

**Où est-il disponible ?**

- 💻 **VS Code** — Agent Mode, Edits, Chat, Inline
- 🖥️ **Visual Studio** — Intégration complète .NET
- ☕ **JetBrains / Eclipse** — IntelliJ, PyCharm, Rider…
- 🍎 **Xcode** — Pour les développeurs Apple
- 🖥️ **Terminal / CLI** — `gh copilot explain | suggest`
- ☁️ **GitHub.com** — Coding Agent, PR reviews, issues
- 📱 **GitHub Mobile** — Copilot Chat en déplacement

> Ce matin : **CLI + VS Code + Cloud Agent**
> → *Choisissez votre point d'entrée selon votre rôle*

---
layout: default
class: section-break
---

# Workshop 1

## GitHub Copilot CLI

*L'entrée universelle — sans IDE, depuis n'importe quel terminal*

---
layout: image-right
image: /assets/github-copilot-dev-days.png
backgroundSize: contain
class: cover-slide
---

# Workshop 1 — GitHub Copilot CLI

## GitHub Copilot Dev Days · Montréal

*Votre terminal, augmenté par l'IA*

`gh copilot explain | suggest | ask`

---

# Pourquoi commencer par le CLI ?

- **Aucun IDE requis** — macOS, Linux, WSL, SSH, tout terminal
- **Universel** — accessible quel que soit votre éditeur habituel
- **Trois commandes** couvrent 80 % des besoins du quotidien

```bash
# Installation (si pas encore fait)
gh extension install github/gh-copilot

# Les deux commandes clés
gh copilot explain   # Comprendre une commande inconnue
gh copilot suggest   # Générer depuis du langage naturel
```

> 📖 Docs : `docs.github.com/en/copilot/how-tos/copilot-cli`

---

# Les 3 super-pouvoirs du CLI

<div class="cards">
  <div class="card blue">
    <strong>🔍 explain</strong>
    Décryptez n'importe quelle commande en langage naturel.
    <small>Idéal : kubectl, awk, git, find…</small>
  </div>
  <div class="card green">
    <strong>✨ suggest</strong>
    Décrivez ce que vous voulez → la commande exacte.
    <small>En français ✓</small>
  </div>
  <div class="card orange">
    <strong>🐛 explain + erreur</strong>
    Collez un message d'erreur → explication + solution.
    <small>npm, docker, python…</small>
  </div>
</div>

**Message clé :** *"Si vous n'utilisez qu'un seul outil Copilot aujourd'hui, commencez par le CLI."*

---

# 🔍 Démo 1 — explain : commande kubectl mystère

**D'abord, à votre avis, que fait cette commande ?**

```bash
kubectl get pods --all-namespaces \
  -o=custom-columns='NAME:.metadata.name,NAMESPACE:.metadata.namespace,
    STATUS:.status.phase,RESTARTS:.status.containerStatuses[0].restartCount' \
  --field-selector=status.phase=Running \
  | awk 'NR>1 && $4>5 {print $1,$2,$3,$4}' \
  | sort -k4 -rn | head -20
```

```bash
# On lance Copilot CLI pour vérifier...
gh copilot explain "kubectl get pods --all-namespaces ..."
```

---

# 🎯 Défi collectif — suggest

**Question posée à la salle :**

> *"Comment lister tous les fichiers modifiés il y a plus de 30 jours et les archiver dans une archive tar.gz ?"*

**Vos propositions d'abord** — puis :

```bash
gh copilot suggest "list all files modified more than 30 days ago and archive them in a tar.gz"
```

*Qui était le plus proche dans la salle ?* 🏆

---

# 🐛 Démo 3 — explain : message d'erreur npm

**Scénario DevOps / étudiant·e :**

```
npm error code EACCES
npm error syscall open
npm error path /usr/local/lib/node_modules/.package-lock.json
npm error errno -13
npm error Error: EACCES: permission denied, open '...'
```

```bash
gh copilot explain "npm error code EACCES errno -13 permission denied"
```

*Copilot explique la cause ET propose la solution — en moins de 10 secondes.*

---

# 🧩 Skills & Plugins

**Étendre Copilot CLI pour des tâches répétitives spécifiques à votre équipe :**

<div class="cards cols-2">
  <div class="card blue">
    <strong>📦 Skills</strong>
    Procédures réutilisables, encapsulées et partageables.
    <br/><code>/skills add</code>
    <br/><small>Projet : <code>.copilot/skills</code></small>
    <br/><small>Global : <code>.agents/skills</code></small>
  </div>
  <div class="card green">
    <strong>🔌 Plugins</strong>
    Bundles complets : skills, agents, MCP servers, hooks.
    <br/><code>/plugin</code>
    <br/><small>Enrichissent tout le workflow CLI</small>
  </div>
</div>

> **Exemple :** Un skill `deploy-review` qui analyse les diffs, vérifie les tests, et génère un résumé de déploiement — disponible dans tous vos projets depuis le terminal.

---

# 🗂️ /context · /compact · Sessions infinies

| Commande | Ce qu'elle fait |
|----------|-----------------|
| `/context` | Visualise les tokens utilisés et les fichiers dans la fenêtre de contexte |
| `/compact` | Résume et compacte le contexte pour libérer de l'espace |

```bash
/context    # → "Your context window: 47,832 tokens used / 200,000"
/compact    # → Summarizes and reduces context
```

**Sessions infinies (exclusif CLI) :**

> *La gestion de contexte est automatique — vous n'aurez probablement jamais à vous en préoccuper. Mais pour les longues sessions de débogage ou les projets complexes, ces commandes donnent une maîtrise totale.*

---

# ⚡ Parallel Copilot

**Deux projets, deux agents, simultanément :**

<div class="cards cols-2">
  <div class="card blue">
    <strong>🖥️ Terminaux fractionnés</strong>
    Deux sessions CLI côte à côte.
    <br/><small>Terminal gauche : correction de bugs</small>
    <br/><small>Terminal droit : ajout de features</small>
  </div>
  <div class="card green">
    <strong>🤖 VS Code Agent Chat</strong>
    Agent mode VS Code en parallèle d'une tâche CLI.
    <br/><small>Délégation asynchrone totale</small>
  </div>
</div>

```bash
# Terminal gauche : projet A      # Terminal droit : projet B
gh copilot ask "Fix auth bug"  |  gh copilot ask "Add payment tests"
```

> *Vous déléguez — ils travaillent. Vous reviewez.*

---

# Le CLI par rôle

| Rôle | Exemple concret |
|------|-----------------|
| 👩‍💻 **Dev** | `explain` une commande `git rebase` avant de l'exécuter |
| 🎓 **Étudiant·e** | Apprendre les commandes sans les mémoriser |
| ⚙️ **DevOps** | `explain` un message d'erreur `kubectl` ou `docker` |
| 🏗️ **Architecte** | `suggest` des one-liners d'analyse de logs |
| 📋 **PM** | Comprendre ce que font les scripts de déploiement |

**Labs CLI disponibles :**
<span class="badge">🎮 Mona Mayhem CLI (~60 min)</span>
<span class="badge">🏗️ Tailspin Toys Workshop (~90 min)</span>

→ `copilot-dev-days.github.io`

---
layout: default
class: section-break
---

# Session 3

## GitHub Copilot dans VS Code

*Les 20 % de fonctionnalités qui donnent 80 % de la valeur*

---

# Au-delà de l'autocomplétion

**Ce que la plupart des gens connaissent :**

- ✅ Autocomplétion en ligne (Tab)
- ✅ Copilot Chat dans la barre latérale

**Ce que nous allons montrer aujourd'hui :**

| Fonctionnalité | Ce que c'est |
|---------------|--------------|
| 🔥 **Chat inline** | Instruction directement dans l'éditeur, sur la sélection |
| 🔥 **Copilot Edits** | Modifier **plusieurs fichiers** en une seule instruction |
| 🔥 **Agent Mode** | Questions et actions sur **tout le projet** (`@workspace`) |
| 🔥 **Génération de tests** | Un fichier de tests complet en un prompt |

> La qualité des réponses dépend **du contexte que vous donnez.**

---

# Référence : le contexte dans Copilot Chat

| Référence | Ce qu'elle fait |
|-----------|-----------------|
| `#file:nom.py` | Inclure un fichier spécifique dans le contexte |
| `#selection` | Utiliser le texte actuellement sélectionné |
| `#codebase` | Analyser l'ensemble du code source |
| `@workspace` | Questions et actions sur tout le projet |
| `@terminal` | Contexte du terminal actif |
| `/explain` | Expliquer le code sélectionné |
| `/tests` | Générer des tests unitaires |
| `/fix` | Proposer une correction |
| `/doc` | Générer de la documentation |

> 💡 **Astuce :** `#file:` + `@workspace` ensemble = réponses radicalement meilleures.

---

# 🎬 Démo 1 — Chat inline : analyse de sécurité

```python
# app.py (Flask — routes API sans validation)
@app.route("/login", methods=["POST"])
def login():
    data = request.json
    # ⚠️ Manque : validation des champs requis
    if authenticate(data["username"], data["password"]):
        session_token = hashlib.sha256(
            f"{data['username']}{datetime.now()}".encode()
        ).hexdigest()
        SESSIONS[session_token] = data["username"]
        return jsonify({"token": session_token})
    return jsonify({"error": "Identifiants invalides"}), 401
```

**Sélectionner la fonction → `Ctrl+I` → taper :**

> *"Explique les failles de sécurité de cette fonction et propose des corrections."*

---

# Agent Mode — La vraie puissance

**Chat classique :**
```
"Ajoute de la gestion d'erreurs à cette fonction"
→ Modifie 1 fichier, dans votre contexte immédiat
```

**Agent Mode (`@workspace`) :**
```
"Ajoute une validation d'input cohérente à toutes les routes
 POST de l'API, en suivant le style de error.py"
→ Analyse l'ensemble du projet
→ Modifie plusieurs fichiers en cohérence
→ Respecte le style existant
```

*C'est la différence entre un assistant ponctuel et un coéquipier.*

---

# 🎬 Démo 2 — @workspace : générer les tests

**L'app de démo n'a aucun test unitaire. On le demande directement :**

```
@workspace Ce projet n'a aucun test. Génère un fichier
test_app.py complet avec pytest, couvrant toutes les routes
et fonctions utilitaires. Inclure des cas de succès et
d'échec pour chaque endpoint.
```

**Ce qui se passe :**
1. Copilot analyse **tout** le projet
2. Identifie les routes, les utilitaires, les cas limites
3. Génère un fichier `test_app.py` complet
4. Vous n'avez plus qu'à reviewer et ajuster

---

# Labs VS Code disponibles

<div class="cards cols-2">
  <div class="card blue">🐍 <strong>Python Agent Lab</strong><br/>FastAPI + HTMX · Social Bingo<br/><small>~1h · 4 parties · 9 étapes</small><br/><small><code>agent-lab-python</code></small></div>
  <div class="card green">🟦 <strong>TypeScript Agent Lab</strong><br/>Vite + React · Social Bingo<br/><small>~1h · 4 parties · 9 étapes</small><br/><small><code>agent-lab-typescript</code></small></div>
  <div class="card yellow">☕ <strong>Java Agent Lab</strong><br/>Spring Boot · Social Bingo<br/><small>~1h · 4 parties · 9 étapes</small><br/><small><code>agent-lab-java</code></small></div>
  <div class="card red">🟣 <strong>.NET Agent Lab</strong><br/>Blazor · Social Bingo<br/><small>~1h · 4 parties · 9 étapes</small><br/><small><code>agent-lab-dotnet</code></small></div>
</div>

→ Tous les labs : **`copilot-dev-days.github.io`**

---
layout: default
class: section-break
---

# Session 4

## GitHub Copilot Coding Agent

*Déléguer, pas juste assister*

---

# Autocomplétion → Chat → Agent

<div class="cards">
  <div class="card" style="opacity:0.75">
    <strong>⌨️ Autocomplétion</strong>
    Vous guidez chaque ligne.
    <small>Résultat : immédiat.<br/>Portée : une ligne.</small>
  </div>
  <div class="card blue">
    <strong>💬 Chat</strong>
    Vous conversez.
    <small>Résultat : interactif.<br/>Portée : un fichier.</small>
  </div>
  <div class="card green" style="border-width:2px">
    <strong>🤖 Coding Agent</strong>
    Vous déléguez.
    <small>Résultat : une PR complète.<br/>Portée : le repo entier.</small>
  </div>
</div>

> **L'agent lit le code, planifie, implémente, crée une PR et attend votre review.**
> *Pendant ce temps, vous faites autre chose.*

---

# Comment ça fonctionne ?

```
1. Vous ouvrez ou créez une Issue GitHub bien décrite
                    ↓
2. Vous l'assignez à "Copilot" (un seul clic)
                    ↓
3. Copilot analyse le repo en profondeur
                    ↓
4. Copilot crée une branche, écrit le code, ouvre une PR
                    ↓
5. Vous reviewez, commentez, mergez (ou renvoyez en révision)
```

*C'est du développement **asynchrone**.*

---

# Qui en bénéficie vraiment ?

| Rôle | Ce que l'agent peut faire |
|------|--------------------------|
| 👩‍💻 **Développeur·euse** | Corriger un bug documenté dans une issue existante |
| 📋 **Chef de projet** | Faire implémenter une user story bien rédigée |
| 🏗️ **Architecte** | Générer le scaffolding depuis une spec technique |
| 🎓 **Étudiant·e** | Voir comment une feature complète est implémentée |

> *"Si vous pouviez déléguer une tâche répétitive à un agent IA*
> *dès demain matin, laquelle serait-ce ?"*

---

# ⭐ Défi live — Votre issue en direct

**Le plan :**

1. **Vous proposez** une user story simple (en français)
2. **Ensemble**, on la rédige comme issue GitHub bien structurée
3. **On l'assigne à Copilot** — un seul clic
4. Copilot se met au travail...

> ⏱️ **On revient sur la PR générée à 11h45 !**

**Exemple :**
```
En tant qu'utilisateur, je veux pouvoir réinitialiser mon
mot de passe via un email, afin de retrouver l'accès à mon
compte si je l'ai oublié.
```

*Lab : `github.com/skills/expand-your-team-with-copilot`*

---
layout: default
class: section-break
---

# Workshop 2

## Workflows Agentiques

*L'orchestration, pas la magie — construire avec des agents*

---

# 🧠 Un agent : ce n'est pas de la magie

**Un système agentique = 4 éléments coordonnés :**

<div class="cards">
  <div class="card blue">
    <strong>🎯 Objectif</strong>
    "Préparer un rapport"<br/>"Générer un plan de test"<br/>"Réviser une PR"
  </div>
  <div class="card green">
    <strong>🧰 Compétences</strong>
    Tools, API, actions<br/>Terminal, tests, GitHub<br/>Fichiers, documentation
  </div>
  <div class="card orange">
    <strong>🧠 Moteur</strong>
    LLM + règles + contexte<br/>Décision à chaque étape
  </div>
  <div class="card yellow">
    <strong>🌍 Environnement</strong>
    IDE · GitHub · Pipelines<br/>Données internes · API
  </div>
</div>

> 💡 **L'image simple :** Un agent = un développeur junior super rapide **+** un chef d'orchestre qui le guide.
>
> *Ce n'est pas un robot autonome — c'est un système orchestré.*

---

# 🔧 L'agent dans votre workflow quotidien

<div class="cards">
  <div class="card blue">
    <strong>💻 Dans l'IDE</strong>
    Génère, corrige, teste, documente, prépare le PR
    <small>VS Code Agent Mode → /new-feature</small>
  </div>
  <div class="card green">
    <strong>🔄 DevOps</strong>
    Analyse les PR · Génère les pipelines · Surveille les vulnérabilités · Rédige les changelogs
  </div>
  <div class="card yellow">
    <strong>📚 Documentation</strong>
    Lit le repo · Génère la doc · Répond aux questions · Crée les guides d'onboarding
  </div>
  <div class="card orange">
    <strong>📋 Gestion de projet</strong>
    Transforme les discussions en user stories · Découpe · Priorise · Sync Jira / Issues
  </div>
</div>

> **Message clé :** *L'IA agentique n'est pas un outil supplémentaire. C'est une couche transversale qui fluidifie tout le cycle de développement.*

---

# 🏗️ Architecture d'un système agentique

| Couche | Composants |
|--------|-----------|
| **1. Interface** | Chat · IDE · GitHub · API |
| **2. Orchestrateur** | LLM · Règles · Mémoire · Contexte |
| **3. Compétences (tools)** | GitHub API · CLI · Terminal · Tests · Bases de données · API internes |
| **4. Garde-fous** | Permissions · Sandboxing · Observabilité · Logs · Limites d'action |

> ⚠️ **La couche #3 est la plus critique :**
> *Un agent n'est utile que s'il a accès aux bons outils.*
>
> *Un agent bien outillé + bien gardé = un agent de confiance.*

---

# ⚠️ Les 4 pièges à éviter

<div class="cards cols-2">
  <div class="card red">
    <strong>❌ Pas de garde-fous</strong>
    Ne jamais autoriser : merger sans validation humaine · déployer sans supervision · modifier des secrets · supprimer des ressources
  </div>
  <div class="card orange">
    <strong>❌ Trop de liberté</strong>
    Un agent doit être : borné · supervisé · traçable · explicable
  </div>
  <div class="card yellow">
    <strong>❌ Croire qu'il comprend tout</strong>
    Il ne comprend pas : les intentions implicites · les règles non écrites · le contexte organisationnel
    <small><em>"Un agent n'a pas de culture d'entreprise."</em></small>
  </div>
  <div class="card">
    <strong>❌ Mauvais outillage</strong>
    Trop peu d'outils = agent inutile
    Trop d'outils = agent dangereux
    <small>Commencer petit, élargir graduellement</small>
  </div>
</div>

---

# 🎯 Exercice — Cartographiez votre agent

**En équipe de 2–3 personnes (10 minutes) :**

> *Choisissez une tâche récurrente dans votre équipe (debugging, docs, revue de code…)*
> *et dessinez les 4 couches de l'agent qui la prendrait en charge.*

```
Objectif   → "____________________________"
Tools      → GitHub API / CLI / ??? 
Garde-fous → Qui approuve ? Quelles limites ?
Valeur     → Combien d'heures récupérées/semaine ?
```

**Partage en grand groupe : 2 min par équipe**

> *Lab complet : `copilot-dev-days.github.io` → Agentic Workflows*

---
layout: default
class: section-break
---

# 🎙️ Table Ronde

## L'IA selon votre rôle

*3–4 volontaires · 20 minutes de conversation vraie*

---

# 🎙️ Questions de la table ronde

**Pour les volontaires :**

1. *Quel est votre rôle au quotidien, et comment l'IA s'y intègre (ou pourrait s'y intégrer) ?*

2. *Quelle démo de ce matin vous a le plus marqué·e ? Pourquoi ?*

3. *Quel est votre plus grand frein à l'adoption de ces outils dans votre équipe ?*

4. *Si vous deviez convaincre votre manager en 30 secondes, quel argument utiliseriez-vous ?*

---

**Note d'animation :** Ne pas chercher les bonnes réponses — favoriser les frictions, les scepticismes, les vraies questions. *C'est là que la conversation devient mémorable.*

---

# ⭐ Retour sur la démo — La PR de Copilot

**On revient sur l'issue créée à 10h55...**

*Ouvrir GitHub et montrer la PR générée.*

**Ce qui s'est passé pendant la table ronde :**
- Copilot a analysé le repo
- Créé une branche
- Écrit le code
- Ouvert une PR avec description complète

> *De l'issue à la PR — sans que vous ayez touché un seul fichier.*

---
layout: default
class: section-break
---

# Conclusion

## Ce qu'on retient de cette matinée

---

# Ce qu'on a appris ce matin

<div class="cards">
  <div class="card blue">
    💻 <strong>Workshop 1 — CLI</strong>
    Accessible sans IDE · explain / suggest / ask
    <small>Skills, /context, /compact, Parallel Copilot</small>
  </div>
  <div class="card green">
    🖥️ <strong>VS Code</strong>
    Bien plus que l'autocomplétion
    <small>Contexte = qualité · Agent Mode = coéquipier</small>
  </div>
  <div class="card orange">
    ☁️ <strong>Coding Agent</strong>
    Délégation asynchrone · De l'issue à la PR
    <small>Pour devs, PMs et architectes</small>
  </div>
  <div class="card yellow">
    🤖 <strong>Workshop 2 — Agentique</strong>
    Orchestration, outils, garde-fous
    <small>Pas de la magie — un système structuré</small>
  </div>
  <div class="card">
    🎯 <strong>Multi-rôles</strong>
    Pas que pour les développeurs
    <small>Différentes entrées, même valeur</small>
  </div>
</div>

---

# 🔗 Ressources à emporter

| Lien | Description |
|------|-------------|
| `copilot-dev-days.github.io` | **12 workshops** · 6 langages · 6 IDEs |
| `aka.ms/get-github-copilot-devdays` | Activer GitHub Copilot **Free** |
| `docs.github.com/en/copilot/how-tos/copilot-cli` | Documentation CLI complète |
| `github.com/skills/getting-started-with-github-copilot` | Lab GitHub Skills — débutant (gratuit) |
| `github.com/skills/expand-your-team-with-copilot` | Lab GitHub Skills — Coding Agent |
| `aka.ms/githubcopilotdevdays/discussion` | Forum de la communauté Dev Days |

---

# 🎯 Votre première action cette semaine

*Pas 5 actions. **Une seule.** Dès demain matin.*

| Rôle | Action recommandée |
|------|--------------------|
| 👩‍💻 Dev | `gh copilot explain` sur la prochaine commande inconnue |
| 🏗️ Architecte | Ouvrir un projet existant et tester `@workspace` |
| 📋 PM | Rédiger une user story et l'assigner à Copilot |
| ⚙️ DevOps | `gh copilot explain` sur le prochain message d'erreur |
| 🎓 Étudiant·e | Lab GitHub Skills "Get Started" (gratuit, 30 min) |

> *"Le meilleur moment pour commencer, c'était hier.*
> *Le deuxième meilleur, c'est demain matin."*

---
layout: image-right
image: /assets/gh-copilot-devdays-sweepstqke-qr.png
backgroundSize: contain
class: section-break
---

# 🎁 Sweepstake GitHub Copilot Pro+

## `aka.ms/githubcopilotdevdays/sweepstakes`

*Tous les participants ayant complété le sondage sont éligibles.*

**Prix : abonnement GitHub Copilot Pro+ — 1 an** 🏆

---
layout: image-right
image: /assets/github-copilot-dev-days.png
backgroundSize: contain
class: end-slide
---

# <span class="maple-leaf">🍁</span> Merci Montréal !

## `github.com/github/GitHub-Copilot-Dev-Days`

Organisé par la communauté **GUM365**
dans le cadre de la série mondiale **GitHub Copilot Dev Days 2026**

📸 Photo de groupe → `#GitHubCopilotDevDays`
🔗 `meetup.com/gum365`
