<!-- ELUCENIA technical documentation · wells-tep · it · no clinical/professional/rights approval -->

# Punteggio di Wells (embolia polmonare)

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/wells-tep)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Segni clinici di TVP

`tvp`

### L’EP è la diagnosi più probabile

`alt`

### Frequenza cardiaca \> 100 bpm

`fc`

### Immobilizzazione ≥ 3 giorni o intervento nelle ultime 4 settimane

`imob`

### TVP o EP pregresse

`prev`

### Emottisi

`hemo`

### Cancro attivo (trattamento negli ultimi 6 mesi o palliativo)

`cancer`

## Edizione del metodo

Wells PE 2000: 7 fattori ponderati; classificazioni a 2 e 3 livelli separate

## Formula documentata

Somma dei punti: segni di TVP 3 · EP più probabile 3 · FC \> 100 1,5 · immobilizzazione/chirurgia 1,5 · TVP/EP precedente 1,5 · emottisi 1 · cancro 1.

## Limiti e popolazione

Il Wells per embolia è stato studiato in persone con sospetto clinico e all’interno di una strategia che combinava il punteggio con il D-dimero. Le classificazioni a due e tre livelli hanno soglie diverse; un punteggio basso o un’embolia improbabile non significano embolia assente. Dosaggi del D-dimero e criteri di applicazione devono corrispondere al protocollo diagnostico utilizzato.

## Riferimenti

- [Wells PS et al. Derivation of a simple clinical model to categorize patients probability of pulmonary embolism. Thromb Haemost, 2000.](https://doi.org/10.1055/s-0037-1613830)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism. Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

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

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

EP probabile: angio-TC del torace

| Dettagli del risultato | |
| --- | --- |
| Probabilità (3 livelli) | moderata (~16,2%) |


### 2

EP probabile: angio-TC del torace

| Dettagli del risultato | |
| --- | --- |
| Probabilità (3 livelli) | alta (~40,6%) |


### 3

EP improbabile: dosare il D-dimero

| Dettagli del risultato | |
| --- | --- |
| Probabilità (3 livelli) | bassa (~1,3%) |

