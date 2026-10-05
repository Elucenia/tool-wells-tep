<!-- ELUCENIA technical documentation · wells-tep · es · no clinical/professional/rights approval -->

# Puntuación de Wells (embolia pulmonar)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/wells-tep)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Signos clínicos de TVP

`tvp`

### La EP es el diagnóstico más probable

`alt`

### Frecuencia cardíaca \> 100 bpm

`fc`

### Inmovilización ≥ 3 días o cirugía en las últimas 4 semanas

`imob`

### TVP o EP previas

`prev`

### Hemoptisis

`hemo`

### Cáncer activo (tratamiento en los últimos 6 meses o paliativo)

`cancer`

## Edición del método

Wells PE 2000: 7 factores ponderados; clasificaciones de 2 y 3 niveles separadas

## Fórmula documentada

Suma de puntos: signos de TVP 3 · TEP más probable 3 · FC \> 100 1,5 · inmovilización/cirugía 1,5 · TVP/TEP previo 1,5 · hemoptisis 1 · cáncer 1.

## Límites y población

El Wells para embolia se estudió en personas con sospecha clínica y dentro de una estrategia que combinaba la puntuación con dímero D. Las clasificaciones de dos y tres niveles tienen puntos de corte distintos; una puntuación baja o una embolia improbable no equivalen a ausencia de embolia. Los ensayos de dímero D y los criterios de aplicación deben corresponder al protocolo diagnóstico utilizado.

## Referencias

- [Wells PS et al. Derivation of a simple clinical model to categorize patients probability of pulmonary embolism. Thromb Haemost, 2000.](https://doi.org/10.1055/s-0037-1613830)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism. Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

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
