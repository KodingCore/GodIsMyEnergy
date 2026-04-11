# 📘 MultiAgentPipeline

***

***

## I - Identification

* **Facette**: PRDCT
* **Nom**: MultiAgentPipeline
* **Nom du fichier**: `PRDCT_MultiAgentPipeline.md`
* **Rôle**: Définit le pipeline complet d’agents intelligents pour la génération de projets avec boucle rétroactive.

***

***

## II - Champs d'Application

Ce document DOIT être lu avant toute génération impliquant plusieurs agents (nouvelle fonctionnalité).

***

***

## III - Données

### 1. Structure du Pipeline (7 étapes)

1. **Agent Reformulation**
   Reformule la demande utilisateur en langage clair et précis.

2. **Agent Amélioration Causale**
   Applique les règles de préférences du projet et pose un petit questionnaire très efficace (3 à 5 questions maximum) pour clarifier le contexte.

3. **Agent Génération**
   Génère les fichiers selon PRDCT_Generator.md et les modèles PRLVR (net8.0-windows).

4. **Agent Tests & Contrôles**
   Exécute :
   * Contrôle des FILEID
   * Validation des formats de commentaires et logs
   * Tests de compilation (`dotnet build`)
   * Tests de debug et SingleInstance/RunAsAdmin
   * Programmation pure et optimisation

5. **Boucle Rétroactive**
   En cas d’erreur ou de non-conformité → retour immédiat vers l’agent précédent concerné.

6. **Agent Évaluation Finale**
   Note sur 50 points (voir PRDCT_AgentEvaluation.md).

7. **Décision Finale**
   Si note ≥ 40 → livraison finale.
   Si note < 40 → retour à l’Agent Amélioration Causale pour nouvelle session de réflexion avant recodage.

***

### 2. Règles de fonctionnement

* Chaque agent travaille de manière séquentielle et autonome.
* La boucle rétroactive est obligatoire dès qu’un contrôle échoue.
* Le pipeline est piloté par l’IA génératrice (Sérènna en mode multi-agents).

*(MultiAgentPipeline)*,
