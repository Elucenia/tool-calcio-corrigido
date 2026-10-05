<!-- ELUCENIA technical documentation · calcio-corrigido · en · no clinical/professional/rights approval -->

# Albumin-corrected calcium

[conditions, sources and permissions](https://elucenia.org/en/tools/calcio-corrigido)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Total calcium

`ca`

mg/dL · range: 2–20

### Albumin

`alb`

g/dL · range: 0.5–6

## Method edition

Simplified adjustment associated with Payne 1973: Ca+0.8×(4−albumin); not measured ionized calcium

## Documented formula

Corrected calcium (mg/dL) = total calcium + 0.8 × (4.0 − albumin in g/dL).

In mmol/L: calcium + 0.02 × (40 − albumin in g/L).

## Limits and population

The formula in Payne’s 1973 publication was derived from samples with protein abnormalities sent for liver function tests and uses an albumin coefficient of 1, with calcium in mg/100 mL and albumin in g/100 mL. The simplified local variant uses 0.8 and needs its own source for that modification. Adjusted calcium is an estimate, not a measurement of ionized calcium.

## References

- [Payne RB, Little AJ, Williams RB, Milner JR. Interpretation of serum calcium in patients with abnormal serum proteins. BMJ, 1973.](https://doi.org/10.1136/bmj.4.5893.643)

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
