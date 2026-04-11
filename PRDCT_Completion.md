# 📘 Completion

***

***

## I - Identification

* **Facette**: PRDCT
* **Nom**: Completion
* **Nom du fichier**: `PRDCT_Completion.md`
* **Rôle**: Répertorier toutes les holdplaces utilisées dans les fichiers de prélivraison et préciser la valeur qui **DOIT** les remplacer lors de la génération.

***

***

## II - Champs d'Application

* Génération d’un fichier à partir d’un modèle PRLVR
* Ajout, modification ou suppression d’une holdplace dans un modèle PRLVR
* Création d’un nouveau modèle de prélivraison

***

***

## III - Données

### 1. Liste des Holdplaces

* **${AppName}**     : Nom technique du projet en PascalCase
* **${UsualName}**   : Nom usuel / commercial du projet
* **${Acronym}**     : Acronyme du projet (3 à 5 lettres)
* **${Version}**     : Version actuelle au format SemVer
* **${Description}** : Description détaillée du projet
* **${Settings}**    : Liste des paramètres et options importantes
* **${Goal}**        : Objectif principal du projet
* **${Sequencies}**  : Ordre d’utilisation recommandé
* **${Variations}**  : Variantes fonctionnelles du projet
* **${Installs}**    : Prérequis et étapes d’installation
* **${Interface}**   : Description des éléments interactifs de l’interface
* **${Structure}**   : Arborescence complète du projet en ASCII
* **${Commentaries}** : Notes et commentaires divers

### 2. Cas Particuliers

* Les holdplaces doivent être utilisées **EXACTEMENT** avec les mêmes noms et la même casse.
* `${AppName}` et `${UsualName}` ne doivent jamais être inversés.
* Les listes (`${Settings}`, `${Goal}`, `${Sequencies}`, etc.) doivent être formatées en Markdown.

### 3. Erreurs Bloquantes

* Utiliser `${ProjectName}` au lieu de `${AppName}`
* Oublier une holdplace présente dans un fichier PRLVR
* Utiliser une holdplace qui n’est pas listée dans ce document
* Laisser une holdplace non remplacée dans un fichier livré

### 4. Contrôles Qualité

* Toutes les holdplaces présentes dans les fichiers PRLVR sont-elles listées ici ?
* Chaque holdplace a-t-elle une description claire et sans ambiguïté ?
* Les noms des variables respectent-ils exactement la casse définie ?

*(Completion)*,
