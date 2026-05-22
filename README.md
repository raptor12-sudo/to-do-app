# Todo App — Projet de fin d'études

Application mobile de gestion de tâches développée avec Apache Cordova et jQuery UI, dans le cadre d'un projet étudiant.

## Aperçu

Application todo list mobile-first pensée pour iOS et Android. Elle permet de créer, organiser et suivre ses tâches du quotidien avec une interface inspirée des apps natives iOS.

## Fonctionnalités

- Ajouter une tâche avec un niveau de priorité (faible, moyenne, haute)
- Glisser une tâche vers la droite pour la supprimer
- Appuyer sur une tâche pour afficher les boutons Fermer / Compléter
- Double-taper sur le nom d'une tâche pour la modifier
- Tag de statut sur chaque tâche : **En cours** ou **Terminé**
- Filtrer les tâches : Toutes / En cours / Terminées
- Barre de progression indiquant le pourcentage de tâches complétées
- Statistiques en haut : nombre total de tâches et tâches en cours
- Réordonner les tâches par drag & drop (sur la bande de priorité)
- Mode sombre / clair
- Données sauvegardées localement via `localStorage`

## Stack technique

| Technologie | Rôle |
|---|---|
| Apache Cordova | Framework mobile hybride (iOS / Android) |
| jQuery 3.7 | Manipulation du DOM et événements |
| jQuery UI 1.13 | Widgets (dialog, sortable) + thème ThemeRoller |
| HTML / CSS / JS | Interface et logique applicative |
| localStorage | Persistance des données |

## Structure du projet

```
todo-app/
├── www/
│   ├── index.html        # Structure de la page
│   ├── css/
│   │   └── style.css     # Styles et thème sombre
│   └── js/
│       └── app.js        # Logique de l'application
├── config.xml            # Configuration Cordova
└── platforms/
    ├── ios/              # Build iOS (Xcode)
    └── android/          # Build Android
```

## Installation

### Prérequis

- Node.js >= 14
- Apache Cordova installé globalement
- Xcode (pour iOS) ou Android Studio (pour Android)

```bash
npm install -g cordova
```

### Cloner et installer

```bash
git clone <url-du-repo>
cd todo-app
npm install
```

### Ajouter les plateformes

```bash
cordova platform add ios
cordova platform add android
```

### Lancer sur simulateur

```bash
# iOS
cordova run ios

# Android
cordova run android
```

### Build de production

```bash
cordova build ios --release
cordova build android --release
```

## Utilisation

| Action | Geste |
|---|---|
| Ajouter une tâche | Bouton **+** en bas à droite |
| Supprimer une tâche | Glisser vers la droite |
| Cocher / décocher | Bouton rond à droite de la tâche |
| Voir les actions | Appuyer une fois sur la tâche |
| Modifier le texte | Double-taper sur le nom |
| Réordonner | Glisser la bande colorée à gauche |
| Changer le thème | Bouton 🌙 / ☀️ en haut à droite |

## Captures d'écran

> *(à ajouter)*

## Auteur

**Tidiane** — Étudiant M2 Génie Informatique, option Réseaux et Systèmes d'Information  
École Supérieure Polytechnique (ESP/UCAD) — Dakar, Sénégal

## Licence

Projet académique — usage éducatif uniquement.
