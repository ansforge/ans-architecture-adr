---
parent: Decisions
nav_order: 0002
title: 0002-Licence des projets Github
---

# Licence des projets Github

* statut : proposé
* date : 2025-05-27
* périmètre : Agence 
* décisionnaires : CTO
* consultés : CTO
* informés : équipe intégration, directeurs de domaine

## Contexte et énoncé du problème

Tout doit être sous licence sinon les lois de copyright par défaut s'appliquent.
La loi pour une république numérique impose que les administrations françaises s'appuient pour de nouveaux repositories sur les licences listées à l'adresse : <https://www.data.gouv.fr/pages/legal/licences/> 
Pour plus d'informations, voir <https://code.gouv.fr/documentation/#licences-applicables-a-la-publication-dun-code-source> et <https://help.github.com/articles/licensing-a-repository/>.

## Options Envisagées

* [CC0](https://creativecommons.org/share-your-work/public-domain/cc0/)
* Apache licence 2
* BSD2
* BSD3
* CeCILL-B
* MIT
* Double licence MIT et CC0

## Résultat de la Décision

Option choisie : Licence MIT car permissive et facilement applicable à la documentation correspondante.

## Avantages et Inconvénients des Options

### CC0

* Bon, car cette licence donne le contenu au "domaine public" et le fait de manière aussi légale que possible.
* Mauvais, car elle ne contient pas d'attribution - et [l'attribution est importante](https://opensource.stackexchange.com/a/9126/5671) et il n'y a pas de reconnaissance de versement direct dans le domaine public dans le droit français.

### Apache licence 2

* Licence persmissive privilégiée par la communauté Apache. A utiliser si l'objectif est de travailler avec cette communauté.

### BSD2 ou BSD3

* Non privilégiée, car il [n'est pas clair qu'elle peut être utilisée pour la documentation](https://opensource.stackexchange.com/a/9545/5671)

### CeCILL-B

* Non privilégiée car elle reprend l’esprit des licences BSD : pas de copyleft mais une exigence de citation.  

### MIT

* Meilleure, car elle [peut explicitement être utilisée pour la documentation](https://opensource.stackexchange.com/a/9545/5671)


### Double licence avec MIT et CC0

Avec l'identifiant SPDX `MIT OR CC0-1.0`, le destinataire des documents peut choisir quelle licence il souhaite utiliser.

* Bon, car cela offre la liberté au destinataire
* Mauvais, car la double licence est plus complexe et le CC0 ne s'applique pas en France

### Conclusion
Par défaut, la licence permissive MIT est donc retenue, mais tout projet nécessitant de participer à une communauté donnée disposant déjà d'une licence majoritaire peut demander à utiliser cette dernière.
