# 📘 Modèle Markdown

***

***

## I - Identification

* **Facette**: KNOWS
* **Sujet**: FILES
* **Nom**: Modèle Markdown
* **Nom du fichier**: `KNOWS_Modele.md`
* **Rôle**: Modèle officiel de référence à copier-coller pour créer ou modifier tout document de la Base de Connaissances.

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
* Le **Sujet** n’est plus inclus dans le nom du fichier (simplification)

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

* **KNOWS** → **Nom** des **Sujet** de la Base de Connaissances  
  Exemple : `# 📘 Empreintes`
* **PRDCT** → **Nom** des **Sujet** de Production  
  Exemple : `# 📘 Fileid`
* **ARMTR** → **Sujet** - Armature de **Nom**  
  Exemple : `# 📘 Readme`

### 4. Structure obligatoire du document

Le squelette suivant doit toujours être respecté :

```markdown
# 📘 Titre du document

***

***

## I - Identification
* **Facette**: ...
* **Sujet**: ...
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
* À la fin du fichier : une ligne vide, puis la conclusion suivie d’une virgule ,

### 6. Contrôles Qualité

* Le nom du fichier respecte-t-il le format FACETTE_NomDuDocument.md ?
* La section Identification contient-elle bien les cinq champs ?
* Le titre H1 respecte-t-il la règle de sa facette ?

*(Modèle Markdown)*,
