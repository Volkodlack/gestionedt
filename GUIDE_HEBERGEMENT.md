# 🚀 Guide d'hébergement - Thierry Carles Gestion du Personnel

## Vue d'ensemble

Ce guide vous explique comment héberger votre application de gestion du personnel sur **GitHub Pages** avec **Cloudflare** pour bénéficier d'un accès en ligne tout en conservant la sauvegarde locale des données.

---

## 📋 Prérequis

- Un compte GitHub (gratuit)
- Un compte Cloudflare (gratuit)
- Le fichier `gestion-emploi-temps.html`
- Le fichier `thierry-carles-data.json` (vos données sauvegardées)

---

## 🔧 Étape 1 : Créer un dépôt GitHub

### 1.1 Créer le dépôt

1. Allez sur [github.com](https://github.com)
2. Cliquez sur le bouton **"+"** en haut à droite → **"New repository"**
3. Nommez votre dépôt : `thierry-carles-gestion`
4. Sélectionnez **Public** (nécessaire pour GitHub Pages gratuit)
5. ✅ Cochez **"Add a README file"**
6. Cliquez sur **"Create repository"**

### 1.2 Uploader les fichiers

1. Dans votre dépôt, cliquez sur **"Add file"** → **"Upload files"**
2. Uploadez le fichier `gestion-emploi-temps.html`
3. **Renommez-le en `index.html`** (important !)
4. Cliquez sur **"Commit changes"**

---

## 🌐 Étape 2 : Activer GitHub Pages

1. Dans votre dépôt, allez dans **"Settings"** (⚙️)
2. Dans le menu de gauche, cliquez sur **"Pages"**
3. Sous **"Source"**, sélectionnez la branche **"main"**
4. Cliquez sur **"Save"**
5. Attendez quelques minutes
6. Votre site sera accessible à : `https://votre-nom.github.io/thierry-carles-gestion/`

---

## ⚡ Étape 3 : Configurer Cloudflare (Optionnel mais recommandé)

Cloudflare offre :
- 🔒 HTTPS automatique et sécurisé
- ⚡ Meilleure performance (CDN)
- 🛡️ Protection DDoS
- 📊 Statistiques de trafic
- 🌍 Possibilité d'utiliser un nom de domaine personnalisé

### 3.1 Créer un compte Cloudflare

1. Allez sur [cloudflare.com](https://www.cloudflare.com)
2. Créez un compte gratuit

### 3.2 Option A : Utiliser un domaine personnalisé

Si vous avez un domaine (ex: `thierry-carles.fr`) :

1. Ajoutez votre domaine dans Cloudflare
2. Changez les serveurs DNS chez votre registrar
3. Dans Cloudflare :
   - Allez dans **"DNS"** → **"Records"**
   - Ajoutez un enregistrement **CNAME** :
     - **Name** : `gestion` (ou `@` pour le domaine racine)
     - **Target** : `votre-nom.github.io`
     - **Proxy status** : ✅ Proxied (orange)
4. Dans GitHub Settings → Pages, ajoutez votre domaine personnalisé

### 3.2 Option B : Utiliser Cloudflare Pages (Alternative complète)

Au lieu de GitHub Pages, vous pouvez héberger directement sur Cloudflare Pages :

1. Dans Cloudflare, allez dans **"Pages"**
2. Cliquez sur **"Connect to Git"**
3. Autorisez Cloudflare à accéder à votre GitHub
4. Sélectionnez le dépôt `thierry-carles-gestion`
5. Configuration :
   - **Framework preset** : None
   - **Build command** : (laissez vide)
   - **Build output directory** : `/`
6. Cliquez sur **"Save and Deploy"**
7. Votre site sera disponible sur `thierry-carles-gestion.pages.dev`

---

## 💾 Gestion des données

### ⚠️ Important à comprendre

L'application stocke les données de **2 façons** :

1. **Dans le navigateur** (localStorage) - temporaire
2. **Dans un fichier JSON** que vous téléchargez - permanent

### Comment ça marche en ligne ?

#### Première utilisation sur un nouvel appareil :
1. Ouvrez l'application en ligne
2. Connectez-vous (admin / admin)
3. Cliquez sur **"📂 Charger"**
4. Sélectionnez votre fichier `thierry-carles-data.json`
5. Toutes vos données sont restaurées !

#### Travail quotidien :
1. Faites vos modifications dans l'application
2. Cliquez sur **"💾 Sauvegarder"** régulièrement
3. Le fichier JSON mis à jour se télécharge
4. **Gardez ce fichier en lieu sûr** (OneDrive, Google Drive, etc.)

#### Sauvegarde automatique recommandée :
- Créez un dossier **"Sauvegardes Thierry Carles"** sur OneDrive/Google Drive
- À chaque sauvegarde, mettez le fichier JSON dans ce dossier
- Renommez avec la date : `thierry-carles-data-2026-02-01.json`
- Gardez plusieurs versions (historique)

---

## 🔐 Sécurité

### Changer le mot de passe par défaut

**IMPORTANT** : Le mot de passe par défaut est `admin`

1. Connectez-vous à l'application
2. Dans le **Tableau de Bord**, cliquez sur **"Changer le mot de passe"**
3. Entrez un nouveau mot de passe sécurisé
4. Cliquez sur **"💾 Sauvegarder"** pour enregistrer le changement dans votre fichier JSON

### Bonnes pratiques :

- ✅ Changez le mot de passe dès la première connexion
- ✅ Utilisez un mot de passe fort (minimum 8 caractères)
- ✅ Ne partagez jamais votre fichier JSON (il contient toutes vos données)
- ✅ Si le dépôt GitHub est **Public**, les gens peuvent voir le code mais PAS vos données
- ⚠️ Pour plus de sécurité, mettez le dépôt en **Private** (nécessite GitHub Pro pour Pages)

---

## 🔄 Mettre à jour l'application

Si je vous envoie une nouvelle version avec des corrections :

1. Téléchargez d'abord vos données : **"💾 Sauvegarder"**
2. Dans GitHub, supprimez l'ancien `index.html`
3. Uploadez la nouvelle version
4. Attendez 1-2 minutes que GitHub Pages se mette à jour
5. Rechargez votre navigateur (Ctrl + F5)
6. Cliquez sur **"📂 Charger"** pour restaurer vos données

---

## 🎯 Workflow recommandé

### Au bureau :
1. Ouvrez l'application en ligne
2. Chargez votre fichier JSON du jour
3. Travaillez normalement
4. **Sauvegardez plusieurs fois par jour**
5. En fin de journée, sauvegardez une dernière fois

### Sur un autre ordinateur :
1. Ouvrez la même URL
2. Chargez votre dernier fichier JSON
3. Continuez votre travail
4. Sauvegardez avant de partir

### Synchronisation :
- Utilisez OneDrive, Google Drive, ou Dropbox
- Mettez le fichier JSON dans un dossier synchronisé
- Tous vos appareils auront accès à la dernière version

---

## 📱 Accès mobile

L'application fonctionne aussi sur smartphone et tablette :

1. Ouvrez l'URL dans votre navigateur mobile
2. Pour un accès rapide, ajoutez-la à l'écran d'accueil :
   - **iPhone** : Safari → Partager → "Sur l'écran d'accueil"
   - **Android** : Chrome → Menu → "Ajouter à l'écran d'accueil"

---

## ❓ FAQ

### Q : Mes données sont-elles sécurisées ?
**R :** Oui ! Les données ne sont JAMAIS envoyées à GitHub ou Cloudflare. Elles restent dans votre navigateur et dans votre fichier JSON local.

### Q : Puis-je travailler hors ligne ?
**R :** Oui ! Une fois la page chargée, elle fonctionne hors ligne. Pensez juste à sauvegarder.

### Q : Que se passe-t-il si je perds mon fichier JSON ?
**R :** Vous perdez toutes vos données. C'est pourquoi il faut faire des sauvegardes régulières.

### Q : Plusieurs personnes peuvent-elles utiliser l'application ?
**R :** Oui, mais chacun doit charger et sauvegarder le même fichier JSON. Il n'y a pas de synchronisation automatique en temps réel.

### Q : Comment partager le fichier JSON avec mes collègues ?
**R :** Utilisez un dossier partagé OneDrive/Google Drive. Tous les utilisateurs doivent :
1. Charger le fichier au début
2. Travailler
3. Sauvegarder dans le dossier partagé
4. Les autres rechargent le nouveau fichier

⚠️ **Attention** : Ne travaillez pas en même temps sur le même fichier, sinon vous allez vous écraser les données mutuellement.

---

## 🆘 Support

Si vous rencontrez des problèmes :

1. **Effacer le cache** : Ctrl + Shift + Suppr (tous les navigateurs)
2. **Essayer un autre navigateur** : Chrome, Firefox, Edge
3. **Vérifier la console** : F12 → Console (pour voir les erreurs)
4. **Recharger complètement** : Ctrl + F5

---

## 📊 Résumé des avantages de cette solution

| Avantage | Description |
|----------|-------------|
| 🆓 **Gratuit** | GitHub Pages et Cloudflare sont 100% gratuits |
| 🌍 **Accessible partout** | De n'importe quel appareil avec internet |
| 🔒 **Sécurisé** | HTTPS automatique, données en local |
| ⚡ **Rapide** | CDN Cloudflare = chargement ultra-rapide |
| 💾 **Contrôle total** | Vous possédez vos données (fichier JSON) |
| 📱 **Multi-plateforme** | PC, Mac, Linux, mobile, tablette |
| 🔄 **Facile à mettre à jour** | Uploadez simplement un nouveau fichier |

---

## ✅ Checklist de déploiement

- [ ] Créer le dépôt GitHub
- [ ] Uploader `index.html`
- [ ] Activer GitHub Pages
- [ ] Tester l'accès à l'URL
- [ ] Se connecter avec admin/admin
- [ ] Changer le mot de passe
- [ ] Créer quelques employés de test
- [ ] Tester la sauvegarde (bouton 💾)
- [ ] Tester le chargement (bouton 📂)
- [ ] Configurer Cloudflare (optionnel)
- [ ] Ajouter l'URL aux favoris
- [ ] Former les utilisateurs

---

**🎉 Votre application est maintenant en ligne et prête à l'emploi !**

Pour toute question, n'hésitez pas à me contacter.
