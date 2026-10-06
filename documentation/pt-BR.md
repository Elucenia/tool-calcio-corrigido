<!-- ELUCENIA technical documentation · calcio-corrigido · pt-BR · no clinical/professional/rights approval -->

# Cálcio corrigido pela albumina

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/calcio-corrigido)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Cálcio total

`ca`

mg/dL · intervalo: 2–20

### Albumina

`alb`

g/dL · intervalo: 0,5–6

## Edição do método

Ajuste simplificado associado a Payne 1973:Ca+0,8×(4−albumina); nãoé cálcio ionizado medido

## Fórmula documentada

Cálcio corrigido (mg/dL) = cálcio total + 0,8 × (4,0 − albumina em g/dL).

Em mmol/L: cálcio + 0,02 × (40 − albumina em g/L).

## Limites e população

A fórmula da publicação Payne 1973 foi derivada de amostras com alterações proteicas enviadas para testes de função hepática e emprega coeficiente 1 para albumina, com cálcio em mg/100 mL e albumina em g/100 mL. A variante simplificada local emprega 0,8 e necessita de fonte própria para essa modificação. Cálcio ajustado é uma estimativa e não uma dosagem de cálcio ionizado.

## Referências

- [Payne RB, Little AJ, Williams RB, Milner JR. Interpretation of serum calcium in patients with abnormal serum proteins. BMJ, 1973.](https://doi.org/10.1136/bmj.4.5893.643)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Cálcio corrigido na faixa normal (8,5 a 10,5 mg/dL)

A correção é aproximada: em paciente crítico, com distúrbio ácido-base ou doença renal, confirme com o cálcio iônico.


### 2

Cálcio corrigido baixo (< 8,5 mg/dL): hipocalcemia provável

A correção é aproximada: em paciente crítico, com distúrbio ácido-base ou doença renal, confirme com o cálcio iônico.


### 3

Cálcio corrigido elevado (> 10,5 mg/dL): hipercalcemia provável

A correção é aproximada: em paciente crítico, com distúrbio ácido-base ou doença renal, confirme com o cálcio iônico.


### 4

Cálcio corrigido na faixa normal (8,5 a 10,5 mg/dL)

A correção é aproximada: em paciente crítico, com distúrbio ácido-base ou doença renal, confirme com o cálcio iônico.

