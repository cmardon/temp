# TP – Création d’un Platformer 2D sous Godot

## 🎯 Objectifs pédagogiques

- Maîtriser les bases de la création d’un jeu de plateforme 2D.
- Manipuler les `TileMap`, `KinematicBody2D` (ou `CharacterBody2D` selon version), collisions et le moteur physique.
- Implémenter un personnage jouable avec un système de mouvement simple.
- Ajouter des éléments de décor à l’aide d’un `TileSet` fourni.

---

## 🧰 Matériel fourni

- Un projet Godot vide avec :
  - Les `TileSet` déjà importés.
  - Une scène de base prête à être utilisée.

---

## 🗺️ Étapes à suivre

### 1. Mise en place du niveau

- Créez une nouvelle scène nommée `Level1` de type `Node2D`.
- Ajoutez un `TileMap` à cette scène.
- Associez le `TileSet` fourni au `TileMap`.
- Construisez un petit niveau de test (sols, murs, plateformes...).

### 2. Création du joueur

- Créez une nouvelle scène nommée `Player` :
  - Type : `CharacterBody2D` (ou `KinematicBody2D` si Godot 3).
  - Ajoutez-y :
    - Un `Sprite2D` pour le visuel.
    - Un `CollisionShape2D` avec une forme adaptée.
  - Implémentez les mouvements basiques :
    - Déplacement gauche/droite.
    - Saut avec détection du sol.
    - Gravité et vitesse de chute.

### 3. Intégration du joueur dans le niveau

- Instanciez la scène `Player` dans `Level1`.
- Positionnez le joueur à un endroit approprié dans le niveau.
- Ajoutez une `Camera2D` pour suivre le joueur :
  - Activez le mode `Current`.
  - Centrez-la sur le joueur.

### 4. Bonus (facultatif)

- Ajoutez des éléments d'interaction simples :
  - Pièces à collecter (`Area2D`).
  - Ennemis basiques (déplacement gauche-droite).
  - Checkpoints ou système de mort/restart.

---

## 🧠 Conseils

- Testez souvent ! Une erreur simple peut casser tout le comportement du joueur.
- Utilisez les `groups` pour organiser vos objets (ennemis, collectibles...).
- N’hésitez pas à consulter la documentation officielle de Godot.

---

## ✅ À rendre

- Le projet complet compressé (`.zip`).
- Un fichier texte ou `.md` décrivant :
  - Ce que vous avez implémenté.
  - Ce que vous avez tenté mais pas terminé.
  - Ce que vous voudriez ajouter avec plus de temps.

---

## ⏱️ Durée estimée

2 heures.

---

## 🎮 Résultat attendu

Un petit jeu de plateforme jouable avec :
- Un niveau construit à partir de tiles.
- Un personnage contrôlable capable de sauter et se déplacer.
