<!-- ELUCENIA technical documentation · wells-tep · fr · no clinical/professional/rights approval -->

# Score de Wells (embolie pulmonaire)

[conditions, sources et autorisations](https://elucenia.org/fr/outils/wells-tep)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Signes cliniques de TVP

`tvp`

### L’EP est le diagnostic le plus probable

`alt`

### Fréquence cardiaque \> 100 bpm

`fc`

### Immobilisation ≥ 3 jours ou chirurgie dans les 4 dernières semaines

`imob`

### Antécédents de TVP ou d’EP

`prev`

### Hémoptysie

`hemo`

### Cancer actif (traitement dans les 6 derniers mois ou palliatif)

`cancer`

## Édition de la méthode

Wells PE 2000 : 7 facteurs pondérés ; classifications à 2 et 3 niveaux distinctes

## Formule documentée

Somme des points : signes de TVP 3 · EP plus probable 3 · FC \> 100 1,5 · immobilisation/chirurgie 1,5 · TVP/EP antérieure 1,5 · hémoptysie 1 · cancer 1.

## Limites et population

Le Wells pour l’embolie a été étudié chez des personnes présentant une suspicion clinique, dans une stratégie combinant le score aux D-dimères. Les classifications à deux et trois niveaux ont des seuils distincts ; un score faible ou une embolie improbable ne signifie pas une embolie absente. Les dosages de D-dimères et les critères d’application doivent correspondre au protocole diagnostique utilisé.

## Références

- [Wells PS et al. Derivation of a simple clinical model to categorize patients probability of pulmonary embolism. Thromb Haemost, 2000.](https://doi.org/10.1055/s-0037-1613830)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism. Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

EP probable : angio-TDM thoracique

| Détails du résultat | |
| --- | --- |
| Probabilité (3 niveaux) | modérée (~16,2%) |


### 2

EP probable : angio-TDM thoracique

| Détails du résultat | |
| --- | --- |
| Probabilité (3 niveaux) | élevée (~40,6%) |


### 3

EP improbable : doser le D-dimère

| Détails du résultat | |
| --- | --- |
| Probabilité (3 niveaux) | faible (~1,3%) |

