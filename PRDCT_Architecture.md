# 📘 Architecture

***

***

## I - Identification

* **Facette**: PRDCT
* **Nom**: Architecture
* **Nom du fichier**: `PRDCT_Architecture.md`
* **Rôle**: Définit l’arborescence canonique de référence du projet et précise le mode de génération des dossiers et fichiers.

***

***

## II - Champs d'Application

Ce document **DOIT** être lu avant toute génération de projet pour garantir la cohérence de l’arborescence.

***

***

## III - Données

### 1. Règles de comportement

* **0** → Création de dossier gérée exclusivement par le programme tiers (via parsing des FILEID).
* **1** → Fichier généré par l’IA uniquement à la première génération.
* **2** → Fichier généré par l’IA à chaque modification du document.

***

### 2. Arborescence canonique de référence

```text
${AppName}/                                       0
├── Src/                                          0
│   ├── Program.cs                                1
│   ├── MainForm.cs                               2
│   ├── ${AppName}.csproj                         1
│   ├── app.manifest                              1
│   ├── Managers/                                 0
│   │   ├── ConfigManager.cs                      1
│   │   ├── LogsManager.cs                        1
│   │   └── SingleInstanceManager.cs              1
│   └── Models/                                   0
├── Assets/                                       0
│   ├── Graphic/                                  0
│   ├── Audio/                                    0
│   └── AppIcon.ico                               1
├── Backups/                                      0
│   ├── CompleteBackups/                          0
│   └── PartialBackups/                           0
├── Config/                                       0
│   ├── DefaultAppSettings.json                   1
│   └── UserSettings.json                         2
├── Docs/                                         0
│   ├── CHANGELOG.md                              2
│   ├── RELEASE_NOTES.md                          2
│   └── VERSIONING_GUIDE.md                       1
├── Logs/                                         0
│   ├── App.log                                   0
│   ├── Errors.log                                0
│   └── Debug.log                                 0
├── Bin/                                          0
├── Obj/                                          0
├── .gitignore                                    1
├── ${AppName}.sln                                1
└── README.md                                     2
```

***

### 3. Principe de génération des dossiers

* Les dossiers marqués 0 sont créés automatiquement par le programme avant de placer les fichiers dedans.
* Les fichiers dans Logs/, Bin/ et Obj/ sont créés dynamiquement par l’application à l’exécution.

Soit, le programme tiers analyse chaque FILEID reçu, extrait le chemin relatif et crée récursivement l’arborescence nécessaire. Aucune action de création de dossier n’est effectuée par le code C# généré ni par l’IA.

***

### 4. Cadre technique

* Framework cible : net9.0-windows
* Compilation : dotnet build (CLI)
* Dépendances : Détection et installations automatique par le programme qui accueil les fichiers générés

*(Architecture)*,
