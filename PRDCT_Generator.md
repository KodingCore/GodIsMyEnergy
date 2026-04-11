# 📘 Generator

***

***

## I - Identification

* **Facette**: PRDCT
* **Nom**: Generator
* **Nom du fichier**: `PRDCT_Generator.md`
* **Rôle**: Règles officielles et complètes de l’IA génératrice de programmes à partir de la Base de Connaissances.

***

***

## II - Champs d'Application

Ce document DOIT être lu à chaque génération de projet, immédiatement après PRDCT_Architecture.md et PRDCT_Completion.md.

***

***

## III - Données

### 1. Ordre de lecture obligatoire

1. ALEPH_EntryPoint.md
2. KNOWS_Glossaire.md
3. KNOWS_Empreintes.md
4. PRDCT_Fileid.md
5. PRDCT_Architecture.md
6. PRDCT_Completion.md
7. PRDCT_Generator.md
8. PRDCT_PromptTemplate.md
9. PRLVR_Readme.md et tous les fichiers PRLVR requis.

***

### 2. Règles d’exécution (10 commandements)

1. Demander les holdplaces ; si seule `${AppName}` est fournie, déduire automatiquement :
   * `${UsualName}` = `${AppName}` avec espace avant chaque majuscule
   * `${Acronym}` = initiales majuscules
   * Autres holdplaces déduites par logique ou laissées en attente.
2. Le programme tiers gère seul tous les dossiers (comportement 0) via FILEID.
3. Générer les fichiers dans l’ordre strict 1 puis 2.
4. Insérer le FILEID canonique en première ligne utile.
5. Remplacer toutes les holdplaces sans exception.
6. Générer uniquement des solutions .NET 8.0-windows (C# 12, Windows Forms) sans dépendance tierce externe.
7. Produire directement un projet complet et un exécutable fonctionnel prêt à compiler via `dotnet build`.
8. Appliquer SingleInstance, RunAsAdmin, logs structurés.
9. Format de réponse strictement formel, professionnel et concis.
10. Toujours proposer un plan de tâches clair avant génération.
11. Exécution silencieuse du pipeline : Tout le processus multi-agents (Reformulation → Amélioration Causale → Génération → Tests & Contrôles → Évaluation) s’exécute en arrière-plan de manière invisible. Seuls les blocs de code source finaux du projet généré (avec leurs FILEID) apparaissent dans la conversation une fois la note finale attribuée et le projet validé.

***

### 3. Contrôles Qualité finaux

* Tous les FILEID corrects ?
* Aucune holdplace restante ?
* Projet compilable directement ?

*(Generator)*,
