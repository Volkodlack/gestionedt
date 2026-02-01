# ⚡ Démarrage Rapide - 5 minutes

## 🎯 Objectif
Avoir l'application fonctionnelle en ligne en moins de 5 minutes.

---

## 📝 Étapes (GitHub Pages)

### 1️⃣ Créer le dépôt (1 min)
1. Allez sur [github.com/new](https://github.com/new)
2. Nom : `thierry-carles-gestion`
3. Type : **Public**
4. ✅ Cochez "Add a README file"
5. Cliquez **"Create repository"**

### 2️⃣ Uploader le fichier (1 min)
1. Cliquez **"Add file"** → **"Upload files"**
2. Glissez `gestion-emploi-temps.html`
3. ⚠️ **IMPORTANT** : Renommez-le en `index.html`
4. Cliquez **"Commit changes"**

### 3️⃣ Activer Pages (1 min)
1. Allez dans **"Settings"** ⚙️
2. Menu gauche → **"Pages"**
3. Source : **main** branch
4. Cliquez **"Save"**
5. Attendez 1-2 minutes

### 4️⃣ Tester (1 min)
1. GitHub vous donne une URL : `https://votre-nom.github.io/thierry-carles-gestion/`
2. Ouvrez cette URL
3. Connexion : `admin` / `admin`
4. ✅ **Ça marche !**

### 5️⃣ Sécuriser (1 min)
1. Dans l'app → **Tableau de bord**
2. Cliquez **"Changer le mot de passe"**
3. Nouveau mot de passe (min. 4 caractères)
4. Cliquez **"💾 Sauvegarder"** (important !)

---

## 🎓 Première utilisation

### Créer un employé
1. Onglet **"Employés"**
2. Bouton **"+ Ajouter un employé"**
3. Remplissez :
   - Nom
   - Horaires de la semaine
4. **"Enregistrer"**

### Créer un chantier
1. Onglet **"Chantiers"**
2. Bouton **"+ Nouveau chantier"**
3. Remplissez :
   - Nom du chantier
   - Adresse complète (pour le calcul de zone)
   - Dates de début et fin
4. **"Enregistrer"**
5. Cliquez **"Assigner"** pour ajouter des employés

### Enregistrer une absence
1. Onglet **"Modifications"**
2. Section **"Absences"**
3. Remplissez :
   - Employé
   - Dates (début et fin)
   - Motif
4. **"Enregistrer l'absence"**

### Exporter un planning
1. Onglet **"Export"**
2. Sélectionnez un employé
3. Cliquez **"Exporter le planning"**
4. Un fichier Excel se télécharge 📊

---

## 💾 Sauvegarder vos données

### Quand sauvegarder ?
- ✅ Après avoir créé des employés
- ✅ Après avoir créé des chantiers
- ✅ En fin de journée
- ✅ Avant de fermer le navigateur
- ✅ Quand le badge ⚠️ "Non sauvegardé" apparaît

### Comment ?
1. Cliquez sur **"💾 Sauvegarder"** (en haut à droite)
2. Un fichier `thierry-carles-data.json` se télécharge
3. Rangez-le dans un dossier sûr (OneDrive, Google Drive...)
4. **Gardez plusieurs versions** (avec la date dans le nom)

### Restaurer les données
1. Cliquez sur **"📂 Charger"**
2. Sélectionnez votre fichier JSON
3. ✅ Toutes vos données sont de retour !

---

## 🔄 Workflow quotidien

**Matin :**
1. Ouvrez l'app
2. Chargez votre fichier JSON du jour précédent
3. Travaillez normalement

**Pendant la journée :**
- Ajoutez absences, retards, heures sup
- Créez de nouveaux chantiers
- Assignez des employés

**Soir :**
1. Sauvegardez (💾)
2. Mettez le fichier JSON dans votre dossier cloud
3. Fermez

---

## 📱 Utiliser sur mobile

1. Ouvrez l'URL de l'app sur votre téléphone
2. Menu → **"Ajouter à l'écran d'accueil"**
3. Maintenant c'est comme une app ! 📲

---

## ⚠️ Points importants

### ✅ À FAIRE
- Sauvegarder régulièrement
- Changer le mot de passe par défaut
- Garder plusieurs versions de sauvegarde
- Tester l'export Excel dès le début

### ❌ À NE PAS FAIRE
- Ne JAMAIS effacer le seul fichier JSON
- Ne PAS nettoyer le cache sans avoir sauvegardé
- Ne PAS travailler à plusieurs en même temps sans coordination

---

## 🆘 Problème ?

### L'app ne charge pas
1. Attendez 5 minutes (GitHub Pages met du temps)
2. Ctrl + F5 (recharge complète)
3. Essayez en navigation privée
4. Essayez un autre navigateur

### J'ai perdu mes données
- Vérifiez votre dossier Téléchargements
- Cherchez `thierry-carles-data*.json`
- Restaurez la dernière version valide

### Le mot de passe ne fonctionne plus
- Avez-vous sauvegardé après l'avoir changé ?
- Si non, il est resté sur "admin"
- Si oui, chargez votre fichier JSON

---

## 🎯 Checklist première journée

- [ ] Dépôt GitHub créé
- [ ] Application en ligne accessible
- [ ] Mot de passe changé
- [ ] 2-3 employés créés avec horaires
- [ ] 1 chantier de test créé
- [ ] 1 employé assigné au chantier
- [ ] 1 absence enregistrée
- [ ] Export Excel testé
- [ ] Première sauvegarde effectuée
- [ ] Fichier JSON bien rangé
- [ ] Test de restauration OK

---

## 📚 Pour aller plus loin

- Lisez le **GUIDE_HEBERGEMENT.md** complet
- Consultez le **README.md** pour toutes les fonctionnalités
- Configurez Cloudflare pour plus de performances

---

**🎉 Félicitations ! Vous êtes prêt à gérer vos employés efficacement !**

*Temps total : ~5 minutes* ⚡
