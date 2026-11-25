# Warhammer 40,000 5ª edición ampliada

Sistema de juego y catálogos de **Warhammer 40,000 5ª edición ampliada** para [NewRecruit](https://www.newrecruit.eu/) / BattleScribe: la 5ª edición con **unidades modificadas** y **unidades y ejércitos nuevos** que no existen en la edición original.

Parte de una copia exacta del repositorio [wh40k-5ed](https://github.com/DiegoMunnizVelazquez/wh40k-5ed). **Ese repositorio no se modifica**: conserva las unidades y los perfiles tal y como son en la 5ª edición. Todo lo que cambia o se añade vive solo aquí.

## Contenido

| Fichero | Para qué sirve |
|---|---|
| `Warhammer 40,000 5ª Edición.gst` | Sistema de juego (reglas, categorías, perfiles y reglas comunes). Es necesario para cargar cualquier catálogo. |
| `*.cat` | Un catálogo por ejército. |
| `README.md` | Esta guía y el registro de cambios. |

## Cómo usarlo

Hacen falta **el `.gst` y los `.cat` juntos**: los catálogos dependen del sistema de juego (`gameSystemId` `8cf6-c83d-3eeb-e95c`).

- Cargar este repositorio de GitHub como fuente de datos en NewRecruit / BattleScribe, o
- descargar el `.gst` y los `.cat` y añadirlos a la carpeta de datos de la aplicación.

Este repositorio **no incluye el paquete `.bsr`**. Si usas también `wh40k-5ed`, no cargues ambos con el mismo sistema de juego a la vez: son versiones distintas del mismo sistema (mismo `gameSystemId`).

## Catálogos

Estado al crear el repositorio (idéntico al de `wh40k-5ed`). La columna *revisión* es el atributo `revision` del fichero y sube cada vez que un catálogo cambia.

| Catálogo | Revisión | Unidades |
|---|---|---|
| Sistema de juego (`.gst`) | 33 | — |
| Ángeles Oscuros | 17 | 27 |
| Ángeles Sangrientos | 15 | 35 |
| Caballeros Grises | 16 | 31 |
| Demonios del Caos | 4 | 30 |
| Eldar Oscuros | 6 | 30 |
| Eldars | 7 | 26 |
| Guardia Imperial | 13 | 25 |
| Hermanas de Batalla | 5 | 15 |
| Imperio Tau | 6 | 17 |
| Lobos Espaciales | 20 | 30 |
| Marines Espaciales | 35 | 46 |
| Marines Espaciales del Caos | 17 | 30 |
| Necrones | 8 | 27 |
| Orkos | 8 | 24 |
| Templarios Negros | 43 | 26 |
| Tiránidos | 7 | 30 |

*Unidades = entradas que el jugador ve al montar la lista (enlaces de la raíz del catálogo).*

## Cambios respecto a wh40k-5ed

Cada cambio se anota aquí con la fecha, el catálogo y las unidades **nuevas** o **modificadas**, indicando qué cambia (perfil, coste, opciones, reglas) y cualquier límite o duda que convenga conocer al usarlas.

_Todavía no hay cambios: los catálogos y el sistema de juego son idénticos a los de `wh40k-5ed`._
