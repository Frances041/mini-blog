# ?? Mini Blog HTML/CSS

Ce projet est un mini blog créé pour apprendre à utiliser **Git** et **GitHub** à travers un projet pratique.

## 🚀 Objectifs du projet
- Comprendre les commandes Git de base et avancées  
- Apprendre à travailler avec les branches (`branch`, `checkout`, `merge`)  
- Gérer les erreurs et synchroniser un projet local avec GitHub  
- Simuler une collaboration professionnelle (pull requests, merges, conflits)  
- Publier un site avec **GitHub Pages**

## 📂 Structure du projet
mini-blog/
│
├── index.html → Page d'accueil du blog
├── style.css → Feuille de style principale
├── article.html → Premier article du blog
├── about.html → Page À propos (Phase 5)
└── README.md → Documentation du projet

## 🧩 Étapes réalisées

### ✅ **Phase 1 — Mise en place du projet**
1. Création du dossier de projet et initialisation du dépôt local (`git init`)
2. Premier commit avec le fichier `index.html` (`git commit -m "Premier commit"`)
3. Création d’une branche pour le design (`git branch design`)
4. Ajout du fichier `style.css` et fusion avec la branche principale (`git merge design`)
5. Publication du projet sur GitHub (`git remote add origin` + `git push -u origin main`)

---

### ✅ **Phase 2 — Ajout d’une nouvelle fonctionnalité**
1. Création d’une branche `article1` pour ajouter une nouvelle page
2. Création du fichier `article.html` et commit de la modification
3. Retour sur la branche principale (`git checkout main`)
4. Fusion de `article1` dans `main` (`git merge article1`)
5. Suppression de la branche devenue inutile (`git branch -d article1`)
6. Mise à jour du dépôt GitHub (`git push`)

---

### ✅ **Phase 3 — Gérer les erreurs et synchroniser le projet**

#### 🧯 Annuler ou corriger des commits
- `git reset --soft HEAD~1` → Annule le dernier commit, garde les fichiers modifiés  
- `git reset --hard HEAD~1` → Annule le commit **et** les modifications  
- `git revert <id>` → Annule un commit déjà poussé sur GitHub en créant un commit inverse  

#### 🔄 Synchroniser avec GitHub
- `git pull` → Récupère et fusionne les changements du dépôt GitHub  
- `git fetch` → Récupère les infos distantes sans les fusionner  

#### ✍️ Exemple concret
- Modification du fichier `index.html` → commit → annulation du commit avec `git reset`  
- Édition du `README.md` directement sur GitHub → mise à jour locale avec `git pull`  

---

### ✅ **Phase 4 — Entraînement complet aux 25 commandes Git**
- Pratique sur : `add`, `commit`, `branch`, `merge`, `reset`, `stash`, `tag`, etc.
- Création d’une branche de test (`test-git`)
- Renommage, suppression, et gestion de fichiers
- Création d’un tag :  
  `git tag -a v1.0 -m "Version stable du mini blog"`
- Publication du tag :  
  `git push origin --tags`

---

### ✅ **Phase 5 — Collaboration simulée**
1. Création d’une nouvelle branche de fonctionnalité :  
   `git checkout -b feature-a-propos`
2. Ajout du fichier `about.html` et commit
3. Push de la nouvelle branche sur GitHub :  
   `git push -u origin feature-a-propos`
4. Création d’une **Pull Request** (PR) via GitHub  
5. Fusion de la PR dans `main`  
6. Suppression de la branche fusionnée  
7. Mise à jour locale du dépôt :  
   `git checkout main` + `git pull`
8. Simulation d’un conflit de fusion (optionnel)  
   - Résolution manuelle puis commit :  
     `git add .` + `git commit -m "Résolution du conflit"`

---

## 🧠 Compétences Git maîtrisées (25 commandes)

`init`, `status`, `add`, `commit`, `log`, `diff`, `branch`, `checkout`,  
`merge`, `remote`, `push`, `pull`, `fetch`, `reset`, `revert`,  
`rm`, `mv`, `stash`, `stash pop`, `tag`, `branch -d`, `branch -m`,  
`checkout -b`, `push origin --tags`, `git config`.

---

## 📘 Prochaine étape — Phase 6
➡️ **Publication en ligne avec GitHub Pages**
- Héberger le mini blog directement sur GitHub  
- Générer une URL publique du type :  
  `https://frances041.github.io/mini-blog/`  
- Apprendre à mettre à jour le site automatiquement via Git

---

🧑‍💻 *Projet de formation réalisé par Frances pour apprendre et maîtriser Git & GitHub, pas à pas.*