# 📘 AgentEvaluation

***

***

## I - Identification

* **Facette**: PRDCT
* **Nom**: AgentEvaluation
* **Nom du fichier**: `PRDCT_AgentEvaluation.md`
* **Rôle**: Grille de notation finale sur 50 points avec seuil de boucle rétroactive.

***

***

## II - Champs d'Application

Ce document DOIT être appliqué à la fin de chaque génération avant livraison.

***

***

## III - Données

### 1. Grille de notation (sur 50 points)

* **10 points – UI** : Design visuel, modernité, clarté des contrôles Windows Forms.
* **10 points – UX** : Fluidité, intuitivité, feedback utilisateur.
* **10 points – Simplicité / Complétude liée au but initial** : Rapport parfait entre minimalisme et couverture des besoins exprimés.
* **10 points – Propreté des fichiers et du projet** : CODE propre, commenté, logs structurés, FILEID corrects, architecture respectée.
* **10 points – Aspects particuliers au projet** : Performance, sécurité, SingleInstance, RunAsAdmin, backups, etc.

***

### 2. Règles de décision

* Note totale **≥ 40** → Projet validé et livré.
* Note totale **< 40** → Retour immédiat à l’Agent Amélioration Causale + nouvelle session de réflexion avant recodage complet.

***

### 3. Format de rendu de l’évaluation

L’IA doit afficher clairement :
« Évaluation finale : XX/50 »
+ détail des 5 critères
+ Décision (Validé ou Boucle rétroactive).

*(AgentEvaluation)*,
