<!-- ELUCENIA technical documentation · calcio-corrigido · it · no clinical/professional/rights approval -->

# Calcio corretto per albumina

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/calcio-corrigido)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Calcio totale

`ca`

mg/dL · intervallo: 2–20

### Albumina

`alb`

g/dL · intervallo: 0,5–6

## Edizione del metodo

Correzione semplificata associata a Payne 1973: Ca+0,8×(4−albumina); non è calcio ionizzato misurato

## Formula documentata

Calcio corretto (mg/dL) = calcio totale + 0,8 × (4,0 − albumina in g/dL).

In mmol/L: calcio + 0,02 × (40 − albumina in g/L).

## Limiti e popolazione

La formula della pubblicazione Payne 1973 è stata derivata da campioni con alterazioni proteiche inviati per test di funzionalità epatica e impiega il coefficiente 1 per l’albumina, con calcio in mg/100 mL e albumina in g/100 mL. La variante locale semplificata impiega 0,8 e necessita di una propria fonte per questa modifica. Il calcio aggiustato è una stima, non una misurazione del calcio ionizzato.

## Riferimenti

- [Payne RB, Little AJ, Williams RB, Milner JR. Interpretation of serum calcium in patients with abnormal serum proteins. BMJ, 1973.](https://doi.org/10.1136/bmj.4.5893.643)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
