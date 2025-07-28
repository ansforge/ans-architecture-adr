---
parent: Decisions
nav_order: 0001
title: 0001-Convergence-des-CMS-publics-esante-et-Portail-Industriel
---

# Convergence des CMS publics esanté.gouv.fr et Portail Industriel

* **statut**: "accepté"
* **date**: "2025-06-26"
* **périmètre**: "Agence"
* **décisionnaires**: "Equipe Portail"
* **consultés**: "Camelia F., Jean-francois B., Céline B., Vanina B., Isabelle B., Christian C., Michael F., Hervé G., Nils G., Fatima E., Laurent J., Jean-Baptiste L., Stéphanie L., David P., Christophe P., Coraline P., Alexandre S., Olivier J."
* **informés**: "Toutes les parties prenantes des projets esante.gouv.fr et Portail Industriel"

---

## Contexte et énoncé du problème

L'Agence du Numérique en Santé (ANS) opère deux portails web publics majeurs sur des plateformes techniques distinctes : `esante.gouv.fr` (site institutionnel) et le `Portail des Industriels (PI)` (site pour les partenaires industriels avec un espace authentifié).

Cette architecture duale génère des problèmes de fond :
* **Confusion et manque de cohérence éditoriale** (doublons de contenus).
* **Maintenabilité technique et efficacité financière à optimiser** (deux CMS Drupal distincts à maintenir).
* **Gouvernance complexe**.

Suite à une décision du CODIR en date du 25 novembre 2024, la fusion des contenus publics sur un unique CMS Drupal a été actée. La question technique à résoudre est donc la suivante : **Quel CMS Drupal retenir pour la fusion des contenus publics : celui d’e-santé, celui du portail industriel ou une nouvelle solution ?**

## Facteurs de décision

* **Continuité fonctionnelle** : La préservation des fonctionnalités existantes, notamment l'espace authentifié des industriels, est une priorité.
* **Coûts et risques** : La solution doit minimiser les coûts de développement, les délais de mise en œuvre et les risques de régressions.
* **Charge de migration** : L'effort et la complexité de la migration des contenus et des fonctionnalités doivent être maîtrisés.
* **Maintenabilité et dette technique** : La solution cible doit être basée sur un socle technique stable, à jour et avec une dette technique limitée.
* **Expérience administrateur et SEO** : La nouvelle plateforme doit offrir une bonne expérience d'administration et préserver le capital SEO existant.

## Options considérées

* **Scénario 1 : Migration du PI vers esanté** (Conserver le CMS d'esante.gouv.fr)
* **Scénario 2 : Migration de esanté vers PI** (Conserver le CMS du Portail Industriel)
* **Scénario 3 : Nouvelle solution Drupal "as a service"** (Option écartée car jugée trop coûteuse et longue à mettre en œuvre)
* **Scénario 4 : Convergence progressive** (Option écartée car jugée trop coûteuse et complexe à mettre en œuvre)

## Avantages et inconvénients des options

### Scénario 1 : Migration du PI vers esanté

* **Positive, car** le socle technique (Drupal 10.4.5) est stable, à jour et avec une faible dette technique.
* **Positive, car** le SEO, l'accessibilité et le multilingue sont déjà optimisés sur cette plateforme.
* **Négative, car** l'absence d'espace authentifié obligerait à une reconstruction complète et coûteuse des modules du PI.
* **Négative, car** la migration des contenus et des fonctionnalités du PI serait complexe et risquée.
* **Négative, car** les coûts et les risques de régression sont jugés élevés.

### Scénario 2 : Migration de esanté vers PI

* **Positive, car** l'espace authentifié et les modules personnalisés (GLPI, GED) sont déjà opérationnels.
* **Positive, car** il y a beaucoup moins de développements nécessaires et aucune régression fonctionnelle attendue sur le périmètre PI.
* **Positive, car** l'expérience d'administration est jugée plus avancée.
* **Négative, car** le socle Drupal est hors support et requiert une mise à jour (action déjà en cours).
* **Négative, car** une dette technique doit être corrigée (erreurs mais avec correction automatique possible).
* **Négative, car** le SEO et le multilingue sont à configurer pour le périmètre esanté.

## Résultat de la décision

Option choisie : **"Scénario 2 : Migration de esanté vers PI"**, parce que cette option est jugée plus réaliste et sécurisée à court terme. Elle ressort comme la meilleure solution (score de **109 points** contre 91 pour le scénario 1), présentant moins de développements, une meilleure continuité fonctionnelle et un meilleur équilibre coûts/délais.

### Conséquences

* **Positive, car** elle assure la continuité de service de l'espace authentifié industriel qui est déjà fonctionnel et intégré avec des outils tiers (GED, GLPI).
* **Positive, car** elle nécessite moins de développements ce qui réduit les coûts et les délais du projet.
* **Positive, car** le risque de régression fonctionnelle est quasi nul sur le périmètre industriel, le plus complexe.
* **Négative, car** une dette technique a été identifiée sur le socle du PI (version de Drupal à mettre à jour, erreurs à corriger).
* **Négative, car** un travail spécifique est à prévoir pour optimiser le SEO (plan de redirection pour les URL d'esanté) et configurer le multilingue.

### Confirmation

La conformité de la mise en œuvre de cette décision sera validée par :
* Un audit de sécurité réalisé après la migration.
* Le suivi des indicateurs SEO suite à la mise en place d'un plan de redirection complet.
* La réalisation de tests de non-régression fonctionnelle sur l'ensemble des périmètres.
* Le chiffrage final des travaux par le prestataire Klee et sa validation en comité de pilotage.

## Informations supplémentaires

Cette décision s'applique à la fusion des contenus **publics** des deux portails. L'espace authentifié industriel existant n'est pas modifié dans son fonctionnement. 
