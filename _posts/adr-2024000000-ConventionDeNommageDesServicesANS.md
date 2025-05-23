---
title: Décision des conventions de nommage des urls
date: 2022-05-05 22:18:00 +0100
categories: [URL, Nommage]
tags: [URL, nommage]
---

<!-- # Ce sont des éléments de métadonnées optionnels. Vous pouvez les supprimer si vous le souhaitez.
status : "{proposé | rejeté | accepté | obsolète | … | remplacé par ADR-0123}"
date : {AAAA-MM-JJ, date de la dernière mise à jour de la décision}
décisionnaires : {liste de toutes les personnes impliquées dans la prise de décision}
consultés : {liste des personnes dont les opinions sont sollicitées (généralement des experts en la matière) et avec lesquelles il y a une communication bidirectionnelle}
informés : {liste des personnes tenues au courant des progrès, avec lesquelles la communication est unidirectionnelle}
-->
status : "{proposé}"
date : {2024-12-10, création}
décisionnaires : {Laurent JOUBERT, Hervé GARREAU}
consultés : {Cedric PANNISSOD, Alexandre SALZMANN, Christian CRIMETZ, Laurent DUMONTIER, Alban MAREAU}
informés : {liste des personnes tenues au courant des progrès, avec lesquelles la communication est unidirectionnelle}

---

# {convention de nommage des urls des applications et services de l'ANS}

## Contexte et Énoncé du Problème

{Adopter une convention de nommage des URL et services de l'ANS de sorte que soit explicite et cohérente. L'objectif est d'uniformiser les moyens d’accéder à ces services par nos partenaires.}

<!-- Cet élément est optionnel. Vous pouvez le supprimer si vous le souhaitez. -->

## Options Considérées

* {[appli/outil/service].[environnement].esante.gouv.fr} 
    * appli/outil/service : nom fourni par les programmes pour leur service applicatif
        * Le référentiel des appli/outil/service pourra faire l’objet d’un document spécifique (à arbitrer). Il contiendra pour chaque          	appli/outil/service ouvert aux partenaires sa description et son identifiant (exemple :finess, ror, 	hub-sante, …)
    * Environnement : liste des environnements accessibles aux partenaires
        * Les environnements concernés sont : 
            * bac à sable (bac-a-sable) pour les tests d’interconnexion avec les partenaires
                * exemple : ror.bac-a-sable.esante.gouv.fr
            * Formation (formation) pour la formation aux outils
                * exemple : ror.formation.esante.gouv.fr
            * Production () pour les services mis à disposition en production le nom de l'environnement n'apparait pas
                * exemple ror.esante.gouv.fr
        

* {titre de l'option 2}
* {titre de l'option 3}
* … <!-- le nombre d'options peut varier -->

## Résultat de la Décision

Option choisie : "{titre de l'option 1}", parce que {justification, par exemple : seule option répondant au critère déterminant | qui résout la force {force} | … | qui ressort comme la meilleure (voir ci-dessous)}.

<!-- Cet élément est optionnel. Vous pouvez le supprimer si vous le souhaitez. -->
### Conséquences

* Positive, car {conséquence positive, par exemple amélioration d'une ou plusieurs qualités désirées, …}
* Négative, car {conséquence négative, par exemple compromis sur une ou plusieurs qualités désirées, …}
* … <!-- le nombre de conséquences peut varier -->

<!-- Cet élément est optionnel. Vous pouvez le supprimer si vous le souhaitez. -->
### Confirmation

{Décrivez comment la mise en œuvre / la conformité de l'ADR peut/sera confirmée. Existe-t-il une fonction automatisée ou manuelle pour cela ? Si oui, listez-la et expliquez comment elle est appliquée. La conception choisie et sa mise en œuvre sont-elles conformes à la décision ? Par exemple, une revue de conception/code ou un test avec une bibliothèque comme ArchUnit peut aider à valider cela. Notez que bien que nous classions cet élément comme optionnel, il est inclus dans de nombreux ADR.}

<!-- Cet élément est optionnel. Vous pouvez le supprimer si vous le souhaitez. -->
## Avantages et Inconvénients des Options

### {titre de l'option 1}

<!-- Cet élément est optionnel. Vous pouvez le supprimer si vous le souhaitez. -->
{exemple | description | lien vers plus d'informations | …}

* Positive, car {argument a}
* Positive, car {argument b}
<!-- utilisez "neutre" si l'argument n'est ni positif ni négatif -->
* Neutre, car {argument c}
* Négative, car {argument d}
* … <!-- le nombre d'avantages et d'inconvénients peut varier -->

### {titre de l'autre option}

{exemple | description | lien vers plus d'informations | …}

* Positive, car {argument a}
* Positive, car {argument b}
* Neutre, car {argument c}
* Négative, car {argument d}
* …

<!-- Cet élément est optionnel. Vous pouvez le supprimer si vous le souhaitez. -->
## Informations Supplémentaires

{Vous pouvez fournir ici des éléments de preuve ou de confiance supplémentaires concernant le résultat de la décision, documenter l'accord de l'équipe sur la décision et/ou définir quand/comment cette décision doit être mise en œuvre et si/quand elle doit être révisée. Des liens vers d'autres décisions et ressources peuvent également apparaître ici.} 

---