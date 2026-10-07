# simplixTV 📺✨

> **Lecteur IPTV moderne, fluide et performant pour Windows, Android TV, Smartphone et Tablette.**

[![Version](https://img.shields.io/badge/version-1.3.4-orange.svg?style=flat-square)](https://github.com/romain-chpl/simplixTV/releases)
[![Flutter](https://img.shields.io/badge/Flutter-%5E3.13.2-02569B.svg?style=flat-square&logo=flutter)](https://flutter.dev)
[![Platforms](https://img.shields.io/badge/plateformes-Windows%20%7C%20Android%20%7C%20Android%20TV-blue.svg?style=flat-square)](https://github.com/romain-chpl/SimplixTV/releases)
[![License](https://img.shields.io/badge/licence-Propriétaire%20%2F%20Non--commercial-lightgrey.svg?style=flat-square)](https://github.com/romain-chpl/SimplixTV/blob/main/LICENSE)

---

## 🌟 Présentation

**simplixTV** est une application IPTV conçue pour offrir une expérience de visionnage haut de gamme, fluide et sans latence sur l'ensemble de vos écrans. Que vous soyez confortablement installé dans votre salon devant votre téléviseur avec une télécommande, sur votre ordinateur de bureau ou en déplacement avec votre smartphone, simplixTV s'adapte automatiquement à votre contexte d'utilisation.

Grâce à son moteur de lecture multimédia propulsé par **`libmpv` (media_kit)** avec accélération matérielle GPU et à sa base de données locale **Drift (SQLite)**, l'application gère des catalogues de dizaines de milliers de flux sans le moindre ralentissement.

---

## 🚀 Fonctionnalités Clés

### 📺 Direct TV (Live Stream)
- **Zapping instantané** et démarrage ultra-rapide des flux.
- **Guide des programmes (EPG)** intégré pour visualiser les émissions en cours et à venir.
- **Badges de qualité automatiques** : détection dynamique `4K`, `FHD`, `HD`.
- **Organisation par catégories & bouquets** avec navigation intuitive.
- **Bouton favori dédié** : accessible directement via télécommande (D-Pad) ou clic souris pour épingler vos chaînes fétiches.

### ⏪ Mode Replay TV (Télévision de rattrapage)
- Accès aux archives TV pour les chaînes compatibles (jusqu'à 7 jours selon votre fournisseur).
- **Sélecteur de date et guide horaire** pour retrouver facilement vos émissions manquées.
- Prise en charge de la timeline avec saut rapide (±30s) et reprise de lecture.

### 🎬 Films & Séries (VOD)
- Présentation moderne au format affiches / posters cinématographiques.
- **Fiches de détails enrichies** : synopsis, note, casting, durée, genre et date de sortie.
- **Gestionnaire de séries avancé** : sélection des saisons et épisodes avec statut de visionnage.
- **Reprise de lecture intelligente** : reprise automatique là où vous vous étiez arrêté.

### ⭐ Gestion Multi-Favoris & Accueil Dynamique
- Épinglage indépendant des chaînes Direct, Replay, Films et Séries.
- **Carrousel Favoris** interactif directement sur l'écran d'accueil pour un accès en un clic.

### 🔍 Recherche Globale Multi-Médias
- Recherche temps réel instantanée à travers l'intégralité du catalogue (Direct, Films, Séries).
- Filtres rapides pour isoler les types de contenus souhaités.

### 🎮 Ergonomie 100% Adaptative & Navigation TV (D-Pad)
- **Mode TV complet** : pilotable intégralement à la télécommande (flèches directionnelles, touche centrale, retour), avec contours de focus haute visibilité (`focusHighlight`).
- **Mode Bureau (Windows)** : raccourcis clavier dédiés, plein écran instantané, ajustements à la molette.
- **Mode Mobile & Tablette** : interface tactile optimisée avec disposition verticale réactive.

---

## ⌨️ Raccourcis Clavier & Télécommande TV

| Commande | Action Clavier | Télécommande Android TV |
| :--- | :--- | :--- |
| **Naviguer** | `Flèches Directionnelles` | `D-pad (Haut / Bas / Gauche / Droite)` |
| **Sélectionner / Valider** | `Entrée` ou `Pavé numérique Entrée` | `Bouton Central (OK / Select)` |
| **Retour / Fermer OSD** | `Échap` ou `Retour arrière` | `Bouton Retour (Back)` |
| **Lecture / Pause** | `Espace` | `OK` (sur l'élément Pause de l'OSD) |
| **Avancer / Reculer (30s)** | `Flèche Droite` / `Flèche Gauche` (sur timeline) | `D-pad Droite / Gauche` |
| **Plein écran** | `F` ou Double-clic | Plein écran automatique |
| **Muet (Mute)** | `M` | Bouton dédié télécommande |

---

## 🛠️ Stack Technique

- **Framework :** [Flutter](https://flutter.dev) (Dart 3.x)
- **Gestion d'État :** [Riverpod](https://riverpod.dev)
- **Moteur Vidéo :** [media_kit](https://github.com/media-kit/media-kit) (`libmpv` avec accélération matérielle décodage GPU DXVA2/D3D11VA/MediaCodec)
- **Base de Données Locale :** [Drift (SQLite)](https://drift.simonbinder.eu/) pour la persistance locale ultra-rapide des flux et de l'historique
- **Réseau :** [Dio](https://pub.dev/packages/dio) avec gestion fine des timeouts et du streaming Xtream Codes
- **Stockage Sécurisé :** `flutter_secure_storage` pour la préservation des identifiants API

---

## 📦 Installation & Démarrage

### Téléchargements :
  **Page de téléchargement** : [Realease](https://github.com/romain-chpl/SimplixTV/releases)
- **Windows :**
  Télécharger le fichier `simplix_installer.exe` depuis la page Realease, puis suivez les instructions de l'installateur.
- **Android/TV :**
  Télécharger le fichier `SimplixTV.apk` depuis la page Realease, puis ouvrez le fichier sur un appareil ou une tv Android pour l'installer.

---

## ⚙️ Configuration Requise

- **Identifiants Xtream Codes :**
  - URL du serveur (ex. `http://mon-serveur-iptv.com:8080`)
  - Nom d'utilisateur
  - Mot de passe
- **Systèmes d'exploitation recommandés :**
  - Windows 10 / 11 (64-bit)
  - Android 8.0 (Oreo) ou supérieur (compatible Google TV & Android TV)

---

## 📄 Licence & Mentions

Projet développé par **romain-chpl** pour simplixTV.  
Ce logiciel est un lecteur multimédia IPTV indépendant et ne fournit aucun contenu, chaîne ou abonnement par lui-même. Vous devez disposer d'un abonnement légal auprès de votre fournisseur de services.
