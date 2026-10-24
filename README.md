# 🎃 Halloween Costume Vote App

Une application web interactive, légère et clé en main pour organiser un concours du meilleur costume d'Halloween lors de vos soirées. Elle permet aux invités d'inscrire leur costume, de voter facilement depuis leur téléphone via un **Code QR**, et d'afficher le classement en temps réel.

---

## ✨ Fonctionnalités principales

- 🎭 **Inscription ouverte à tous** : Les participants ajoutent leur propre costume (nom, participant, description, avatar ou image) directement depuis la page d'accueil.
- 📱 **Vote mobile facile** : Interface optimisée pour smartphone avec limitation anti-triche du nombre de votes par personne (via `localStorage`).
- 🏆 **Podium et Classement en direct** : Visualisation du Top 3 (Podium) et du tableau complet mis à jour instantanément.
- 🔐 **Portail Administrateur protégé (MDP : `1234`)** :
  - **Gestion des costumes** : Modification et suppression des participations.
  - **Générateur de Code QR** : Génération automatique et mode projection plein écran pour téléviseurs ou moniteurs.
  - **Contrôle du scrutin** : Verrouillage/déverrouillage des votes et ajustement de la limite de votes max par personne.
  - **Réinitialisation** : Remise à zéro des scores ou nettoyage de la liste.
- 🎉 **Effets d'Halloween** : Confettis thématiques (orange, violet, vert) et design sombre (*Spooky Theme*).

---

## 🚀 Déploiement rapide sur GitHub Pages

1. **Activez GitHub Pages** :
   - Allez dans votre dépôt GitHub : `Settings` > `Pages`.
   - Sous **Build and deployment**, choisissez la branche `main` (ou `master`) et conservez `/ (root)`.
   - Cliquez sur **Save**.

2. **Accédez au site** :
   - Votre application sera accessible en quelques secondes à l'adresse :  
     `https://<votre-pseudo>.github.io/halloween-vote/`

---

## 🛠️ Stack technique

- **HTML5 & Vanilla JavaScript** (aucun framework complexe requis).
- **Tailwind CSS** (via CDN pour un style responsive et rapide).
- **FontAwesome** (icônes).
- **QRCode.js** (génération dynamique de codes QR).
- **Canvas Confetti** (animation de célébration lors du vote).

---

## 🔒 Configuration du MDP Admin

Le mot de passe par défaut du panneau d'administration est **`1234`**.  
Pour le modifier, éditez directement la ligne suivante dans le fichier `index.html` :

```javascript
if (input === '1234') { ... }
