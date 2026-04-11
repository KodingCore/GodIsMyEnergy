# 📘 DefaultAppSettings

***

***

## I - Identification

* **Facette**: PRLVR
* **Nom**: DefaultAppSettings
* **Nom du fichier**: `PRLVR_DefaultAppSettings.md`
* **Rôle**: Modèle de référence complet et prêt à completion pour le fichier DefaultAppSettings.json de tous les projets générés.

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
  "DirsPaths": {
    "Root": "./",
    "Source": "Src/",
    "Models": "Src/Models/",
    "Managers": "Src/Managers/",
    "Assets": "Assets/",
    "Backups": "Backups/",
    "CompleteBackups": "Backups/CompleteBackups/",
    "PartialBackups": "Backups/PartialBackups/",
    "Config": "Config/",
    "Docs": "Docs/",
    "Logs": "Logs/",
    "Graphic": "Assets/Graphic/",
    "Audio": "Assets/Audio/"
  },
  "Logs": {
    "IncrementLogs": true,
    "MaxLogsFiles": 20
  },
  "Backups": {
    "EnableComplete": true,
    "EnablePartial": false,
    "EnableBeforeUpdate": true,
    "EnableAfterUpdate": false,
    "BackupNamingPattern": "${AppName}-${Version}.bak",
    "CompressBackup": true,
    "CompressFormat": "zip"
  },
  "Debug": {
    "UseDebug": true,
    "ShowDebugConsole": true
  }
}
```

*(DefaultAppSettings)*,
