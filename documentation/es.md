<!-- ELUCENIA technical documentation · calcio-corrigido · es · no clinical/professional/rights approval -->

# Calcio corregido por albúmina

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/calcio-corrigido)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Calcio total

`ca`

mg/dL · intervalo: 2–20

### Albúmina

`alb`

g/dL · intervalo: 0,5–6

## Edición del método

Ajuste simplificado asociado a Payne 1973: Ca+0,8×(4−albúmina); no es calcio ionizado medido

## Fórmula documentada

Calcio corregido (mg/dL) = calcio total + 0,8 × (4,0 − albúmina en g/dL).

En mmol/L: calcio + 0,02 × (40 − albúmina en g/L).

## Límites y población

La fórmula de la publicación Payne 1973 se derivó de muestras con alteraciones proteicas enviadas para pruebas de función hepática y utiliza un coeficiente de 1 para la albúmina, con calcio en mg/100 mL y albúmina en g/100 mL. La variante simplificada local utiliza 0,8 y necesita una fuente propia para esta modificación. El calcio ajustado es una estimación, no una medición del calcio ionizado.

## Referencias

- [Payne RB, Little AJ, Williams RB, Milner JR. Interpretation of serum calcium in patients with abnormal serum proteins. BMJ, 1973.](https://doi.org/10.1136/bmj.4.5893.643)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Calcio corregido en el rango normal (8,5 a 10,5 mg/dL)

La corrección es aproximada: en un paciente crítico, con trastorno ácido-base o enfermedad renal, confirmar con calcio iónico.


### 2

Calcio corregido bajo (< 8,5 mg/dL): hipocalcemia probable

La corrección es aproximada: en un paciente crítico, con trastorno ácido-base o enfermedad renal, confirmar con calcio iónico.


### 3

Calcio corregido elevado (> 10,5 mg/dL): hipercalcemia probable

La corrección es aproximada: en un paciente crítico, con trastorno ácido-base o enfermedad renal, confirmar con calcio iónico.


### 4

Calcio corregido en el rango normal (8,5 a 10,5 mg/dL)

La corrección es aproximada: en un paciente crítico, con trastorno ácido-base o enfermedad renal, confirmar con calcio iónico.

