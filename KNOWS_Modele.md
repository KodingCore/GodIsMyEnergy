# 📘 Modele

***

***

## I - Identification

* **Facette**: KNOWS
* **Nom**: Modele
* **Nom du fichier**: `KNOWS_Modele.md`
* **Rôle**: Modèle officiel de référence à copier-coller pour créer ou modifier tout document de Base de Connaissances.

***

***

## II - Champs d'Application

* Création d’un nouveau document KNOWS
* Renommage, restructuration ou mise à jour d’un document KNOWS existant
* Garantie de cohérence visuelle et structurelle

***

***

## III - Données

### 1. Règles de nommage des fichiers

* Format obligatoire : `FACETTE_NomDuDocument.md`

### 2. Exemples de noms actuels

* `KNOWS_Empreintes.md`
* `KNOWS_Glossaire.md`
* `KNOWS_Identification.md`
* `KNOWS_Sommaire.md`
* `KNOWS_Index.md`
* `KNOWS_Modele.md`
* `PRDCT_Fileid.md`
* `PRDCT_ComportementArchitectural.md`
* `PRDCT_Completion.md`
* `ARMTR_Readme.md`

### 3. Règles du titre H1 selon la facette

Le H1 de tout les documents est nommé par le **Nom** de leur section `I - Identification`

### 4. Structure obligatoire du document

Le squelette suivant doit toujours être respecté :

```markdown
# 📘 Titre du document

***

***

## I - Identification

* **Facette**: ...
* **Nom**: ...
* **Nom du fichier**: ...
* **Rôle**: ...

***

***

## II - Champs d'Application

Ce document **DOIT** être consulté à chaque fois que :

* Point 1
* Point 2
* Point 3

***

***

## III - Données

### 1. Titre de la section

Contenu...

***

*(NomCourt)*,

```

### 5. Règles de formatage strictes

* Tous les items de liste doivent commencer par *
* Après "Ce document DOIT être consulté à chaque fois que :", une ligne vide obligatoire
* À la fin du fichier : la conclusion suivie d’une virgule , puis une ligne vide

### 6. Contrôles Qualité

* Le nom du fichier respecte-t-il le format FACETTE_NomDuDocument.md ?
* La section Identification contient-elle bien les cinq champs ?
* Le titre H1 respecte-t-il la règle de sa facette ?

*(Modele)*,
