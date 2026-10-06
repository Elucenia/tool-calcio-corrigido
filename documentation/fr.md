<!-- ELUCENIA technical documentation · calcio-corrigido · fr · no clinical/professional/rights approval -->

# Calcémie corrigée sur l’albumine

[conditions, sources et autorisations](https://elucenia.org/fr/outils/calcio-corrigido)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Calcium total

`ca`

mg/dL · intervalle: 2–20

### Albumine

`alb`

g/dL · intervalle: 0,5–6

## Édition de la méthode

Correction simplifiée associée à Payne 1973 : Ca+0,8×(4−albumine) ; pas une mesure du calcium ionisé

## Formule documentée

Calcium corrigé (mg/dL) = calcium total + 0,8 × (4,0 − albumine en g/dL).

En mmol/L : calcium + 0,02 × (40 − albumine en g/L).

## Limites et population

La formule de Payne 1973 a été dérivée d’échantillons présentant des anomalies protéiques adressés pour des tests de fonction hépatique et utilise un coefficient de 1 pour l’albumine, avec le calcium en mg/100 mL et l’albumine en g/100 mL. La variante locale simplifiée utilise 0,8 et nécessite une source propre à cette modification. Le calcium ajusté est une estimation et non un dosage du calcium ionisé.

## Références

- [Payne RB, Little AJ, Williams RB, Milner JR. Interpretation of serum calcium in patients with abnormal serum proteins. BMJ, 1973.](https://doi.org/10.1136/bmj.4.5893.643)

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

Calcium corrigé dans la plage normale (8,5 à 10,5 mg/dL)

La correction est approximative : chez un patient critique, en cas de trouble acido-basique ou de maladie rénale, confirmer par le calcium ionisé.


### 2

Calcium corrigé bas (< 8,5 mg/dL) : hypocalcémie probable

La correction est approximative : chez un patient critique, en cas de trouble acido-basique ou de maladie rénale, confirmer par le calcium ionisé.


### 3

Calcium corrigé élevé (> 10,5 mg/dL) : hypercalcémie probable

La correction est approximative : chez un patient critique, en cas de trouble acido-basique ou de maladie rénale, confirmer par le calcium ionisé.


### 4

Calcium corrigé dans la plage normale (8,5 à 10,5 mg/dL)

La correction est approximative : chez un patient critique, en cas de trouble acido-basique ou de maladie rénale, confirmer par le calcium ionisé.

