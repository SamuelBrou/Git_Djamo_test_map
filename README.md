# Git Maestro Google Maps

Ce projet contient une suite de tests automatisés pour l’application **Google Maps (Android)** en utilisant [Maestro](https://maestro.mobile.dev/).  
L’objectif est de vérifier la recherche, la génération d’itinéraires.

---

## 📂 Structure du projet


├── .maestro/screenshots/ # Captures d’écran des tests 1-Search.yaml # Test de recherche d'une destination
├── 2-Modify.yaml # Test de modification du point de départ
├── 3-Itineraire.yaml # Test d'itinéraire
├── E2E.yaml # Scénario end-to-end regroupant tous les tests
├── .maestro/screenshots/ # Captures d’écran des tests
└── README.md # Documentation du projet

## 🛠️ Prérequis

- macOS, Linux ou Windows
- **Java JDK 17+**
- [Maestro](https://maestro.mobile.dev/) installé :
  ```bash
  brew tap mobile-dev-inc/tap
  brew install maestro
Un émulateur Android (Androïd Studio)

## Exécution des tests

1. Lancer un test individuel
bash
Copier le code
maestro test 1-Search.yaml
2. Lancer tous les tests end-to-end
bash
Copier le code
maestro test E2E.yaml
3. Ajouter des tags pour filtrer
Par exemple, pour exécuter uniquement les tests de type smoke :

bash
Copier le code
maestro test E2E.yaml --tag smoke