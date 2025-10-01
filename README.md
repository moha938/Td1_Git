<div align="center">

# 🚀 TD1 - Prise en main de Git & GitHub

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com)
[![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)](https://git-scm.com/)
[![Markdown](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white)](https://www.markdownguide.org/)

**Bienvenue dans votre premier projet de prise en main de Git et GitHub ! 🎉**

*Un guide complet pour maîtriser les bases du contrôle de version*

[🔗 Voir le projet](https://github.com/moha938/Td1_Git) • [📚 Documentation Git](https://git-scm.com/doc) • [💡 GitHub Guides](https://guides.github.com/)

</div>

---

## 📑 Table des matières

- [🎯 Objectifs du TD](#-objectifs-du-td)
- [🔧 Prérequis](#-prérequis)
- [📖 Introduction](#-introduction)
- [🌱 Les bases de Git](#-les-bases-de-git)
- [🐙 Les bases de GitHub](#-les-bases-de-github)
- [💻 Exercices pratiques](#-exercices-pratiques)
- [📚 Commandes essentielles](#-commandes-essentielles)
- [🎓 Ressources utiles](#-ressources-utiles)
- [👥 Contributeurs](#-contributeurs)
- [📄 Licence](#-licence)

---

## 🎯 Objectifs du TD

À la fin de ce TD, vous serez capable de :

- ✅ Comprendre les concepts fondamentaux de Git
- ✅ Créer et gérer un dépôt Git local
- ✅ Effectuer des commits et gérer l'historique
- ✅ Créer et manipuler des branches
- ✅ Utiliser GitHub pour collaborer
- ✅ Créer des pull requests et gérer des issues
- ✅ Contribuer à des projets open source

---

## 🔧 Prérequis

Avant de commencer, assurez-vous d'avoir :

- 🖥️ Git installé sur votre machine ([Télécharger Git](https://git-scm.com/downloads))
- 🌐 Un compte GitHub ([Créer un compte](https://github.com/join))
- 📝 Un éditeur de texte (VS Code, Sublime Text, etc.)
- 💻 Un terminal/ligne de commande

### Vérifier l'installation de Git

```bash
git --version
```

### Configuration initiale

```bash
git config --global user.name "Votre Nom"
git config --global user.email "votre.email@example.com"
```

---

## 📖 Introduction

### Qu'est-ce que Git ? 🤔

**Git** est un système de contrôle de version distribué qui permet de :
- 📝 Suivre les modifications de votre code
- 🔄 Revenir à des versions antérieures
- 👥 Collaborer efficacement en équipe
- 🔀 Gérer plusieurs versions en parallèle

### Qu'est-ce que GitHub ? 🌐

**GitHub** est une plateforme d'hébergement de code qui utilise Git et offre :
- ☁️ Hébergement de dépôts Git dans le cloud
- 👥 Outils de collaboration (issues, pull requests)
- 📊 Suivi de projets et gestion d'équipe
- 🌍 Partage et découverte de projets open source

---

## 🌱 Les bases de Git

### 🗂️ Les trois états de Git

Git gère trois états principaux pour vos fichiers :

1. **Modifié (Modified)** : Le fichier a été changé mais pas encore enregistré
2. **Indexé (Staged)** : Le fichier modifié est marqué pour être inclus dans le prochain commit
3. **Validé (Committed)** : Les données sont stockées en toute sécurité dans votre base de données locale

```
Working Directory  →  Staging Area  →  Git Repository
     (modifié)          (indexé)         (validé)
```

### 🔄 Le workflow Git de base

```bash
# 1. Initialiser un dépôt
git init

# 2. Ajouter des fichiers à l'index
git add fichier.txt
git add .  # Ajouter tous les fichiers

# 3. Créer un commit
git commit -m "Message descriptif du commit"

# 4. Voir l'historique
git log
git log --oneline --graph --all

# 5. Voir le statut
git status
```

### 🌿 Les branches

Les branches permettent de développer des fonctionnalités de manière isolée :

```bash
# Créer une nouvelle branche
git branch nom-de-la-branche

# Se déplacer sur une branche
git checkout nom-de-la-branche

# Créer et se déplacer en une commande
git checkout -b nom-de-la-branche

# Fusionner une branche
git checkout main
git merge nom-de-la-branche

# Lister les branches
git branch -a
```

---

## 🐙 Les bases de GitHub

### 📦 Créer un dépôt

1. Cliquez sur le bouton **"New repository"**
2. Donnez un nom à votre dépôt
3. Ajoutez une description (optionnel)
4. Choisissez entre public/privé
5. Cliquez sur **"Create repository"**

### 🔗 Lier un dépôt local à GitHub

```bash
# Ajouter un dépôt distant
git remote add origin https://github.com/username/repository.git

# Vérifier les dépôts distants
git remote -v

# Pousser les modifications
git push -u origin main

# Récupérer les modifications
git pull origin main
```

### 🔀 Pull Requests

Les **Pull Requests** sont essentielles pour la collaboration :

1. 🔨 Créez une branche pour votre fonctionnalité
2. 💾 Effectuez vos commits
3. 📤 Poussez la branche sur GitHub
4. 🔀 Créez une Pull Request
5. 👀 Attendez la revue de code
6. ✅ Fusionnez après approbation

### 📝 Issues

Les **Issues** permettent de :
- 🐛 Signaler des bugs
- 💡 Proposer des améliorations
- 📋 Organiser les tâches
- 💬 Discuter des fonctionnalités

---

## 💻 Exercices pratiques

### Exercice 1 : Premier commit 🎯

```bash
# 1. Créer un nouveau dossier
mkdir mon-premier-projet
cd mon-premier-projet

# 2. Initialiser Git
git init

# 3. Créer un fichier
echo "# Mon Premier Projet" > README.md

# 4. Ajouter et commiter
git add README.md
git commit -m "Premier commit : ajout du README"
```

### Exercice 2 : Travailler avec des branches 🌿

```bash
# 1. Créer une branche de développement
git checkout -b developpement

# 2. Modifier un fichier
echo "Nouvelle ligne" >> README.md

# 3. Commiter les changements
git add README.md
git commit -m "Ajout d'une nouvelle ligne"

# 4. Retourner sur main et fusionner
git checkout main
git merge developpement
```

### Exercice 3 : Pousser sur GitHub 🚀

```bash
# 1. Créer un dépôt sur GitHub (via l'interface web)

# 2. Lier votre dépôt local
git remote add origin https://github.com/votre-username/votre-repo.git

# 3. Pousser vos commits
git push -u origin main

# 4. Vérifier sur GitHub !
```

### Exercice 4 : Collaborer avec une Pull Request 🤝

```bash
# 1. Forker un projet sur GitHub

# 2. Cloner votre fork
git clone https://github.com/votre-username/projet-forke.git

# 3. Créer une branche
git checkout -b ma-contribution

# 4. Faire des modifications et commiter
git add .
git commit -m "Ma contribution"

# 5. Pousser la branche
git push origin ma-contribution

# 6. Créer une Pull Request sur GitHub
```

---

## 📚 Commandes essentielles

### Configuration

```bash
git config --global user.name "Nom"          # Définir le nom
git config --global user.email "email"       # Définir l'email
git config --list                            # Voir la configuration
```

### Création et clonage

```bash
git init                                     # Initialiser un dépôt
git clone <url>                              # Cloner un dépôt
```

### Modifications

```bash
git status                                   # Voir l'état des fichiers
git add <fichier>                            # Ajouter à l'index
git add .                                    # Ajouter tous les fichiers
git commit -m "message"                      # Créer un commit
git commit -am "message"                     # Add + commit
```

### Historique

```bash
git log                                      # Voir l'historique
git log --oneline                            # Historique condensé
git log --graph --all --oneline              # Historique graphique
git diff                                     # Voir les modifications
```

### Branches

```bash
git branch                                   # Lister les branches
git branch <nom>                             # Créer une branche
git checkout <branche>                       # Changer de branche
git checkout -b <branche>                    # Créer et changer
git merge <branche>                          # Fusionner une branche
git branch -d <branche>                      # Supprimer une branche
```

### Dépôts distants

```bash
git remote add origin <url>                  # Ajouter un dépôt distant
git push origin <branche>                    # Pousser vers le dépôt
git pull origin <branche>                    # Récupérer les modifications
git fetch                                    # Télécharger sans fusionner
```

### Annulations

```bash
git checkout -- <fichier>                    # Annuler modifications
git reset HEAD <fichier>                     # Retirer de l'index
git revert <commit>                          # Annuler un commit
```

---

## 🎓 Ressources utiles

### Documentation officielle

- 📖 [Documentation Git](https://git-scm.com/doc)
- 📖 [GitHub Docs](https://docs.github.com/)
- 📖 [Pro Git Book](https://git-scm.com/book/fr/v2) (en français)

### Tutoriels interactifs

- 🎮 [Learn Git Branching](https://learngitbranching.js.org/?locale=fr_FR)
- 🎮 [GitHub Skills](https://skills.github.com/)
- 🎮 [Git Immersion](http://gitimmersion.com/)

### Aide-mémoires

- 📋 [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
- 📋 [GitHub Git Cheat Sheet](https://training.github.com/downloads/github-git-cheat-sheet.pdf)

### Vidéos et cours

- 🎥 [Git & GitHub Crash Course](https://www.youtube.com/results?search_query=git+github+tutorial)
- 🎥 [OpenClassrooms - Gérez du code avec Git et GitHub](https://openclassrooms.com/fr/courses/7162856-gerez-du-code-avec-git-et-github)

---

## 👥 Contributeurs

Ce projet a été créé dans le cadre d'un TD de prise en main de Git et GitHub.

Vous souhaitez contribuer ? N'hésitez pas à :
- 🐛 Signaler des bugs via les [Issues](../../issues)
- 💡 Proposer des améliorations
- 🔀 Soumettre des Pull Requests

---

## 📄 Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

<div align="center">

### 🌟 N'oubliez pas de mettre une étoile si ce projet vous a aidé ! 🌟

**Fait avec ❤️ pour apprendre Git & GitHub**

[⬆️ Retour en haut](#-td1---prise-en-main-de-git--github)

</div>
