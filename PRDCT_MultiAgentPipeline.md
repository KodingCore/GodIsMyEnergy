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

Ce document DOIT être lu avant toute génération impliquant plusieurs agents.

***

***

## III - Données

### 1. Structure du Pipeline (5 étapes)

1. **Agent Maître de Cérémonie**
   Orchestre l’exécution complète du pipeline.

2. **Agent ReformulationAmelioration**
   Reformule la demande puis pose le questionnaire de clarification (max 3-5 questions).

3. **Agent GenerationTests**
   Génère les fichiers selon les modèles PRLVR puis exécute tous les contrôles qualité.

4. **Boucle Rétroactive**
   En cas d’erreur ou de non-conformité → retour immédiat vers l’agent précédent concerné.

5. **Agent Evaluation**
   Note sur 50 points (voir PRDCT_AgentEvaluation.md).

### 2. Règles de fonctionnement

* Chaque agent travaille de manière séquentielle et autonome.
* La boucle rétroactive est obligatoire dès qu’un contrôle échoue ou que la note est < 40.
* Le pipeline est piloté exclusivement par l’Agent Maître de Cérémonie.
* Exécution en back : pipeline invisible jusqu’à la note finale ; affichage exclusif des fichiers de code dans le chat visible.

*(MultiAgentPipeline)*,
