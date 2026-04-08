# 📘 DefaultAppSettings

***

***

## I - Identification

* **Facette**: PRLVR
* **Sujet**: PARAM
* **Nom**: DefaultAppSettings
* **Nom du fichier**: `PRLVR_DefaultAppSettings.md`
* **Rôle**: Modèle JSON de configuration par défaut (prêt à completion).

***

***

```json
{
  "FILEID": "${AppName}/Config/DefaultAppSettings.json",
  "Metadata": {
    "Project": "${UsualName}",
    "GeneratedBy": "ConfigManager.cs"
  },
  "Author": {
    "Society": "LightWay Project",
    "AuthorName": "Lelievre Mike",
    "AuthorEmail": "kcorvais@gmail.com",
    "AuthorWebsite": "https://lightway-project.com"
  },
  "Identity": {
    "AppName": "${AppName}",
    "AppUsualName": "${UsualName}",
    "AppAcronym": "${Acronym}",
    "AppVersion": "${Version}",
    "AppBarTitle": "LightWay Project - ${AppName}"
  },
  "System": {
    "DateFormat": "DD/MM HH:mm",
    "DatetimeZone": "Europe/Paris",
    "Locale": "fr-FR",
    "FilesEncoding": "UTF-8",
    "VersionFormat": "SemVer"
  },
  "Runtime": {
    "UseImages": true,
    "IsDaemon": false,
    "RunAsAdmin": true,
    "KeepOldFiles": false,
    "SingleInstance": true
  },
  "DirsPaths": { ... }   // (le reste du JSON reste identique)
}
```

*(DefaultAppSettings)*,