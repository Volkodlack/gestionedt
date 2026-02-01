# 👔 Thierry Carles - Gestion du Personnel

Application web moderne de gestion des emplois du temps et du personnel pour l'entreprise Thierry Carles.

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-Private-red)

---

## 🎯 Fonctionnalités

### 📊 Tableau de bord
- Vue d'ensemble des employés présents
- Suivi des retards du jour
- Liste des absents avec motifs

### 👥 Gestion des employés
- Création et modification des profils
- Enregistrement des horaires hebdomadaires
- ID unique pour chaque employé

### 📝 Modifications d'emploi du temps
- **Absences** : Gestion par période avec motifs personnalisables
- **Retards & départs anticipés** : Comptabilisation en minutes
- **Heures supplémentaires** : Enregistrement précis (arrivée/départ)

### 🏗️ Gestion des chantiers
- Enregistrement des chantiers avec localisation
- **Calcul automatique des zones** (0-3) selon la distance
- **Calcul automatique des paniers** selon convention collective
- Assignation flexible des employés par période

### 📤 Export Excel
- Export annuel par employé
- Un onglet par mois
- Format professionnel et coloré
- Calculs automatiques :
  - Total des heures travaillées
  - Montant des paniers
  - Heures supplémentaires
  - Congés payés pris
  - Retards cumulés
  - Absences par motif

---

## 🔐 Sécurité

- Connexion protégée par mot de passe
- Possibilité de changer le mot de passe
- Données stockées localement (pas de serveur)
- Fichier JSON pour sauvegarde externe

---

## 💾 Sauvegarde des données

L'application utilise un système de sauvegarde par fichier :

1. **💾 Bouton "Sauvegarder"** : Télécharge un fichier JSON avec toutes vos données
2. **📂 Bouton "Charger"** : Restaure les données depuis un fichier JSON
3. **⚠️ Indicateur** : Vous alerte des modifications non sauvegardées

### ⚡ Important
- Les données ne sont PAS stockées sur GitHub
- Vous devez sauvegarder régulièrement votre fichier JSON
- Gardez plusieurs versions de sauvegarde

---

## 🚀 Installation

### Option 1 : Utilisation locale
1. Téléchargez `index.html`
2. Double-cliquez pour l'ouvrir dans votre navigateur
3. Connexion par défaut : `admin` / `admin`

### Option 2 : Hébergement en ligne (GitHub Pages)
1. Forkez ce dépôt
2. Activez GitHub Pages dans Settings → Pages
3. Accédez à votre application via l'URL fournie

📖 **Guide complet d'hébergement** : Consultez `GUIDE_HEBERGEMENT.md`

---

## 🎨 Design

- Interface moderne et épurée
- Couleurs inspirées du logo de l'entreprise (violet/rose)
- Responsive (PC, tablette, mobile)
- Animations fluides
- Feedback visuel pour chaque action

---

## 🛠️ Technologies

- **HTML5** : Structure
- **React 18** : Framework JavaScript
- **Babel** : Transpilation JSX
- **XLSX.js** : Export Excel
- **CSS3** : Design moderne avec gradients et animations

---

## 📱 Compatibilité

- ✅ Chrome / Edge (recommandé)
- ✅ Firefox
- ✅ Safari
- ✅ Mobile (iOS / Android)

---

## 📋 Utilisation

### Première connexion
1. Ouvrez l'application
2. Connexion : `admin` / `admin`
3. **Changez immédiatement le mot de passe** (Tableau de bord → Changer le mot de passe)

### Workflow type
1. **Employés** : Créez vos employés avec leurs horaires
2. **Chantiers** : Enregistrez vos chantiers (zones calculées automatiquement)
3. **Modifications** : Ajoutez absences, retards, heures sup au quotidien
4. **Export** : Générez les plannings Excel mensuellement
5. **Sauvegarde** : Cliquez sur 💾 Sauvegarder régulièrement

---

## 🏢 Convention collective

L'application respecte la convention collective des chauffagistes et plombiers :

### Zones et paniers
- **Zone 0** (< 10 km) : 0 €
- **Zone 1** (10-30 km) : 7,50 €
- **Zone 2** (30-60 km) : 12,50 €
- **Zone 3** (> 60 km) : 17,50 €

Le calcul se fait automatiquement depuis l'adresse de l'entreprise :
📍 40 Chem. de la Gare, 59144 Wargnies-le-Grand

---

## ⚙️ Configuration

### Changement du mot de passe
1. Tableau de bord → "Changer le mot de passe"
2. Entrez le mot de passe actuel
3. Définissez le nouveau (min. 4 caractères)
4. **N'oubliez pas de sauvegarder après !**

---

## 🔄 Mise à jour

Pour mettre à jour l'application :
1. **Sauvegardez vos données** (💾 Sauvegarder)
2. Remplacez `index.html` par la nouvelle version
3. Rechargez la page (Ctrl + F5)
4. **Chargez vos données** (📂 Charger)

---

## 📞 Support

Pour toute question ou problème :
- Consultez `GUIDE_HEBERGEMENT.md` pour l'installation
- Vérifiez la console du navigateur (F12) pour les erreurs
- Essayez dans un autre navigateur
- Effacez le cache (Ctrl + Shift + Suppr)

---

## 📄 License

© 2026 Thierry Carles - Tous droits réservés
Application développée pour un usage privé interne.

---

## 🎯 Roadmap future (idées)

- [ ] Synchronisation cloud automatique
- [ ] Notifications pour les retards/absences
- [ ] Graphiques et statistiques avancées
- [ ] Export PDF des plannings
- [ ] Multi-utilisateurs avec rôles
- [ ] Application mobile native

---

**Développé avec ❤️ pour Thierry Carles**
