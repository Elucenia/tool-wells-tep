<!-- ELUCENIA technical documentation · wells-tep · pt-BR · no clinical/professional/rights approval -->

# Escore de Wells (embolia pulmonar)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/wells-tep)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Sinais clínicos de TVP

`tvp`

### TEP é o diagnóstico mais provável

`alt`

### FC \> 100 bpm

`fc`

### Imobilização ≥ 3 dias ou cirurgia nas últimas 4 semanas

`imob`

### TVP ou TEP prévios

`prev`

### Hemoptise

`hemo`

### Câncer ativo (tratamento nos últimos 6 meses ou paliativo)

`cancer`

## Edição do método

Wells PE 2000:7 fatores ponderados; classificação 2 níveis e 3 níveis separadas

## Fórmula documentada

Soma dos pontos: sinais de TVP 3 · TEP mais provável 3 · FC \> 100 1,5 · imobilização/cirurgia 1,5 · TVP/TEP prévio 1,5 · hemoptise 1 · câncer 1.

## Limites e população

O Wells para embolia foi estudado em pessoas com suspeita clínica e dentro de uma estratégia que combinava escore com D-dímero. As classificações de dois e três níveis têm cortes distintos; escore baixo ou embolia improvável não são sinônimos de embolia ausente. Ensaios de D-dímero e critérios de aplicação devem corresponder ao protocolo diagnóstico utilizado.

## Referências

- [Wells PS et al. Derivation of a simple clinical model to categorize patients probability of pulmonary embolism. Thromb Haemost, 2000.](https://doi.org/10.1055/s-0037-1613830)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism. Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

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

TEP provável: angiotomografia de tórax

| Detalhes do resultado | |
| --- | --- |
| Probabilidade (3 níveis) | moderada (~16,2%) |


### 2

TEP provável: angiotomografia de tórax

| Detalhes do resultado | |
| --- | --- |
| Probabilidade (3 níveis) | alta (~40,6%) |


### 3

TEP improvável: dosar D-dímero

| Detalhes do resultado | |
| --- | --- |
| Probabilidade (3 níveis) | baixa (~1,3%) |

