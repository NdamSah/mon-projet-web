# Épreuve de GIT - Gestion du versionning d'un Site Web Statique
**Étudiante :** Mariatou Sah Ndam 
**Classe :**B1 
**Examinateur :** BOGNI-DANCHI 
**Institution :** École Supérieure Française KEYCE 

## 1. Stratégie de branchement adoptée
Conformément aux consignes du sujet, nous avons mis en place un flux de travail rigoureux :
- `main` : Branche finale contenant le code stable et validé prêt pour la publication.
- `dev` : Branche d'intégration globale où toutes les fonctionnalités testées sont rassemblées.
- `test/frontend` : Branche intermédiaire servant à réaliser les tests d'intégration visuelle et fonctionnelle.
- `feature/*` : Branches de développement isolées par fonctionnalité (HTML, CSS, JS).

## 2. Étapes suivies lors du projet
1. **Initialisation** du dépôt Git local dans le dossier du projet.
2. **Création des branches de fonctionnalités** (`feature/html-structure`, `feature/css-theme`, `feature/js-interactions`).
3. **Création et correction des fichiers de base** (`index.html`, `services.html`, `contact.html`, `style.css`, `script.js`).
4. **Fusions successives** en respectant le flux recommandé : `feature/*` ➔ `test/frontend` ➔ `dev` ➔ `main`.
5. **Création du dépôt distant sur GitHub** et téléversement (push) de l'ensemble des branches locales.

## 3. Commandes Git utilisées
- `git init` : Initialiser le dépôt local.
- `git checkout -b <nom_branche>` : Créer et basculer sur une nouvelle branche.
- `git status` : Suivre l'état des fichiers modifiés ou non-suivis.
- `git add .` : Indexer les fichiers avant le commit.
- `git commit -m "message"` : Enregistrer les instantanés du projet.
- `git merge <branche>` : Fusionner les branches.
- `git log --oneline --graph --all` : Visualiser l'arborescence complète et valider les fusions.
- `git push -u origin main` & `git push --all origin` : Publier le travail sur GitHub.