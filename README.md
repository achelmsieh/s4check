# S/4 Check

Outil d'aide à la reprise du code ABAP pour la migration SAP S/4HANA.
Page autonome : aucun serveur, aucune connexion réseau, rien n'est envoyé.

**Site : https://achelmsieh.github.io/s4check/**

## Les quatre onglets

| Onglet | À quoi ça sert |
|---|---|
| **Recherche** | Parcourir l'index par module fonction, paramètre ou data element. |
| **Analyse de code** | Coller du code ABAP : les modules fonction sont détectés, les champs impactés surlignés, le pragma ATC généré. |
| **SELECT → ACDOCA** | Réécrire un `SELECT` sur BSEG / BKPF / COEP / FAGLFLEXA vers ACDOCA, avec les avertissements ledger, signe et périmètre. |
| **Conversion ATC** | Réécrire les instructions signalées par l'ATC, groupées par note. |

## Les notes couvertes

| Note | Sujet |
|---|---|
| 2628704 | AFLE — extension de longueur de champ |
| 2438131 | Datatypes des paramètres de BAPI |
| 2438006 | N° article 18 → 40, modules fonction locaux |
| 2156822 | Mapping des champs vers ACDOCA |
| 2610650 | Extension des champs montant (AFLE) |
| 2215424 | Extension du n° article à 40 caractères |
| *sans note* | Dépendance à l'ordre des lignes |

Chaque note s'active et se désactive depuis la barre sous les onglets.
Survolez un numéro pour savoir ce qu'il couvre et ce qui reste manuel.

## Vérifier l'intégrité du fichier

    sha256sum index.html

Le résultat doit correspondre au contenu de `index.html.sha256`.

## Licence

© AEH. Usage autorisé. Modification, redistribution et réutilisation
soumises à autorisation écrite de l'auteur. Voir l'en-tête de `index.html`.
