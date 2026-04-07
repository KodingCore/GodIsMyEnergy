# 📘 Comportement Architectural

***

***

## I - Identification

* **Facette**: PRDCT
* **Sujet**: FILES
* **Nom**: Comportement Architectural
* **Nom du fichier**: `PRDCT_ComportementArchitectural.md`
* **Rôle**: Définit l’arborescence type du projet et le comportement de génération (0/1/2) de chaque dossier et fichier.

***

***

## II - Champs d'Application

* Génération d’un nouveau projet
* Modification de l’arborescence du projet
* Ajout ou suppression d’un fichier ou dossier
* Décision entre génération automatique et génération par l’IA

***

***

## III - Données

### 1. Règles de comportement

* **0** → Créé automatiquement par le programme
* **1** → Généré par l’IA uniquement à la première génération
* **2** → Généré par l’IA à chaque modification du document

### 2. Arborescence type du projet

```text
${AppName}/                                       0
├── Src/                                          0
│   ├── Program.cs                                1
│   ├── MainForm.cs                               2
│   ├── ${AppName}.csproj                         1
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

### 3. Cas Particuliers

* Les dossiers marqués 0 sont créés automatiquement par le programme avant de placer les fichiers dedans.
* Les fichiers dans Logs/, Bin/ et Obj/ sont créés dynamiquement par l’application à l’exécution.

### 4. Erreurs Bloquantes

* Utiliser un chiffre autre que 0, 1 ou 2
* Mettre un fichier en 2 alors qu’il ne sera jamais modifié manuellement
* Oublier de mettre le dossier parent en 0 quand ses fichiers sont en 1 ou 2

### 5. Contrôles Qualité

* Tous les dossiers parents des fichiers générés sont-ils bien en 0 ?
* Les comportements 1 et 2 sont-ils cohérents avec la fréquence de modification attendue ?
* L’arborescence est-elle complète et sans doublon ?

*(Comportement Architectural)*,
