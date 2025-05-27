---
parent: Decisions
nav_order: 0001
title: Choix du modèle pour la rédaction des ADR

---

# Choix du modèle pour la rédaction des ADR

* statut : proposé
* date : 2025-05-27
* décisionnaires : CTO
* consultés : CTO
* informés : équipe intégration, directeurs de domaine

---

# Formalisme des décisions d'architecture au format markdown sur Github

## Contexte et énoncé du problème

Actuellement, les décisions d'architecture sont prises de manière informelle, dispersées dans des discussions verbales, des emails, des groupes Sharepoint et des tickets Jira. Cela rend difficile le suivi des raisons derrière ces décisions, leur impact et leur révision ultérieure. L'objectif est de formaliser le processus de décision d'architecture en utilisant un modèle standardisé, stocké dans un format lisible par tous et accessible via un système de gestion de versions (Git).  Comment structurer et documenter les décisions d'architecture de manière claire, traçable et collaborative ?  

## Facteurs de Décision

* **Lisibilité et simplicité :** Le formalisme doit être facile à comprendre et à maintenir pour l'ensemble de l'équipe.
* **Traçabilité :** Il doit être facile de retrouver l'historique des décisions et leur justification.
* **Collaborativité :** Le processus doit encourager la participation de tous les membres de l'ANS.
* **Intégration à l'existant :** Le format doit s'intégrer facilement à l'écosystème Github (Markdown, pull requests).
* **Maintenabilité :** La structure doit être facile à faire évoluer au fil du temps.

## Options considérées

* **ans-architecture-adr sur Github :** Utiliser un template ADR (Architecture Decision Record) au format Markdown et stocker ces fichiers dans un repository Github.
* **Wiki Github :** Utiliser le Wiki Github pour documenter les décisions d'architecture.
* **Confluence :** Centraliser les décisions d'architecture dans un espace Confluence.
* **GED :** Utiliser la GED pour collaborer et documenter les décisions d'architecture.

## Résultat de la Décision

Option choisie : "ans-architecture-adr sur Github" parce que c'est la solution qui combine le mieux la lisibilité, la traçabilité, la collaborativité et l'intégration avec notre infrastructure existante (Github). De plus, l'utilisation du format Markdown favorise la portabilité et l'archivage à long terme.


### Conséquences
* **Positive, car** améliore la transparence et la compréhension des décisions d'architecture. Facilite l'onboarding de nouveaux membres dans l'équipe.  Augmente la traçabilité des décisions.
* **Négative, car** nécessite un certain effort initial pour adopter et maintenir la discipline des ADR. Peut impliquer une charge administrative légèrement supérieure à des méthodes plus informelles.

<!-- Cet élément est optionnel. Vous pouvez le supprimer si vous le souhaitez. -->
### Confirmation

La conformité de l'ADR sera confirmée par une revue des pull requests contenant les nouveaux ADR ou les mises à jour d'ADR existants. Un script Github Actions pourrait être mis en place pour valider la structure et le contenu des ADR (présence de certains champs obligatoires par exemple).  Une review du code affecté par la décision d'architecture sera également effectuée pour s'assurer de la conformité.

<!-- Cet élément est optionnel. Vous pouvez le supprimer si vous le souhaitez. -->
## Avantages et inconvénients des Options

### ans-architecture-adr sur Github

* Positive, car facilite la collaboration via les pull requests Github.
* Positive, car le format Markdown est simple, lisible et portable.
* Neutre, car nécessite la mise en place d'une convention de nommage et d'organisation des fichiers ADR.
* Négative, car peut nécessiter un temps d'adaptation pour des gens non techniques.

### Wiki Github

* Positive, car facile à mettre en place et à utiliser.
* Positive, car intégrée nativement à Github.
* Neutre, car moins structuré qu'un modèle ADR ce qui peut conduire à un manque de cohérence.
* Négative, car moins adapté au suivi des changements et à la traçabilité des décisions.
* Négative, car moins formel, donc moins de garantie de couverture des points importants.

### Confluence

* Positive, car permet une gestion centralisée des connaissances.
* Neutre, car nécessite une licence Confluence.
* Négative, car peut devenir un silo d'information si mal utilisé.
* Négative, car accès potentiellement limité à certaines personnes.

### GED 

* Positive, car facile à utiliser et à partager.
* Négative, car manque de traçabilité des modifications.
* Négative, car moins structuré et formel qu'un ADR.
* Négative, car peut devenir un silo d'information si mal utilisé.
* Négative, car accès potentiellement limité à certaines personnes.

<!-- Cet élément est optionnel. Vous pouvez le supprimer si vous le souhaitez. -->
## Informations Supplémentaires

La mise en œuvre de ce formalisme a débuté par la création d'un repository dédié aux ADR : https://github.com/ansforge/ans-architecture-adr

---