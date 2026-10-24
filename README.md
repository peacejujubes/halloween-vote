# 🎃 Halloween Costume Vote App

Une application web interactive, responsive et en temps réel pour organiser un concours du meilleur costume d'Halloween lors de vos soirées. 

Grâce à l'intégration de **Firebase Realtime Database**, tous les costumes inscrits et les votes effectués depuis les smartphones des invités sont synchronisés instantanément sur tous les écrans (téléphones, ordinateurs et écrans de projection).

---

## ✨ Fonctionnalités principales

- 🎭 **Inscription ouverte à tous** : Les participants ajoutent leur propre costume (nom, participant, description, avatar emoji ou photo) directement depuis la page d'accueil.
- ⚡ **Synchronisation Temps Réel (Firebase)** : Aucun rafraîchissement requis. Lorsqu'un costume est ajouté ou qu'un vote est émis, la liste et le classement se mettent à jour en direct.
- 📱 **Vote mobile & anti-triche** : Interface optimisée pour smartphone avec limitation du nombre de votes autorisés par personne (sauvegardé en `localStorage`).
- 🏆 **Podium et Classement interactif** : Visualisation stylisée du Top 3 (Podium) et du tableau complet des résultats.
- 🔐 **Portail Administrateur protégé (MDP : `1234`)** :
  - **Gestion des participations** : Modification et suppression des costumes en direct.
  - **Générateur de Code QR** : Génération dynamique et mode projection plein écran pour téléviseurs ou projecteurs.
  - **Contrôle du scrutin** : Verrouillage/déverrouillage des votes à distance et ajustement de la limite de votes par personne.
  - **Réinitialisation** : Remise à zéro des scores ou suppression globale de la liste.
- 🎉 **Animations d'Halloween** : Pluie de confettis thématiques (orange, violet, vert, jaune) lors du vote.

---

## 🛠️ Stack technique

- **Frontend** : HTML5, Vanilla JavaScript, Tailwind CSS (CDN).
- **Backend / Database** : Firebase Realtime Database (SDK v9 Compat).
- **Librairies** : 
  - `QRCode.js` pour la génération des codes QR.
  - `canvas-confetti` pour les animations de célébration.
  - `FontAwesome 6` pour l'iconographie.

---

## 🚀 Déploiement sur GitHub Pages

1. **Activez GitHub Pages** :
   - Rendez-vous sur votre dépôt GitHub : `Settings` > `Pages`.
   - Sous **Build and deployment**, choisissez la branche `main` (ou `master`) et conservez `/ (root)`.
   - Cliquez sur **Save**.

2. **Accédez au site** :
   - Votre application sera en ligne en quelques secondes à l'adresse :  
     `https://<votre-pseudo>.github.io/halloween-vote/`

---

## 🔐 Remarque sur la sécurité & Firebase

Les identifiants `firebaseConfig` présents dans `index.html` servent uniquement d'identifiants de projet et sont publiquement accessibles par nature dans les applications web front-end. La sécurité de la base de données est assurée directement par les **Règles de sécurité Firebase Realtime Database** définies dans la console Google Firebase.

> **Mot de passe Admin par défaut** : `1234`  
> *(Modifiable directement dans la fonction `handleAdminLogin` du fichier `index.html`)*

---

🎃 *Joyeux Halloween et que le meilleur costume gagne !*
