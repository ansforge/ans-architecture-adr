---
parent: decisions
nav_order: 0
---
# Utiliser les rapports de décisions architecturales en markdown

## Contexte et énoncé du problème

Nous voulons enregistrer les décisions architecturales de l'ANS indépendamment de savoir si les décisions concernent l'architecture ("rapport de décision architecturale"), le code ou d'autres domaines.
Quel format et quelle structure ces enregistrements devraient-ils suivre ?

## Options Envisagées

* [MADR](https://adr.github.io/madr/) 4.0.0 – Les Records de Décisions Architecturales Markdown
* [Modèle de Michael Nygard](http://thinkrelevance.com/blog/2011/11/15/documenting-architecture-decisions) – La première incarnation du terme "ADR"
* [Décisions Architecturales Durables](https://www.infoq.com/articles/sustainable-architectural-design-decisions) – Les Déclarations Y
* Autres modèles listés à <https://github.com/joelparkerhenderson/architecture_decision_record>
* Forme libre – Aucune convention pour le format et la structure des fichiers

## Résultat de la Décision

Option choisie : "MADR 4.0.0", car

* Les hypothèses implicites doivent être rendues explicites.
  La documentation de conception est important pour permettre aux personnes de comprendre les décisions plus tard.
  Voir également ["Un processus de conception rationnel : Comment et pourquoi le simuler"](https://doi.org/10.1109/TSE.1986.6312940).
* MADR permet de capturer de manière structurée toute décision.
* Le format MADR est concis et s'adapte à notre style de développement.
* La structure MADR est compréhensible et facilite l'utilisation et la maintenance.
* Le projet MADR est actif.
