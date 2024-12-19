Voici une version optimisée et professionnelle de votre `README.md`, adaptée pour un projet **sans base de données** et avec sauvegarde dans un fichier texte uniquement :

---

# 🗂️ Gestion des Dossiers Apprenants

Un outil performant développé en **langage C** pour gérer les dossiers des apprenants.  
Ce projet repose sur une gestion des données en **mémoire vive** avec une option de **sauvegarde et de chargement** à partir de fichiers texte.

---

## ✨ Fonctionnalités

- **📋 Créer un dossier** : Ajoutez de nouveaux apprenants à la base.  
- **🔍 Rechercher un dossier** : Trouvez un apprenant via son nom.  
- **📊 Afficher les dossiers** : Listez tous les apprenants enregistrés.  
- **🧮 Calculer les moyennes** : Moyenne pondérée des évaluations d'un apprenant.  
- **🗑️ Supprimer un dossier** : Retirez un apprenant de la base grâce à son identifiant.  
- **💾 Sauvegarde et chargement** : Gérez la persistance des données avec un fichier texte.

---

## 🛠️ Pré-requis

- **GCC** : Pour compiler le code.  

---

## 📂 Structure du Projet

La structure des fichiers est organisée pour garantir modularité et maintenabilité :

```bash
.
├── include/              # Fichiers d'en-tête (.h)
│   ├── student.h
│   ├── utils.h
│
├── src/                  # Fichiers sources (.c)
│   ├── main.c
│   ├── student.c
│   ├── utils.c
│   ├── file_operations.c
│
├── build/                # Fichiers objets compilés (.o)
│
├── bin/                  # Fichiers exécutables
│   └── gestion_dossiers
│
├── data/                 # Sauvegarde des données
│   └── dossiers.txt      # Fichier texte pour la persistance
│
├── .gitignore            # Fichiers et dossiers ignorés par Git
├── Makefile              # Script pour automatiser la compilation
└── README.md             # Documentation du projet
```

---

## 🚀 Instructions d'Utilisation

1. **Compiler le projet** :  
   Utilisez `make` pour compiler tous les fichiers sources et générer l'exécutable :  
   ```bash
   make
   ```

2. **Exécuter le programme** :  
   Lancez l'application via l'exécutable généré :  
   ```bash
   ./bin/gestion_dossiers
   ```

3. **Nettoyer les fichiers objets** :  
   Supprimez les fichiers compilés pour garder un répertoire propre :  
   ```bash
   make clean
   ```

4. **Sauvegarder les données** :  
   À la fin d'une session, les données seront automatiquement enregistrées dans le fichier `students.txt`.

5. **Charger les données** :  
   Lors du démarrage, le programme charge automatiquement les données existantes depuis `students.txt`.

---

## 📊 Exemple d'Exécution

Voici un aperçu d'une session utilisateur :  

1. **Ajout d'un apprenant** :  
   ```
   Nom et Prénom: Mohamed Hedi Gharbi
   Âge: 22
   Note 1: 18
   Note 2: 17
   Dossier crée avec succés !
   ```

2. **Affichage des apprenants** :  
   ```
   Liste des apprenants :  
   ================================================================================
   | N° | Nom et Prénom            | Âge | Eval Num 1 | Eval Num 2 |
   ================================================================================
   | 1  | Mohamed Hedi Gharbi      | 22  | 18.00      | 17.00      |
   ================================================================================

   ```

3. **Sauvegarde automatique** :  
   ```
   students.txt :
   ==========================================================================
   | N° | Nom et Prénom            | Âge | Note Eval 1 | Note Eval 2 |
   ==========================================================================
   | 1  | Mohamed Hedi Gharbi      | 22  | 18.00       | 17.00       |
   ==========================================================================
   ```

4. **Chargement des données** :  
   ```
   Chargement des données depuis 'students.txt'...  
   Données chargées avec succès !
   ```

---

## 🌟 Points Forts

- **Simplicité** : Aucune dépendance externe. Tout est géré avec des fichiers texte.  
- **Modularité** : Le code est découpé en plusieurs modules pour une maintenabilité optimale.  
- **Persistance des données** : Les données sont conservées entre les sessions grâce au fichier `data/dossiers.txt`.  

---

## 🛡️ Licence

Ce projet est distribué sous la licence **MIT**. Consultez le fichier `LICENSE` pour plus d'informations.

---

## 🤝 Contribution

Les contributions sont les bienvenues pour améliorer ce projet ! Voici comment participer :  

1. Forkez ce dépôt.  
2. Créez une branche dédiée pour vos modifications :  
   ```bash
   git checkout -b feature/nouvelle-fonctionnalité
   ```
3. Commitez vos changements :  
   ```bash
   git commit -m "Ajout d'une nouvelle fonctionnalité"
   ```
4. Poussez vos modifications :  
   ```bash
   git push origin feature/nouvelle-fonctionnalité
   ```
5. Ouvrez une **Pull Request** et décrivez vos modifications.  

---

## 👨‍💻 Auteur

- **Mohamed Hedi Gharbi [GitHub](https://github.com/Mohamed-Hedi-Gharbi)**  
  

---

### ⭐ Si ce projet vous est utile, n'oubliez pas de laisser une étoile sur GitHub !  

--- 

