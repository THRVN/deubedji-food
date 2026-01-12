# 🔧 COMMANDES GIT - Guide de démarrage

> **Copie-colle ces commandes dans ton terminal, dans l'ordre**

---

## 📍 ÉTAPE 0.1 : Initialisation (10 min)

### 1️⃣ Créer le dossier du projet
```bash
# Crée le dossier principal
mkdir deubedji-food

# Entre dans le dossier
cd deubedji-food
```

### 2️⃣ Initialiser Git
```bash
# Initialise le dépôt Git
git init
```

### 3️⃣ Créer le fichier .gitignore
```bash
# Crée le fichier .gitignore
touch .gitignore
```

Ouvre `.gitignore` dans ton éditeur et ajoute :
```
# Fichiers système
.DS_Store
Thumbs.db

# Éditeurs
.vscode/
.idea/
*.swp
*.swo

# Temporaires
*.tmp
.cache/

# Node modules (si utilisé plus tard)
node_modules/
package-lock.json

# Logs
*.log
```

### 4️⃣ Configurer Git (si première fois)
```bash
# Configure ton nom (remplace par le tien)
git config --global user.name "Ton Nom"

# Configure ton email (remplace par le tien)
git config --global user.email "ton.email@exemple.com"
```

### 5️⃣ Premier commit
```bash
# Ajoute .gitignore au staging
git add .gitignore

# Crée le premier commit
git commit -m "Initial commit - Configuration Git"
```

✅ **VICTOIRE #1** : Ton projet est sous contrôle de version ! 🎉

---

## 📍 ÉTAPE 0.2 : Fichiers de suivi (10 min)

### 1️⃣ Copier les fichiers de suivi
Ces fichiers ont été créés par Claude, déplace-les dans ton dossier `deubedji-food/` :
- `ROADMAP.md`
- `TODO.md`
- `JOURNAL.md`
- `BLOCAGES.md`
- `README.md`

### 2️⃣ Commit des fichiers de suivi
```bash
# Ajoute tous les fichiers .md
git add *.md

# Commit
git commit -m "Ajout fichiers de suivi - ROADMAP, TODO, JOURNAL, BLOCAGES, README"
```

✅ **VICTOIRE #2** : Ta structure de gestion est en place ! 🎉

---

## 📍 ÉTAPE 0.3 : Arborescence (10 min)

### 1️⃣ Créer tous les dossiers
```bash
# Crée la structure complète
mkdir -p css js assets/icons assets/images data
```

### 2️⃣ Créer les fichiers vides
```bash
# Fichiers HTML
touch index.html

# Fichiers CSS
touch css/style.css css/components.css

# Fichiers JS
touch js/app.js js/equipments.js js/recipes.js js/storage.js

# Fichiers de données
touch data/equipments.json data/recipes.json data/adaptations.json
```

### 3️⃣ Créer des fichiers .gitkeep pour les dossiers vides
```bash
# Git n'aime pas les dossiers vides, on crée des fichiers invisibles
touch assets/icons/.gitkeep
touch assets/images/.gitkeep
```

### 4️⃣ Commit de la structure
```bash
# Ajoute tout
git add .

# Commit
git commit -m "Structure de dossiers et fichiers vides créée"
```

✅ **VICTOIRE #3** : Ton projet a une structure complète ! 🎉

---

## 🌐 OPTIONNEL : Connexion à GitHub

Si tu veux héberger ton projet sur GitHub (recommandé pour sauvegarder et partager) :

### 1️⃣ Créer un repo sur GitHub
- Va sur https://github.com
- Clique sur "New repository"
- Nom : `deubedji-food`
- Description : "App de recettes adaptée à mes ustensiles"
- Public ou Private (selon ta préférence)
- **Ne coche PAS** "Initialize with README" (on en a déjà un)
- Clique sur "Create repository"

### 2️⃣ Connecter ton projet local à GitHub
```bash
# Remplace "TON_USERNAME" par ton nom d'utilisateur GitHub
git remote add origin https://github.com/TON_USERNAME/deubedji-food.git

# Renomme la branche principale en "main" (standard actuel)
git branch -M main

# Envoie tout sur GitHub
git push -u origin main
```

✅ **VICTOIRE BONUS** : Ton code est sauvegardé en ligne ! 🎉

---

## 📚 COMMANDES GIT ESSENTIELLES

Tu utiliseras ces commandes à chaque étape :

### Vérifier l'état
```bash
# Voir quels fichiers ont changé
git status
```

### Ajouter des fichiers
```bash
# Ajouter un fichier spécifique
git add nom-du-fichier.ext

# Ajouter tous les fichiers modifiés
git add .
```

### Créer un commit
```bash
# Commit avec message
git commit -m "Description de ce qui a été fait"
```

### Voir l'historique
```bash
# Liste des commits
git log

# Version compacte
git log --oneline
```

### Envoyer sur GitHub (si configuré)
```bash
# Envoie les commits
git push
```

### Annuler des modifications (si besoin)
```bash
# Annuler les modifications d'un fichier (avant add)
git checkout -- nom-du-fichier.ext

# Retirer un fichier du staging (après add mais avant commit)
git reset nom-du-fichier.ext
```

---

## ✅ CHECKLIST DE DÉMARRAGE

Avant de passer à la Phase 1, vérifie que tu as bien :

- [ ] Créé le dossier `deubedji-food/`
- [ ] Initialisé Git (`git init`)
- [ ] Créé `.gitignore`
- [ ] Fait 3 commits (config, suivi, structure)
- [ ] Tous les dossiers créés (css/, js/, assets/, data/)
- [ ] Tous les fichiers vides créés
- [ ] (Optionnel) Projet connecté à GitHub

Si c'est bon, tu peux passer à la **Phase 1 - Étape 1.1** ! 🚀

---

## 🆘 EN CAS DE PROBLÈME

### "git: command not found"
→ Git n'est pas installé. Télécharge-le sur https://git-scm.com/

### "fatal: not a git repository"
→ Tu n'es pas dans le bon dossier ou git init n'a pas été fait
```bash
cd chemin/vers/deubedji-food
git init
```

### "nothing to commit"
→ Aucun fichier n'a été modifié ou ajouté au staging
```bash
git add .
git commit -m "Message"
```

---

**Tu es prêt ! Bonne chance pour la suite ! 💪**
