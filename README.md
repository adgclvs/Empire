# Empire

Empire est un jeu de stratégie en temps réel (RTS) développé en Java. Ce projet, inspiré de jeux comme Anno 1602 et Forge of Empires, permet de gérer des ressources, des habitants et des bâtiments pour faire prospérer une ville. Il se concentre sur une conception orientée objet et utilise JavaFX pour l'interface utilisateur.

## Fonctionnalités principales

- **Gestion des ressources** : Production et consommation de ressources (nourriture, bois, pierre, etc.).
- **Gestion des bâtiments** : Construction et gestion de bâtiments ayant des rôles spécifiques.
- **Gestion des habitants** : Logement des habitants, affectation aux bâtiments, gestion de la consommation de nourriture.
- **Carte interactive** : Interface graphique permettant de placer les bâtiments.
- **Temps réel** : Mécanisme basé sur des threads pour simuler le passage du temps.

## Prérequis

Avant de lancer le projet, assurez-vous que les éléments suivants sont installés :

- **Java** : Version 17 ou supérieure.
- **Maven** : Pour la gestion des dépendances.
- **JavaFX** : Version 20.
- **Un IDE** (comme IntelliJ IDEA, Eclipse, ou VS Code).

## Installation

1. Clonez le dépôt Git :

   ```bash
   git clone git@github.com:adgclvs/Empire.git
   cd Empire
   ```

2. Installez les dépendances Maven :

   ```bash
   mvn install
   ```

3. Lancez l'application :
   ```bash
   mvn javafx:run
   ```

## Structure du projet

Voici une vue d'ensemble de la structure du projet :

```plaintext
Empire/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── adrien/
│   │   │   │   ├── buildings/       # Classes pour gérer les bâtiments
│   │   │   │   ├── game/            # Gestion globale du jeu
│   │   │   │   ├── resources/       # Gestion des ressources
│   │   │   │   ├── controllers/     # Contrôleurs pour l'interface JavaFX
│   │   │   ├── MainApp.java         # Point d'entrée de l'application
│   │   ├── resources/               # Fichiers FXML et autres ressources
│   ├── test/                        # Tests unitaires
├── target/                          # Fichiers générés (non versionnés)
├── README.md
├── pom.xml                          # Configuration Maven
```

### Principales classes

- **`Resource`** : Représente les ressources du jeu (nourriture, bois, pierre, etc.).
- **`Building`** : Classe abstraite pour les bâtiments.
- **`GameManager`** : Gestion des bâtiments, des ressources, et des habitants.
- **`Map`** : Gestion de la carte où les bâtiments sont placés.
- **`MainApp`** : Point d'entrée du programme.

## Fonctionnement

### Objectif

- Construire et gérer une ville prospère en équilibrant production et consommation.
- Optimiser les ressources pour éviter les pénuries.

### Interactions utilisateur

1. Via l'interface graphique :
   - Ajouter ou retirer des bâtiments.
   - Affecter des travailleurs aux bâtiments.
   - Observer la production et la consommation en temps réel.

## Auteur(s)

- Adrien Gonçalves

## Notes supplémentaires

- L'interface graphique est minimaliste mais fonctionnelle. De futures améliorations pourraient inclure une meilleure jouabilité et des graphismes avancés.
- Les fichiers générés (comme le dossier `target`) sont exclus du dépôt grâce au fichier `.gitignore`.
