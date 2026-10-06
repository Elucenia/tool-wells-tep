<!-- ELUCENIA technical documentation · wells-tep · en · no clinical/professional/rights approval -->

# Wells score (pulmonary embolism)

[conditions, sources and permissions](https://elucenia.org/en/tools/wells-tep)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Clinical signs of DVT

`tvp`

### PE is the most likely diagnosis

`alt`

### Heart rate \> 100 bpm

`fc`

### Immobilization ≥ 3 days or surgery in the last 4 weeks

`imob`

### Previous DVT or PE

`prev`

### Hemoptysis

`hemo`

### Active cancer (treatment in the last 6 months or palliative treatment)

`cancer`

## Method edition

Wells PE 2000: 7 weighted factors; separate 2-level and 3-level classifications

## Documented formula

Sum of points: DVT signs 3 · PE more likely 3 · HR \> 100 1.5 · immobilization/surgery 1.5 · previous DVT/PE 1.5 · hemoptysis 1 · cancer 1.

## Limits and population

Wells for embolism was studied in people with clinical suspicion within a strategy combining the score with D-dimer. The two- and three-level classifications have different cutoffs; a low score or unlikely embolism does not mean embolism is absent. D-dimer assays and application criteria must match the diagnostic protocol used.

## References

- [Wells PS et al. Derivation of a simple clinical model to categorize patients probability of pulmonary embolism. Thromb Haemost, 2000.](https://doi.org/10.1055/s-0037-1613830)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism. Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Likely PE: chest CT angiography

| Result details | |
| --- | --- |
| Probability (3 levels) | moderate (~16.2%) |


### 2

Likely PE: chest CT angiography

| Result details | |
| --- | --- |
| Probability (3 levels) | high (~40.6%) |


### 3

Unlikely PE: measure D-dimer

| Result details | |
| --- | --- |
| Probability (3 levels) | low (~1.3%) |

