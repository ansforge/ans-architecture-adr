---
parent: Decisions
nav_order: 1
---

# Licence des projets Github

* statut : proposé
* date : 2025-05-27
* décisionnaires : CTO
* consultés : CTO
* informés : équipe intégration, directeurs de domaine

## Contexte et énoncé du problème

Tout doit être sous licence sinon les lois de copyright par défaut s'appliquent.
Par exemple, en Allemagne, cela signifie que les utilisateurs ne peuvent pas modifier quoi que ce soit sans demander explicitement la permission.
Pour plus d'informations, voir <https://help.github.com/articles/licensing-a-repository/>.

## Options Envisagées

* [CC0](https://creativecommons.org/share-your-work/public-domain/cc0/)
* BSD3
* MIT
* Double licence MIT et CC0
* Aucune licence
* Autres licences open source

## Résultat de la Décision

Option choisie : Licence MIT car permissive.

## Avantages et Inconvénients des Options

### CC0

* Bon, car cette licence donne le contenu au "domaine public" et le fait de manière aussi légale que possible.
* Mauvais, car elle ne contient pas d'attribution - et [l'attribution est importante](https://opensource.stackexchange.com/a/9126/5671).

### BSD3

* Mauvais, car il [n'est pas clair qu'elle peut être utilisée pour la documentation](https://opensource.stackexchange.com/a/9545/5671)

### MIT

* Bon, car elle [peut explicitement être utilisée pour la documentation](https://opensource.stackexchange.com/a/9545/5671)
* Bon, car elle est concrète.

### Double licence avec MIT et CC0

Avec l'identifiant SPDX `MIT OR CC0-1.0`, le destinataire des documents peut choisir quelle licence il souhaite utiliser.

* Bon, car cela offre la liberté au destinataire
* Mauvais, car la double licence n'est pas largement connue
