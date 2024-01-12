# @etalab/decoupage-administratif

Données concernant le découpage administratif français, au format JSON.

- Communes
- Arrondissements
- Départements
- Régions
- EPCI (à fiscalité propre)
- EPT (Etablissements Publics Territoriaux), sans fiscalité propre (disponible depuis 2023)

## Installation

```bash
# npm
npm install @etalab/decoupage-administratif

# yarn
yarn add @etalab/decoupage-administratif
```

## Utilisation

### Node

```js
const communes = require('@etalab/decoupage-administratif/data/communes.json')
const departements = require('@etalab/decoupage-administratif/data/departements.json')
const regions = require('@etalab/decoupage-administratif/data/regions.json')
const arrondissements = require('@etalab/decoupage-administratif/data/arrondissements.json')
const epci = require('@etalab/decoupage-administratif/data/epci.json')
const ept = require('@etalab/decoupage-administratif/data/ept.json')
```

### via des URLs

Pour la dernière version

- Communes https://unpkg.com/@etalab/decoupage-administratif/data/communes.json
- Départements https://unpkg.com/@etalab/decoupage-administratif/data/departements.json
- Régions https://unpkg.com/@etalab/decoupage-administratif/data/regions.json
- Arrondissements https://unpkg.com/@etalab/decoupage-administratif/data/arrondissements.json
- EPCI https://unpkg.com/@etalab/decoupage-administratif/data/epci.json
- EPT https://unpkg.com/@etalab/decoupage-administratif/data/ept.json

Il est possible de rajouter une version. Pour les EPCI 2021, par exemple https://unpkg.com/@etalab/decoupage-administratif@1.1.1/data/epci.json (voir le lien millésime et version de packages)

## Millésimes et versions de package

Vous avez besoin de données selon une année? Voici un tableau récapitulatif pour choisir:

| Année | Version du package                        | NPM                                               | Yarn                                               |
|-------|-------------------------------------------|---------------------------------------------------|----------------------------------------------------|
| 2023  | 3.1.1                                     | `npm install @etalab/decoupage-administratif@3.1.1` | `yarn add @etalab/decoupage-administratif@3.1.1` |
| 2022  | 2.3.1                                     | `npm install @etalab/decoupage-administratif@2.3.1` | `yarn add @etalab/decoupage-administratif@2.3.1` |
| 2021  | 1.1.1                                     | `npm install @etalab/decoupage-administratif@1.1.1` | `yarn add @etalab/decoupage-administratif@1.1.1` |
| 2020  | Non disponible, sauf EPCI 2020 avec 0.8.0 | `npm install @etalab/decoupage-administratif@0.8`   | `yarn add @etalab/decoupage-administratif@0.8`   |
| 2019  | 0.7                                       | `npm install @etalab/decoupage-administratif@0.7`   | `yarn add @etalab/decoupage-administratif@0.7`   |

## Sources

* [Code Officiel Géographique](https://insee.fr/fr/information/2560452) de l'INSEE
* [Liste des EPCI à fiscalité propre](https://www.collectivites-locales.gouv.fr/institutions/liste-et-composition-des-epci-fiscalite-propre) de la DGCL ([url exacte](https://www.collectivites-locales.gouv.fr/files/Accueil/DESL/2023/epcicom2023.xlsx))
* [Liste des EPT (Etablissements Publics Territoriaux)](https://www.insee.fr/fr/information/2510634) avec [l'url exacte du fichier](https://www.insee.fr/fr/statistiques/fichier/2510634/ept_au_01-01-2023.xlsx)
* [Population légale](https://www.insee.fr/fr/statistiques/6683035?sommaire=6683037) de l'INSEE + [population Mayotte INSEE 2017](https://www.insee.fr/fr/statistiques/3291775?sommaire=2120838) + [population COM](https://www.insee.fr/fr/statistiques/6683025?sommaire=6683037)
* [Liste des codes postaux](https://www.data.gouv.fr/fr/datasets/base-officielle-des-codes-postaux/) issue des données La Poste. Antérieurement, sous licence ODBL, maintenant en LO
* [Correspondances communes code SIREN et code INSEE](https://www.banatic.interieur.gouv.fr/V5/fichiers-en-telechargement/fichiers-telech.php) Menu gauche "Table de correspondance code SIREN / Code Insee des communes" ([url exacte](https://www.banatic.interieur.gouv.fr/V5/ressources/documents/document_reference/TableCorrespondanceSirenInsee.zip))

## Licence

Données : [Licence Ouverte](https://www.etalab.gouv.fr/licence-ouverte-open-licence)\
Code : MIT
