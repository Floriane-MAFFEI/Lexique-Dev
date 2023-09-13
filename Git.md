# Guide des commandes de base de Git

---

<h2 align="center">GIT</h2>

---

![Git Cheatsheet](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d8/Git_operations.svg/1024px-Git_operations.svg.png)

---

### Configuration

---

#### git config --global user.name "nom"

Définit le nom à associer à toutes les opérations de commit

---

#### git config --global user.email "adresseMail"

Définit l'adresse mail à associer à toutes les opérations de commit

---

#### git config --global color.ui auto

Active la colorisation de la sortie de ligne de commande

---

### Créer des dépôts

---


#### git init

Crée un dépôt

--- 

#### git clone

Clone un dépot GitHub existant

---

### Effectuer des modifications

--- 

#### git add

Ajoute le changement dans le répertoire de travail.

Informe Git que l'on souhaite unclure les mises à jour dans un fichier particulier.

**Attention** : Les changements ne seront pris en compte que lors du ```git commit```

---

#### git commit -m "message descriptif"

Enregistre les fichiers ajouté via ```git add``` de façon permanente dans l'historique des versions (dépôt)

---

### Grouper des changements

---

#### git branch

Gestion des branches

---

#### git merge

Fusionne une branche dans une autre

---

#### git checkout

Annule les modifications effectuées.
Déplace sur une référence (branche, hash)

---

### Vérification de l'historique des versions

---

#### git log

Affiche la liste des commits effectués sur une branche

---

### Synchroniser des changements

---

#### git push

Publie les nouvelles révisions sur le *Remote*

---

### Enregistrements des changements non finis

---

#### git stash

Stocke de côté un état non commité afin d'effectuer d'autres tâches

