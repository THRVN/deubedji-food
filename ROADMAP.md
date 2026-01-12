# 🗺️ ROADMAP - Deubedji-food

> **Principe :** Chaque étape = 15-30 minutes max | Un commit = Une victoire 🎉

---

## 🟢 PHASE 0 : MISE EN PLACE (30 min total)

### [Étape 0.1] Initialisation du projet (10 min)
**Objectif :** Créer le dossier et initialiser Git
- Créer le dossier `deubedji-food`
- Ouvrir le terminal dans ce dossier
- Exécuter : `git init`
- Créer `.gitignore`
- **Commit :** "Initial commit - Structure de base"

### [Étape 0.2] Créer les fichiers de suivi (10 min)
**Objectif :** Mettre en place les outils de suivi
- Créer `ROADMAP.md` (ce fichier)
- Créer `TODO.md`
- Créer `JOURNAL.md`
- Créer `BLOCAGES.md`
- Créer `README.md`
- **Commit :** "Ajout fichiers de suivi"

### [Étape 0.3] Créer l'arborescence vide (10 min)
**Objectif :** Avoir tous les dossiers prêts
- Créer les dossiers : `css/`, `js/`, `assets/icons/`, `assets/images/`, `data/`
- Créer des fichiers vides : `index.html`, `css/style.css`, `js/app.js`
- **Commit :** "Structure de dossiers créée"

---

## 🟢 PHASE 1 : PAGE D'ACCUEIL BASIQUE (2h total)

### [Étape 1.1] HTML de base (20 min)
**Fichier :** `index.html`
- Créer la structure HTML5 de base
- Ajouter le `<head>` avec titre et meta
- Créer un `<header>` avec le nom du site
- Ajouter un `<main>` vide
- Ajouter un `<footer>` simple
- **Commit :** "Structure HTML de base"

### [Étape 1.2] CSS Reset et variables (15 min)
**Fichier :** `css/style.css`
- Ajouter un CSS reset simple
- Définir les variables CSS (couleurs principales)
- Définir la font de base
- **Commit :** "CSS reset et variables"

### [Étape 1.3] Styliser le header (20 min)
**Fichier :** `css/style.css`
- Centrer le titre
- Ajouter un fond de couleur
- Ajouter du padding
- Rendre responsive (test mobile)
- **Commit :** "Header stylisé"

### [Étape 1.4] Créer la zone de bienvenue (25 min)
**Fichiers :** `index.html`, `css/style.css`
- Ajouter une section "Bienvenue" dans le `<main>`
- Texte expliquant le concept
- Bouton "Commencer"
- Styliser la section
- **Commit :** "Page d'accueil avec bienvenue"

### [Étape 1.5] Tester et ajuster responsive (20 min)
**Fichiers :** `css/style.css`
- Ouvrir dans le navigateur
- Tester sur mobile (DevTools)
- Ajuster les tailles de texte
- Vérifier les marges
- **Commit :** "Responsive design page accueil"

---

## 🟢 PHASE 2 : SYSTÈME DE COMPTE SIMPLE (1h30 total)

### [Étape 2.1] Créer le HTML du formulaire de pseudo (20 min)
**Fichier :** `index.html`
- Créer une `<section id="login">`
- Input texte pour le pseudo
- Bouton "Créer mon compte"
- Cacher cette section par défaut (CSS)
- **Commit :** "Formulaire de création de compte"

### [Étape 2.2] Styliser le formulaire (15 min)
**Fichier :** `css/style.css`
- Centrer le formulaire
- Styliser l'input
- Styliser le bouton
- Ajouter des transitions hover
- **Commit :** "Style formulaire compte"

### [Étape 2.3] JavaScript - Afficher/cacher sections (25 min)
**Fichier :** `js/app.js`
- Sélectionner les éléments DOM
- Fonction pour afficher le formulaire quand on clique "Commencer"
- Cacher la section bienvenue
- Tester dans le navigateur
- **Commit :** "Navigation entre sections"

### [Étape 2.4] LocalStorage - Sauvegarder le pseudo (30 min)
**Fichier :** `js/storage.js`
- Créer une fonction `saveUserPseudo(pseudo)`
- Utiliser `localStorage.setItem()`
- Créer une fonction `getUserPseudo()`
- Utiliser `localStorage.getItem()`
- Tester dans la console
- **Commit :** "Sauvegarde du pseudo en local"

