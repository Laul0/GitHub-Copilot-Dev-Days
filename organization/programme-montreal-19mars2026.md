# 🍁 GitHub Copilot Dev Days — Montréal
### Jeudi 19 mars 2026 | 9h00 – 12h00

> **Langue :** Français  
> **Format :** Sessions-only (3 heures)  
> **Lieu :** [À confirmer]  
> **Communauté :** [GUM365 Montréal](https://www.meetup.com/gum365/events/313677064/)  
> **Inscription :** [Luma](https://luma.com/githubcopilotdevdays)

---

## 🎯 Thème de la matinée

**« Bien plus qu'un outil de code — GitHub Copilot à travers tous vos workflows »**

Une autre communauté montréalaise présente déjà l'angle classique du développeur.
Notre pari : montrer que l'IA générative, et GitHub Copilot en particulier, change la donne **pour tous les rôles dans une équipe tech** — qu'on soit développeur, architecte, chef de projet, DevOps ou étudiant.

---

## 📋 Programme détaillé

| Heure | Durée | Segment | Format |
|-------|-------|---------|--------|
| 9h00 | 10 min | Accueil & café | Réseautage |
| 9h10 | 5 min | Mot de bienvenue & tour de salle | Interactif |
| 9h15 | 30 min | **Session 1 — Ouverture** : Pourquoi l'IA *maintenant* ? | Présentation + démo |
| 9h45 | 30 min | **Session 2 — CLI** : GitHub Copilot dans le terminal | Présentation + démo live |
| 10h15 | 10 min | Pause / Questions | — |
| 10h25 | 30 min | **Session 3 — VS Code** : L'éditeur augmenté | Présentation + démo live |
| 10h55 | 30 min | **Session 4 — Cloud Agent** : Déléguer à votre IA | Présentation + démo live |
| 11h25 | 20 min | **Table ronde** : L'IA selon votre rôle | Panel participatif |
| 11h45 | 15 min | Conclusion, ressources & prochaines étapes | Interactif |
| 12h00 | — | Fin de la matinée | — |

---

## 🔑 Détail des segments

### 9h00 – 9h10 | Accueil & café
- Réseautage informel à l'entrée.
- Afficher sur l'écran : le lien des labs ([copilot-dev-days.github.io](https://copilot-dev-days.github.io)) et le QR code d'inscription GitHub Copilot gratuit ([aka.ms/get-github-copilot-devdays](https://aka.ms/get-github-copilot-devdays)).

---

### 9h10 – 9h15 | Mot de bienvenue & brise-glace
**Durée :** 5 minutes  
**Animateur :** Présentateur principal

**Tour de salle express (mains levées) :**
> *"Qui est développeur ? Architecte ? Chef de projet / PM ? DevOps / SRE ? Étudiant ? Autre ?"*

Garder en tête la composition de la salle pour adapter les exemples pendant les démos.

---

### 9h15 – 9h45 | SESSION 1 — Ouverture
**Présentation :** `GitHub Copilot Dev Days Overview.pptx`  
**Outil :** Demo Time VSCode (slides traduits en français)  
**Durée :** 30 minutes

**Angle différenciateur :**  
Ne pas commencer par « voici l'autocomplétion de code ».
Commencer par **le contexte business et humain** :

1. **Pourquoi maintenant ?** (5 min)
   - L'IA n'est pas un buzzword de plus : montrer l'adoption réelle (statistiques GitHub Octoverse).
   - Le vrai changement : l'IA passe de *l'autocomplétion* à *l'agent*.

2. **GitHub Copilot — l'écosystème complet** (10 min)
   - IDE, CLI, cloud, mobile, PR review, docs...
   - L'insister sur la dimension multi-plateforme : ce n'est pas juste VS Code.

3. **Tableau des personas** (10 min) — présenter 4 cas concrets :
   | Rôle | Cas d'usage GitHub Copilot |
   |------|---------------------------|
   | 👩‍💻 Développeuse | Génération de code, tests unitaires, refactoring |
   | 🏗️ Architecte | Analyse de code existant, revue d'architecture, documentation |
   | 📋 Chef de projet | Rédaction de user stories, analyse d'impact, résumés de PR |
   | ⚙️ DevOps | Pipelines CI/CD, scripts shell, debugging de logs |

4. **Démo rapide d'impact** (5 min)
   - Montrer une PR review générée par Copilot sur un vrai repo.
   - Phrase clé à retenir : *"GitHub Copilot ne remplace pas votre équipe — il lui ajoute un coéquipier qui ne dort jamais."*

---

### 9h45 – 10h15 | SESSION 2 — GitHub Copilot CLI
**Présentation :** `GitHub Copilot Dev Days - CLI.pptx`  
**Outil :** Demo Time VSCode  
**Durée :** 30 minutes  
**Référence :** [Docs CLI](https://docs.github.com/en/copilot/how-tos/copilot-cli/cli-getting-started)

**Angle différenciateur :**  
Le CLI est souvent négligé au profit de l'IDE. C'est pourtant l'entrée la plus universelle — accessible sans VS Code, sans JetBrains, depuis n'importe quel terminal.

**Structure de la démo (en français) :**
1. `gh copilot explain` — expliquer une commande inconnue (exemple : une commande `kubectl` complexe)
2. `gh copilot suggest` — générer une commande depuis du langage naturel
   > *"Comment lister tous les fichiers modifiés il y a plus de 30 jours ?"*
3. **Cas DevOps** : débugger un message d'erreur avec `gh copilot explain`
4. **Cas étudiant** : comprendre Git sans mémoriser les commandes

**Message clé :** *"Si vous n'utilisez qu'un seul outil Copilot aujourd'hui, commencez par le CLI."*

---

### 10h15 – 10h25 | Pause & questions en direct
- Garder 2–3 questions de la salle.
- Afficher le lien des labs sur l'écran.

---

### 10h25 – 10h55 | SESSION 3 — GitHub Copilot dans VS Code
**Présentation :** `GitHub Copilot Dev Days - VS Code.pptx`  
**Outil :** Demo Time VSCode  
**Durée :** 30 minutes  
**Train the Trainer :** [▶️ Vidéo](https://youtu.be/eUDx_g_BLeA)

**Angle différenciateur :**  
Montrer les fonctionnalités **au-delà de l'autocomplétion** — celles que 80 % des utilisateurs n'exploitent pas encore.

**Structure de la démo :**
1. **Copilot Chat en ligne** — poser une question sur une fonction sélectionnée
2. **Inline edits** — modifier un bloc de code via instruction en français
3. **Copilot Edits** — modifier plusieurs fichiers simultanément avec une seule instruction
4. **Agent mode (@workspace)** — poser une question sur l'ensemble du projet
5. **Génération de tests** — un fichier de tests en un prompt

**Astuce à partager :**
> Utiliser `#file:`, `#selection`, `@workspace` dans le chat pour un contexte précis — la qualité des réponses est radicalement meilleure.

---

### 10h55 – 11h25 | SESSION 4 — GitHub Copilot Cloud Agent
**Présentation :** `GitHub Copilot Dev Days - Cloud Agent.pptx`  
**Outil :** Demo Time VSCode  
**Durée :** 30 minutes

**Angle différenciateur :**  
C'est la session la plus « futuriste » et celle qui résonne le plus auprès des PM et architectes — l'idée de *déléguer* une tâche de développement à une IA pendant qu'on fait autre chose.

**Structure de la démo :**
1. **Qu'est-ce qu'un coding agent ?** (5 min)
   - Différence entre l'autocomplétion, le chat et l'agent
   - L'agent : il lit le code, planifie, crée une PR, attend votre review

2. **Démo live** (15 min)
   - Assigner une issue GitHub simple à GitHub Copilot
   - Suivre l'avancement dans l'interface GitHub
   - Reviewer et merger la PR générée

3. **Cas d'usage par rôle** (10 min) :
   | Rôle | Ce que l'agent peut faire pour vous |
   |------|-------------------------------------|
   | Développeur | Corriger un bug d'une issue existante |
   | PM | Faire implémenter une user story documentée |
   | Architecte | Générer du scaffolding à partir d'une spec |

**Question clé à lancer dans la salle :**
> *"Si vous pouviez déléguer une tâche répétitive à un agent IA dès demain, laquelle serait-ce ?"*

---

### 11h25 – 11h45 | Table ronde — « L'IA selon votre rôle »
**Durée :** 20 minutes  
**Format :** Panel participatif (3–4 volontaires dans la salle)

**Objectif :** Ancrer l'expérience dans la réalité de chaque participant — sortir du mode "démo" pour entrer dans le mode "comment je l'utilise concrètement".

**Questions guides :**
1. *"Quel est votre rôle au quotidien, et comment l'IA s'y intègre (ou pourrait s'y intégrer) ?"*
2. *"Quelle démo de ce matin vous a le plus marqué ? Pourquoi ?"*
3. *"Quel est votre plus grand frein à l'adoption de ces outils dans votre équipe ?"*
4. *"Si vous deviez convaincre votre manager d'adopter GitHub Copilot, quel argument utiliseriez-vous ?"*

**Note d'animation :** Ne pas chercher les bonnes réponses — favoriser les tensions, les scepticismes, les vraies questions. C'est là que la conversation devient mémorable.

---

### 11h45 – 12h00 | Conclusion & prochaines étapes
**Durée :** 15 minutes

**Structure :**

1. **Récapitulatif visuel** (3 min)
   > Ce qu'on a vu ce matin :
   > - L'IA comme outil transversal, pas uniquement pour les devs
   > - CLI → accessibilité universelle
   > - VS Code → productivité avancée
   > - Cloud Agent → délégation et asynchronisme

2. **Ressources à emporter** (5 min)
   - 🌐 Labs : [copilot-dev-days.github.io](https://copilot-dev-days.github.io)
   - 🆓 Compte GitHub Copilot gratuit : [aka.ms/get-github-copilot-devdays](https://aka.ms/get-github-copilot-devdays)
   - 📖 CLI Docs : [docs.github.com/en/copilot/how-tos/copilot-cli](https://docs.github.com/en/copilot/how-tos/copilot-cli/cli-getting-started)
   - 🎬 Demo Time VSCode : [demotime.elio.dev](https://demotime.elio.dev/)
   - 💬 Discussions : [github.com/github/GitHub-Copilot-Dev-Days/discussions](https://aka.ms/githubcopilotdevdays/discussion)

3. **Appel à l'action** (5 min)
   - *"Pas besoin d'attendre : le plan gratuit GitHub Copilot est disponible dès aujourd'hui."*
   - Encourager à tester **une seule chose** cette semaine : la suggestion qui résonne le plus avec leur rôle.
   - Inviter à rejoindre la communauté GUM365 pour les prochains événements.

4. **Photo de groupe & réseautage** (2 min)
   - Moment informel pour les échanges post-session.

---

## 🎬 Préparation technique (avant 9h00)

### Outils à installer
- [ ] [Demo Time VSCode](https://demotime.elio.dev/) — pour tous les slides PPTX traduits en français
- [ ] GitHub Copilot Free activé sur le compte de démo
- [ ] CLI GitHub installé : `gh auth login` effectué
- [ ] Fichiers de démo prêts dans VS Code (repo local)

### Fichiers de démo recommandés
- Un repo Node.js / Python simple avec une issue open (pour Cloud Agent)
- Un script shell complexe (pour la démo CLI `explain`)
- Un fichier avec du code sans tests (pour la démo VS Code)

### Vérifications A/V
- [ ] Projector / écran testé
- [ ] Police et zoom de l'éditeur agrandis (≥ 16px) pour la projection
- [ ] Wi-Fi invité testé
- [ ] QR codes imprimés ou affichés numériquement

---

## 💡 Ce qui rend cette matinée différente

| Événement classique | Notre approche |
|---------------------|----------------|
| Focus développeur | Multi-rôles (dev, PM, archi, DevOps) |
| Un seul IDE | CLI + VS Code + Cloud (multi-plateforme) |
| Démos techniques | Cas d'usage ancrés dans le quotidien |
| Présentation unilatérale | Table ronde participative |
| En anglais | 100 % en français |
| Recette standard | Angle « et si ce n'était pas que pour les devs ? » |

---

*Organisé par la communauté GUM365 Montréal — dans le cadre de la série mondiale GitHub Copilot Dev Days 2026.*
