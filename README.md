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

Contenido idéntico al de `wh40k-5ed` al crear el repositorio. La columna *revisión* es el atributo `revision` del fichero: **en este repositorio todos los ficheros empiezan en la revisión 1** (no coincide con la numeración de `wh40k-5ed`) y sube en 1 cada vez que un catálogo cambia.

| Catálogo | Revisión | Unidades |
|---|---|---|
| Sistema de juego (`.gst`) | 1 | — |
| Ángeles Oscuros | 1 | 27 |
| Ángeles Sangrientos | 1 | 35 |
| Caballeros Grises | 1 | 31 |
| Demonios del Caos | 1 | 30 |
| Eldar Oscuros | 1 | 30 |
| Eldars | 1 | 26 |
| Guardia Imperial | 1 | 25 |
| Hermanas de Batalla | 1 | 15 |
| Imperio Tau | 1 | 17 |
| Lobos Espaciales | 1 | 30 |
| Marines Espaciales | 1 | 46 |
| Marines Espaciales del Caos | 1 | 30 |
| Necrones | 1 | 27 |
| Orkos | 1 | 24 |
| Templarios Negros | 1 | 26 |
| Tiránidos | 1 | 30 |

*Unidades = entradas que el jugador ve al montar la lista (enlaces de la raíz del catálogo).*

## Cambios respecto a wh40k-5ed

Cada cambio se anota aquí con la fecha, el catálogo y las unidades **nuevas** o **modificadas**, indicando qué cambia (perfil, coste, opciones, reglas) y cualquier límite o duda que convenga conocer al usarlas.

### Reinicio de revisiones — todos los catálogos y el sistema de juego

- Todas las revisiones (`revision`) pasan a **1**, y el `gameSystemRevision` de cada catálogo a 1, para que este repositorio tenga numeración propia, independiente de `wh40k-5ed`.
- No cambia ninguna unidad ni perfil: el contenido de las unidades sigue siendo idéntico al de `wh40k-5ed`.

### Sincronización con wh40k-5ed (2026-11-27)

- Los catálogos y el sistema de juego vuelven a ser **idénticos a los de `wh40k-5ed`** en su estado actual (incluidas sus últimas correcciones y la revisión de Ángeles Oscuros), porque aquí aún no se ha modificado ni creado ninguna unidad.
- Las revisiones se mantienen en **1** (`revision` y `gameSystemRevision`): la numeración propia de este repositorio no avanza hasta que haya cambios propios.
- El catálogo `Ángeles Oscuros` se llama ahora así (con tilde), igual que en `wh40k-5ed`; sustituye a `Angeles Oscuros.cat`.