### [Étape 2.5] Lier le formulaire au storage (20 min)
**Fichier :** `js/app.js`
- Importer la fonction de storage
- Au clic sur "Créer mon compte", sauvegarder le pseudo
- Afficher un message de confirmation
- Rediriger vers la page principale
- **Commit :** "Création de compte fonctionnelle"

---

## 🟢 PHASE 3 : LISTE DES USTENSILES (2h total)

### [Étape 3.1] Créer le fichier de données ustensiles (20 min)
**Fichier :** `data/equipments.json`
- Créer un tableau JSON
- Ajouter 10 ustensiles de base (nom, id, catégorie, icône)
- Exemple : four, casserole, poêle, mixeur, etc.
- **Commit :** "Base de données ustensiles"

### [Étape 3.2] HTML de la page de sélection (20 min)
**Fichier :** `index.html`
- Créer une `<section id="equipments-selection">`
- Ajouter un titre "Mes ustensiles"
- Zone pour afficher la liste (vide pour l'instant)
- Bouton "Valider ma sélection"
- **Commit :** "Structure page ustensiles"

### [Étape 3.3] CSS de la grille d'ustensiles (25 min)
**Fichier :** `css/style.css`
- Créer une grille CSS (3 colonnes desktop, 2 mobile)
- Style pour les cartes d'ustensiles
- État sélectionné/non sélectionné
- **Commit :** "Style grille ustensiles"

### [Étape 3.4] JS - Charger les ustensiles depuis JSON (30 min)
**Fichier :** `js/equipments.js`
- Fonction `loadEquipments()` avec fetch()
- Parser le JSON
- Retourner le tableau
- Gérer les erreurs
- Tester dans la console
- **Commit :** "Chargement données ustensiles"

### [Étape 3.5] JS - Afficher les ustensiles dans le DOM (30 min)
**Fichiers :** `js/equipments.js`, `js/app.js`
- Fonction `displayEquipments(equipments)`
- Boucle pour créer les éléments HTML
- Injecter dans le DOM
- Appeler au chargement de la page
- **Commit :** "Affichage liste ustensiles"

### [Étape 3.6] JS - Sélection/désélection au clic (25 min)
**Fichier :** `js/equipments.js`
- Ajouter un event listener sur chaque ustensile
- Toggle de la classe "selected"
- Sauvegarder l'état dans un tableau
- Afficher le nombre d'ustensiles sélectionnés
- **Commit :** "Sélection ustensiles fonctionnelle"

---

## 🟢 PHASE 4 : SAUVEGARDE DES USTENSILES (1h total)

### [Étape 4.1] Storage - Fonction de sauvegarde (20 min)
**Fichier :** `js/storage.js`
- Créer `saveUserEquipments(equipmentsArray)`
- Convertir en JSON avec `JSON.stringify()`
- Sauvegarder dans localStorage
- **Commit :** "Fonction sauvegarde ustensiles"

### [Étape 4.2] Storage - Fonction de récupération (15 min)
**Fichier :** `js/storage.js`
- Créer `getUserEquipments()`
- Récupérer depuis localStorage
- Parser avec `JSON.parse()`
- Retourner le tableau
- **Commit :** "Fonction récupération ustensiles"

### [Étape 4.3] Lier la sélection au storage (25 min)
**Fichier :** `js/app.js`
- Au clic sur "Valider ma sélection"
- Récupérer les ustensiles sélectionnés
- Appeler `saveUserEquipments()`
- Afficher un message de confirmation
- **Commit :** "Sauvegarde sélection ustensiles"

### [Étape 4.4] Restaurer la sélection au chargement (20 min)
**Fichier :** `js/app.js`
- Au chargement de la page ustensiles
- Appeler `getUserEquipments()`
- Pré-cocher les ustensiles sauvegardés
- **Commit :** "Restauration sélection ustensiles"

---

## 🟢 PHASE 5 : BASE DE RECETTES (1h30 total)

### [Étape 5.1] Créer le fichier de recettes (30 min)
**Fichier :** `data/recipes.json`
- Créer 3 recettes simples
- Structure : id, titre, temps, difficulté, ingrédients, étapes, ustensiles requis
- Exemple : pâtes carbonara, omelette, salade composée
- **Commit :** "Base de données recettes"

### [Étape 5.2] HTML de la page recettes (20 min)
**Fichier :** `index.html`
- Créer `<section id="recipes-list">`
- Zone pour afficher les cartes de recettes
- Filtre par difficulté (plus tard)
- **Commit :** "Structure page recettes"

### [Étape 5.3] CSS des cartes de recettes (25 min)
**Fichier :** `css/style.css`
- Style pour les cartes (image, titre, tags)
- Grille responsive
- Effet hover
- **Commit :** "Style cartes recettes"

### [Étape 5.4] JS - Charger et afficher les recettes (30 min)
**Fichier :** `js/recipes.js`
- Fonction `loadRecipes()` avec fetch
- Fonction `displayRecipes(recipes)`
- Créer les cartes dynamiquement
- Tester l'affichage
- **Commit :** "Affichage liste recettes"

---

## 🟢 PHASE 6 : FILTRAGE PAR USTENSILES (2h total)

### [Étape 6.1] Logique de filtrage de base (30 min)
**Fichier :** `js/recipes.js`
- Fonction `filterRecipesByEquipments(recipes, userEquipments)`
- Vérifier si l'utilisateur a tous les ustensiles requis
- Retourner les recettes compatibles
- Tester dans la console
- **Commit :** "Logique de filtrage recettes"

### [Étape 6.2] Afficher seulement les recettes compatibles (25 min)
**Fichier :** `js/app.js`
- Récupérer les ustensiles de l'utilisateur
- Filtrer les recettes
- Afficher uniquement les compatibles
- **Commit :** "Filtrage recettes par ustensiles"

### [Étape 6.3] Indicateur visuel de compatibilité (20 min)
**Fichiers :** `css/style.css`, `js/recipes.js`
- Ajouter un badge "Compatible avec vos ustensiles"
- Couleur verte si compatible
- Gris si incompatible (avec liste ustensiles manquants)
- **Commit :** "Indicateurs compatibilité recettes"

### [Étape 6.4] Créer le fichier d'adaptations (25 min)
**Fichier :** `data/adaptations.json`
- Définir des règles de substitution
- Exemple : "four" peut être remplacé par "micro-ondes" pour certains plats
- Structure : ustensile manquant → alternatives + instructions
- **Commit :** "Base de données adaptations"

### [Étape 6.5] Suggérer des adaptations (30 min)
**Fichier :** `js/recipes.js`
- Fonction `suggestAdaptations(recipe, userEquipments)`
- Vérifier les ustensiles manquants
- Proposer des alternatives depuis adaptations.json
- Afficher les suggestions dans la carte
- **Commit :** "Suggestions d'adaptations"

---

## 🟢 PHASE 7 : PAGE DÉTAIL RECETTE (1h30 total)

### [Étape 7.1] HTML page détail (20 min)
**Fichier :** `index.html`
- Créer `<section id="recipe-detail">`
- Zones : image, titre, infos, ingrédients, étapes, ustensiles
- **Commit :** "Structure page détail recette"

### [Étape 7.2] CSS page détail (25 min)
**Fichier :** `css/style.css`
- Layout responsive (2 colonnes desktop)
- Style liste ingrédients
- Style étapes numérotées
- **Commit :** "Style page détail recette"

### [Étape 7.3] Navigation vers le détail (20 min)
**Fichier :** `js/app.js`
- Au clic sur une carte de recette
- Récupérer l'ID de la recette
- Cacher la liste, afficher le détail
- **Commit :** "Navigation vers détail recette"

### [Étape 7.4] Afficher les données de la recette (30 min)
**Fichier :** `js/recipes.js`
- Fonction `displayRecipeDetail(recipeId)`
- Récupérer la recette depuis les données
- Remplir tous les champs du DOM
- Afficher les adaptations si nécessaire
- **Commit :** "Affichage détail recette complet"

### [Étape 7.5] Bouton retour et navigation (15 min)
**Fichier :** `js/app.js`
- Ajouter un bouton "← Retour aux recettes"
- Événement pour revenir à la liste
- **Commit :** "Navigation retour depuis détail"

---

## 🟢 PHASE 8 : CONSEILS D'ACHAT (1h total)

### [Étape 8.1] Analyser les ustensiles manquants (25 min)
**Fichier :** `js/equipments.js`
- Fonction `getMissingEquipments(allEquipments, userEquipments)`
- Comparer les listes
- Retourner les ustensiles manquants
- **Commit :** "Analyse ustensiles manquants"

### [Étape 8.2] Calculer la priorité d'achat (30 min)
**Fichier :** `js/equipments.js`
- Pour chaque ustensile manquant, compter combien de recettes il débloque
- Trier par nombre de recettes débloquées
- Ajouter un score de priorité
- **Commit :** "Calcul priorité achats"

### [Étape 8.3] Page conseils d'achat (20 min)
**Fichiers :** `index.html`, `css/style.css`
- Créer `<section id="shopping-advice">`
- Afficher la liste des ustensiles recommandés
- Ordre : plus prioritaire en premier
- Montrer combien de recettes seront débloquées
- **Commit :** "Page conseils d'achat"

---

## 🟢 PHASE 9 : AMÉLIORATIONS UX (1h30 total)

### [Étape 9.1] Barre de recherche recettes (30 min)
**Fichiers :** `index.html`, `js/recipes.js`
- Ajouter un input de recherche
- Filtrer par nom de recette en temps réel
- **Commit :** "Barre de recherche recettes"

### [Étape 9.2] Filtres par catégorie (25 min)
**Fichiers :** `index.html`, `js/recipes.js`
- Boutons : Entrées / Plats / Desserts
- Filtrer les recettes affichées
- **Commit :** "Filtres par catégorie"

### [Étape 9.3] Système de favoris (35 min)
**Fichiers :** `js/storage.js`, `js/recipes.js`
- Bouton ♥ sur chaque recette
- Sauvegarder dans localStorage
- Page "Mes favoris"
- **Commit :** "Système de favoris"

---

## 🟢 PHASE 10 : FINITIONS (1h total)

### [Étape 10.1] Page À propos (20 min)
**Fichiers :** `index.html`, `css/style.css`
- Section expliquant le projet
- Crédits
- **Commit :** "Page À propos"

### [Étape 10.2] Mode sombre (30 min)
**Fichiers :** `css/style.css`, `js/app.js`
- Définir les variables CSS pour le thème sombre
- Bouton toggle
- Sauvegarder la préférence
- **Commit :** "Mode sombre"

### [Étape 10.3] Tests finaux et corrections (30 min)
- Tester toutes les fonctionnalités
- Vérifier le responsive
- Corriger les petits bugs
- **Commit :** "Tests et corrections finales"

---

## 🎉 PHASE 11 : DÉPLOIEMENT (30 min)

### [Étape 11.1] Préparer pour GitHub Pages (15 min)
- Vérifier que tous les chemins sont relatifs
- Créer un repo GitHub
- Push du code
- **Commit :** "Préparation déploiement"

### [Étape 11.2] Activer GitHub Pages (15 min)
- Activer GitHub Pages dans les settings
- Tester l'URL publique
- Partager le lien !
- **Commit :** "Site en ligne !"

---

## 📊 RÉSUMÉ PAR PHASE

| Phase | Durée estimée | Commits |
|-------|---------------|---------|
| 0. Mise en place | 30 min | 3 |
| 1. Page d'accueil | 2h | 5 |
| 2. Système de compte | 1h30 | 5 |
| 3. Liste ustensiles | 2h | 6 |
| 4. Sauvegarde ustensiles | 1h | 4 |
| 5. Base recettes | 1h30 | 4 |
| 6. Filtrage | 2h | 5 |
| 7. Détail recette | 1h30 | 5 |
| 8. Conseils achat | 1h | 3 |
| 9. Améliorations UX | 1h30 | 3 |
| 10. Finitions | 1h | 3 |
| 11. Déploiement | 30 min | 2 |
| **TOTAL** | **~15h** | **48 commits** |

---

## 💡 CONSEILS POUR RÉUSSIR

### ✅ Bonnes pratiques
- ⏱️ **Timer de 25 min** : Mets un minuteur pour chaque session
- 🎯 **Une étape = Une session** : Ne fais qu'une seule étape par session
- 📝 **Note tout** : Utilise `JOURNAL.md` après chaque session
- 🔄 **Commit systématique** : Chaque étape terminée = 1 commit
- 🚫 **Ne saute pas d'étapes** : L'ordre est important

### 🛑 Si tu bloques
1. Note le problème dans `BLOCAGES.md`
2. Prends une pause de 10 minutes
3. Relis l'étape depuis le début
4. Cherche l'erreur dans la console du navigateur
5. Demande de l'aide avec le contexte précis

### 🎮 Gamification
- [X] Phase 0 → Badge "Démarrage" 🏁
- [ ] Phase 1 → Badge "Designer" 🎨
- [ ] Phase 2 → Badge "Authentificateur" 🔐
- [ ] Phase 3 → Badge "Organisateur" 🔧
- [ ] Phase 5 → Badge "Chef" 👨‍🍳
- [ ] Phase 11 → Badge "Lanceur" 🚀

---

**Prochaine étape :** Commence par l'Étape 0.1 - Initialisation du projet
