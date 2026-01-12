# 🍳 Deubedji-food

> **Une app de recettes qui s'adapte à TES ustensiles de cuisine**

![Status](https://img.shields.io/badge/status-en%20développement-yellow)
![Version](https://img.shields.io/badge/version-0.1.0-blue)

---

## 🎯 Le concept

Deubedji-food est une application web de recettes de cuisine avec une particularité : **les recettes s'adaptent automatiquement aux ustensiles que tu possèdes** !

Plus besoin de sauter une recette parce qu'elle demande un robot-mixeur que tu n'as pas. L'app te propose :
- ✅ Les recettes que tu peux faire avec ton équipement actuel
- 🔄 Des adaptations intelligentes si tu n'as pas tous les ustensiles
- 🛒 Des conseils d'achat priorisés (quels ustensiles acheter pour débloquer le plus de recettes)

---

## ✨ Fonctionnalités principales

### 🔐 Compte simple (sans email)
- Création de compte avec juste un pseudo
- Sauvegarde locale (localStorage) pour retrouver tes données

### 🔧 Gestion des ustensiles
- Sélectionne les ustensiles que tu possèdes
- Liste complète : four, casseroles, poêles, mixeur, etc.
- Mise à jour facile de ton inventaire

### 📖 Recettes adaptées
- Catalogue de recettes variées
- **Filtrage automatique** : vois seulement les recettes réalisables avec ton équipement
- **Suggestions d'adaptations** : alternatives si un ustensile manque
- Détails complets : ingrédients, étapes, temps, difficulté

### 🛒 Conseils d'achat
- Analyse de ce qui te manque
- **Priorisation intelligente** : quels ustensiles acheter en premier
- Montre combien de nouvelles recettes chaque achat te débloquerait

### ❤️ Favoris et recherche
- Sauvegarde tes recettes préférées
- Recherche par nom
- Filtres par catégorie (entrées, plats, desserts)

---

## 🛠️ Technologies utilisées

- **HTML5** - Structure
- **CSS3** - Styles (avec variables CSS et responsive design)
- **JavaScript (Vanilla)** - Logique applicative
- **LocalStorage** - Sauvegarde des données
- **JSON** - Base de données (recettes, ustensiles, adaptations)

**Aucun framework** - 100% vanilla pour apprendre les bases !

---

## 📁 Structure du projet

```
deubedji-food/
├── index.html              # Page principale
├── css/
│   ├── style.css           # Styles principaux
│   └── components.css      # Styles des composants
├── js/
│   ├── app.js              # Logique principale
│   ├── equipments.js       # Gestion des ustensiles
│   ├── recipes.js          # Gestion des recettes
│   └── storage.js          # Sauvegarde locale
├── data/
│   ├── equipments.json     # Liste des ustensiles
│   ├── recipes.json        # Base de recettes
│   └── adaptations.json    # Règles d'adaptation
└── assets/
    ├── icons/              # Icônes des ustensiles
    └── images/             # Images des recettes
```

---

## 🚀 Installation & Utilisation

### Prérequis
- Un navigateur web moderne (Chrome, Firefox, Safari, Edge)
- Aucune installation nécessaire !

### Lancement
1. Clone ou télécharge ce repository
2. Ouvre `index.html` dans ton navigateur
3. C'est tout ! 🎉

```bash
# Si tu veux utiliser un serveur local (optionnel)
python -m http.server 8000
# Puis ouvre http://localhost:8000
```

---

## 📖 Guide d'utilisation

1. **Première visite**
   - Entre un pseudo (pas d'email requis)
   - Sélectionne les ustensiles que tu possèdes
   - Valide

2. **Consulter les recettes**
   - Vois les recettes compatibles avec ton équipement
   - Clique sur une recette pour voir le détail
   - Suis les instructions étape par étape

3. **Gérer tes favoris**
   - Clique sur ♥ pour ajouter aux favoris
   - Retrouve-les dans "Mes favoris"

4. **Conseils d'achat**
   - Va dans "Conseils d'achat"
   - Vois quels ustensiles acheter en priorité
   - Découvre combien de recettes tu débloquerais

---

## 🗺️ Roadmap

Consulte [ROADMAP.md](ROADMAP.md) pour voir le plan détaillé de développement.

### Statut actuel : Phase 0 - Mise en place
- [x] Initialisation du projet
- [ ] Structure de base
- [ ] ...

---

## 🤝 Contribution

Ce projet est personnel et à but pédagogique, mais toute suggestion est la bienvenue !

---

## 👤 Auteur

Développé avec ❤️ et beaucoup de patience (TDAH-friendly development)

---

## 📝 Licence

Projet personnel - Utilisation libre pour l'apprentissage

---

## 🎓 Apprentissages visés

Ce projet me permet d'apprendre :
- [x] Structure d'un projet web
- [ ] Manipulation du DOM en JavaScript
- [ ] LocalStorage API
- [ ] Fetch API et JSON
- [ ] CSS Grid et Flexbox
- [ ] Responsive design
- [ ] Git et versioning
- [ ] Déploiement web

---

**Bon appétit et bon code ! 👨‍🍳💻**
