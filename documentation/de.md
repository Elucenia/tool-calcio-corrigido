<!-- ELUCENIA technical documentation · calcio-corrigido · de · no clinical/professional/rights approval -->

# Albuminkorrigiertes Kalzium

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/calcio-corrigido)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Gesamtkalzium

`ca`

mg/dL · Bereich: 2–20

### Albumin

`alb`

g/dL · Bereich: 0,5–6

## Fassung der Methode

Vereinfachte Korrektur nach Payne 1973: Ca+0,8×(4−Albumin); kein gemessenes ionisiertes Kalzium

## Dokumentierte Formel

Korrigiertes Kalzium (mg/dL) = Gesamtkalzium + 0,8 × (4,0 − Albumin in g/dL).

In mmol/L: Kalzium + 0,02 × (40 − Albumin in g/L).

## Grenzen und Population

Die Formel aus Payne 1973 wurde anhand von Proben mit Proteinveränderungen entwickelt, die für Leberfunktionstests eingesandt wurden, und verwendet einen Albuminkoeffizienten von 1 mit Kalzium in mg/100 mL und Albumin in g/100 mL. Die vereinfachte lokale Variante verwendet 0,8 und benötigt eine eigene Quelle für diese Änderung. Adjustiertes Kalzium ist eine Schätzung, keine Messung des ionisierten Kalziums.

## Referenzen

- [Payne RB, Little AJ, Williams RB, Milner JR. Interpretation of serum calcium in patients with abnormal serum proteins. BMJ, 1973.](https://doi.org/10.1136/bmj.4.5893.643)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Korrigiertes Kalzium im Normbereich (8,5 bis 10,5 mg/dL)

Die Korrektur ist näherungsweise: bei kritisch kranken Patienten, mit Säure-Basen-Störung oder Nierenerkrankung, mit ionisiertem Kalzium bestätigen.


### 2

Niedriges korrigiertes Kalzium (< 8,5 mg/dL): wahrscheinliche Hypokalzämie

Die Korrektur ist näherungsweise: bei kritisch kranken Patienten, mit Säure-Basen-Störung oder Nierenerkrankung, mit ionisiertem Kalzium bestätigen.


### 3

Erhöhtes korrigiertes Kalzium (> 10,5 mg/dL): wahrscheinliche Hyperkalzämie

Die Korrektur ist näherungsweise: bei kritisch kranken Patienten, mit Säure-Basen-Störung oder Nierenerkrankung, mit ionisiertem Kalzium bestätigen.


### 4

Korrigiertes Kalzium im Normbereich (8,5 bis 10,5 mg/dL)

Die Korrektur ist näherungsweise: bei kritisch kranken Patienten, mit Säure-Basen-Störung oder Nierenerkrankung, mit ionisiertem Kalzium bestätigen.

