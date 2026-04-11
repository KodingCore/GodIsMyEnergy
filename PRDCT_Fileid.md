# 📘 Fileid

***

***

## I - Identification

* **Facette**: PRDCT
* **Nom**: Fileid
* **Nom du fichier**: `PRDCT_Fileid.md`
* **Rôle**: Définir de façon stricte le format, le placement et les règles de contrôle du FILEID dans tous les fichiers générés.

***

***

## II - Champs d'Application

* Génération de tout nouveau fichier (quel que soit son type)
* Création ou modification d’un modèle de prélivraison
* Contrôle qualité sur un fichier généré
* Correction d’un FILEID mal formé

***

***

## III - Données

### 1. Règles générales

* Format : `FILEID=AppName/SousDossier/Fichier.Extension`
* Chemin relatif POSIX (séparateur `/`)
* Dossiers et fichiers en PascalCase
* Extension en minuscules

### 2. Placement selon le type de fichier

#### CSharp (.cs)

Ligne 1 :

```cs
// FILEID=AppName/SousDossier/Fichier.cs
```

#### C# Project (.csproj)

Ligne 1:

```cshtml
<!-- FILEID=AppName/SousDossier/Fichier.csproj -->
```

#### JSON (.json)

Première propriété de l’objet racine:

```json
"FILEID":"AppName/SousDossier/Fichier.json"
```

#### Markdown (.md)

Ligne 1:

```markdown
FILEID=AppName/SousDossier/Fichier.md
```

#### Solution Visual Studio (.sln)

Ligne 1:

```solution-file
# FILEID=AppName/SousDossier/Fichier.sln
```

#### Gitignore (.gitignore)

Ligne 1:

```python
# FILEID=AppName/.gitignore
```

#### Python (.py)

Ligne 1 pour l'environnement (optionnel):

```python
#! python3
```

Ligne 2 pour l'encodage (OBLIGATOIRE):

```python
# -*- coding: utf-8 -*-
```

Ligne 3:

```python
# FILEID=AppName/SousDossier/Fichier.py
```

#### INI (.ini)

Ligne 1:

```ini
; FILEID=AppName/SousDossier/Fichier.ini
```

#### TXT (.txt)

Ligne 1:

```text
FILEID=AppName/SousDossier/Fichier.txt
```

#### PowerShell (.ps1)

Ligne 1 pour l'élévation de privilèges (optionnel):

```powershell
#Requires -RunAsAdministrator
```

Ligne 2:

```powershell
# FILEID=AppName/SousDossier/Fichier.ps1
```

#### Visual Basic for Applications (.vba, .bas, .cls)

Ligne 1:

```vba
' FILEID=AppName/SousDossier/Fichier.bas
```

#### XML & App Manifest (.xml, .manifest)

Ligne 1 pour la déclaration XML (OBLIGATOIRE):

```xml
<?xml version="1.0" encoding="utf-8"?>
```

Ligne 2:

```xml
<!-- FILEID=AppName/SousDossier/Fichier.xml -->
```

#### YAML (.yml / .yaml)

Ligne 1:

```yaml
# FILEID=AppName/SousDossier/Fichier.yaml
```

#### Shell (.sh)

Ligne 1 pour le Shebang (optionnel):

```bash
#!/bin/bash
```

Ligne 2:

```bash
# FILEID=AppName/SousDossier/Fichier.sh
```

#### Batch (.bat)

Ligne 1:

```dos
REM FILEID=AppName/SousDossier/Fichier.bat
```

#### HTML (.html)

Ligne 1:

```html
<!DOCTYPE html>
```

Ligne 2:

```html
<!-- FILEID=AppName/SousDossier/Fichier.html -->
```

#### CSS & SCSS (.css, .scss)

Ligne 1:

```css
@charset "UTF-8";
```

Ligne 2:

```css
/* FILEID=AppName/SousDossier/Fichier.css */
```

#### JavaScript (.js)

Ligne 1 :

```JavaScript
// FILEID=AppName/SousDossier/Fichier.js
```

### 3. Cas Particuliers

* Le FILEID doit toujours être sur la **première ligne utile**
* Le chemin doit rester **strictement relatif** à la racine du projet
* Aucun FILEID ne doit être présent dans les fichiers PRLVR

### 4. Erreurs Bloquantes

* Absence de FILEID
* Chemin absolu ou utilisation de `..`
* Double slash `//`
* Absence d’extension
* FILEID mal placé (surtout en Python)

### 5. Contrôles Qualité

* Chaque format utilise-t-il son placement canonique ?
* Les chemins sont-ils relatifs, complets et sans espace ?
* L’ordre Python (encodage puis FILEID) est-il respecté ?

*(Fileid)*,
