<!-- ELUCENIA technical documentation · wells-tep · de · no clinical/professional/rights approval -->

# Wells-Score (Lungenembolie)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/wells-tep)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Klinische Zeichen einer TVT

`tvp`

### Lungenembolie ist die wahrscheinlichste Diagnose

`alt`

### Herzfrequenz \> 100 bpm

`fc`

### Immobilisation ≥ 3 Tage oder Operation in den letzten 4 Wochen

`imob`

### Frühere TVT oder Lungenembolie

`prev`

### Hämoptyse

`hemo`

### Aktiver Krebs (Behandlung in den letzten 6 Monaten oder palliativ)

`cancer`

## Fassung der Methode

Wells PE 2000: 7 gewichtete Faktoren; getrennte Einteilung in 2 und 3 Stufen

## Dokumentierte Formel

Punktesumme: TVT-Zeichen 3 · LE wahrscheinlicher 3 · Herzfrequenz \> 100 1,5 · Immobilisierung/Operation 1,5 · frühere TVT/LE 1,5 · Hämoptyse 1 · Krebs 1.

## Grenzen und Population

Wells für Embolie wurde bei Personen mit klinischem Verdacht innerhalb einer Strategie untersucht, die Score und D-Dimer kombinierte. Zwei- und dreistufige Klassifikationen haben unterschiedliche Schwellen; niedriger Score oder unwahrscheinliche Embolie sind nicht mit fehlender Embolie gleichzusetzen. D-Dimer-Assays und Anwendungskriterien müssen zum verwendeten diagnostischen Protokoll passen.

## Referenzen

- [Wells PS et al. Derivation of a simple clinical model to categorize patients probability of pulmonary embolism. Thromb Haemost, 2000.](https://doi.org/10.1055/s-0037-1613830)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism. Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

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
