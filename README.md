# S/4 Check

Outil d'aide à la reprise du code ABAP pour la migration SAP S/4HANA.
Page autonome : aucun serveur, aucune connexion réseau, rien n'est envoyé.

**Site : https://<compte>.github.io/<depot>/**

## Ce qui fonctionne immédiatement

| Onglet | État |
|---|---|
| **Conversion ATC** | opérationnel — réécrit les instructions signalées par l'ATC |
| **Recherche** | attend vos données |
| **Analyse de code** | attend vos données |
| **SELECT → ACDOCA** | attend vos données |

L'onglet Conversion ATC couvre les notes 2610650 (montants), 2215424
(numéro d'article) et la famille sans note (dépendance à l'ordre des lignes).
Il n'a besoin d'aucune donnée externe.

## Charger vos données

Les onglets Recherche, Analyse et SELECT → ACDOCA s'appuient sur des données
extraites de notes SAP. **Ce contenu n'est pas publié ici** : il provient de
notes accessibles derrière authentification SAP, et n'a pas à figurer sur un
site en libre accès.

Chacun génère les siennes avec les scripts du projet, puis les charge depuis
le bandeau en haut de la page :

- `index.json`
- `acdoca_fields.json`
- `struct_fields.json`

La lecture se fait **dans votre navigateur**. Les fichiers ne quittent pas
votre poste et ne sont envoyés à personne.

## Vérifier l'intégrité du fichier

    sha256sum index.html

Le résultat doit correspondre au contenu de `index.html.sha256`.

## Licence

© AEH. Usage autorisé. Modification, redistribution et réutilisation
soumises à autorisation écrite de l'auteur. Voir l'en-tête de `index.html`.
