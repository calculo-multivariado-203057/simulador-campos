# Simulador de campos vectoriales y Maxwell

Recurso educativo digital para la **Fase 4** del curso **Cálculo Multivariado (203057)** de la
Universidad Nacional Abierta y a Distancia (UNAD). Representa el campo, calcula los operadores que
el Apéndice 5 pide calcular, y **comprueba** el trabajo que el estudiante hizo a mano. No resuelve
las integrales ni plantea la igualdad del teorema: eso es de él.

## Qué hace cada módulo

| Módulo | Apoya | Qué hace |
|---|---|---|
| 1 · Campo vectorial y visualización | Actividad 1, ítems I y II | Representa el campo en el espacio a partir de las componentes P, Q y R, y ofrece una lectura visual para que el estudiante escriba su anticipación antes de calcular. |
| 2 · Divergencia y rotacional | Actividad 2, ítems I, II y III | Contrasta primero lo que el estudiante calculó a mano y después muestra los valores, porque el apéndice pide expresamente que el simulador los determine. |
| 3 · Campo sobre la curva o la superficie | Actividad 3, ítems II y IV | Muestra el campo sobre la curva parametrizada o el sólido que la superficie encierra, y comprueba el valor de la circulación o del flujo **sin revelarlo**. |
| 4 · Integrando del teorema | Actividad 4, ítem II | Comprueba que el integrando escrito al lado derecho de la igualdad coincida con la divergencia o con el rotacional, según el teorema elegido. |

La actividad 3 verifica por comparación numérica: la circulación se obtiene integrando sobre la
parametrización que escribe el estudiante, y el flujo por una superficie cerrada se obtiene
integrando la divergencia sobre el sólido que encierra, reconociendo la caja y la bola para
integrarlas con exactitud.

Cada módulo trae un ejemplo resuelto plegado, que permanece oculto hasta que el estudiante lo abre.
El trabajo se conserva en el navegador y puede trasladarse a otro equipo mediante un código, de modo
que la fase puede desarrollarse en varias sesiones y en el orden que el estudiante decida.

## Uso

Abra `index.html` en cualquier navegador moderno. **No requiere instalación, servidor ni conexión a
internet**: mathjs, Plotly y MathJax están incluidos en `vendor/`, de manera que el recurso seguirá
funcionando aunque esos servicios cambien de dirección o el estudiante trabaje sin conectividad,
condición frecuente en las zonas rurales del Caribe colombiano en las que se sitúa el curso.

## Qué comprueba y qué no

| Comprueba | No muestra |
|---|---|
| La divergencia y las tres componentes del rotacional que el estudiante calculó | — (el apéndice pide que el simulador las determine, así que después las muestra) |
| Si la curva parametrizada es cerrada | — |
| El valor de la circulación o del flujo | El valor correcto, cuando el del estudiante no coincide |
| El integrando del lado derecho de la igualdad del teorema | El resultado de esa integral: la actividad 4 pide plantear, no resolver |

## Dónde está publicado

| | |
|---|---|
| Simulador | https://calculo-multivariado-203057.github.io/simulador-campos/ |

El sitio se sirve con GitHub Pages desde la rama `main`, carpeta raíz. El archivo `.nojekyll` evita
el procesamiento de Jekyll, de modo que los archivos se publican tal como están.

## Autoría y filiación

**Pablo Emilio Gutiérrez Duncan**
Director del curso Cálculo Multivariado (203057)
Escuela de Ciencias Básicas, Tecnología e Ingeniería (ECBTI)
Universidad Nacional Abierta y a Distancia (UNAD) — CCAV Puerto Colombia, Zona Caribe
ORCID: https://orcid.org/0009-0001-6596-8536

## Cómo citar

Gutiérrez Duncan, P. E. (2026). *Simulador de campos vectoriales y Maxwell* (versión 1.0)
[Software]. Universidad Nacional Abierta y a Distancia.
https://github.com/calculo-multivariado-203057/simulador-campos

El archivo `CITATION.cff` permite que GitHub genere la cita automáticamente y que Zenodo la lea si
se le asigna un DOI.

## Recursos relacionados

Los tres simuladores del momento intermedio del curso:

| Fase | Recurso |
|---|---|
| 2 | [Simulador de gradiente y optimización](https://github.com/calculo-multivariado-203057/simulador-gradiente) |
| 3 | [Simulador de integración múltiple](https://github.com/calculo-multivariado-203057/simulador-integracion) |
| 4 | Simulador de campos vectoriales y Maxwell (este) |

## Licencia

El simulador se publica bajo **Creative Commons Atribución-NoComercial-CompartirIgual 4.0
Internacional (CC BY-NC-SA 4.0)**; véase [`LICENSE`](LICENSE).

Las bibliotecas incluidas en `vendor/` conservan sus propias licencias, que se distribuyen junto a
cada archivo:

| Componente | Versión | Licencia |
|---|---|---|
| mathjs | 12.4.2 | Apache-2.0 |
| Plotly.js | 2.32.0 | MIT |
| MathJax (salida SVG) | 3.2.2 | Apache-2.0 |
