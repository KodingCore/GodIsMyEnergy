# 📘 Project

***

***

## I - Identification

* **Facette**: PRLVR
* **Nom**: Project
* **Nom du fichier**: `PRLVR_Project.md`
* **Rôle**: Modèle de référence complet et prêt à completion pour le fichier Project.csproj de tous les projets générés.

***

***

```xml
<!-- FILEID=${AppName}/Src/${AppName}.csproj -->
<Project Sdk="Microsoft.NET.Sdk">

  <PropertyGroup>
    <OutputType>WinExe</OutputType>
    <TargetFramework>net8.0-windows</TargetFramework>
    <Nullable>enable</Nullable>
    <UseWindowsForms>true</UseWindowsForms>
    <ApplicationManifest>app.manifest</ApplicationManifest>
    <RootNamespace>${AppName}</RootNamespace>
    <AssemblyName>${AppName}</AssemblyName>
  </PropertyGroup>

  <ItemGroup>
    <!-- Références internes uniquement - aucune dépendance tierce externe -->
  </ItemGroup>

</Project>
```

*(Project)*,
