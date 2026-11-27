# Warhammer 40,000 5ª edición ampliada

Sistema de juego y catálogos de **Warhammer 40,000 5ª edición ampliada** para [NewRecruit](https://www.newrecruit.eu/) / BattleScribe: la 5ª edición con **unidades modificadas** y **unidades y ejércitos nuevos** que no existen en la edición original.

Parte de una copia exacta del repositorio [wh40k-5ed](https://github.com/DiegoMunnizVelazquez/wh40k-5ed). **Ese repositorio no se modifica**: conserva las unidades y los perfiles tal y como son en la 5ª edición. Todo lo que cambia o se añade vive solo aquí.

## Contenido

| Fichero | Para qué sirve |
|---|---|
| `Warhammer 40,000 5ª Edición Ampliada.gst` | Sistema de juego (reglas, categorías, perfiles y reglas comunes). Es necesario para cargar cualquier catálogo. |
| `*.cat` | Un catálogo por ejército. |
| `README.md` | Esta guía y el registro de cambios. |

## Cómo usarlo

Hacen falta **el `.gst` y los `.cat` juntos**: los catálogos dependen del sistema de juego (`gameSystemId` `310af520-2d8e-4c1d-b969-d49b4f3ad0f9`).

- Cargar este repositorio de GitHub como fuente de datos en NewRecruit / BattleScribe, o
- descargar el `.gst` y los `.cat` y añadirlos a la carpeta de datos de la aplicación.

Este repositorio **no incluye el paquete `.bsr`**. El sistema de juego tiene **nombre e identificador propios** («Warhammer 40,000 5ª Edición Ampliada»), distintos de los de `wh40k-5ed`, así que NewRecruit / BattleScribe los trata como sistemas independientes y se pueden tener cargados a la vez.

## Catálogos

Contenido idéntico al de `wh40k-5ed` al crear el repositorio. La columna *revisión* es el atributo `revision` del fichero: **en este repositorio todos los ficheros empiezan en la revisión 1** (no coincide con la numeración de `wh40k-5ed`) y sube en 1 cada vez que un catálogo cambia.

| Catálogo | Revisión | Unidades |
|---|---|---|
| Sistema de juego (`.gst`) | 1 | — |
| Ángeles Oscuros | 2 | 27 |
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

### Ángeles Oscuros — equipo de CG alineado con Marines Espaciales (revisión 2)

Costes y opciones de equipo del Señor de la Compañía, el Bibliotecario, el Capellán y el Capellán Interrogador tomados de sus equivalentes de `Marines Espaciales` (Capitán, Bibliotecario y Capellán). Los personajes con nombre (Azrael, Ezekiel, Belial, Sammael) no cambian.

- **Señor de la Compañía** (modificada): mismo equipo que el Capitán de ME (grupo Armadura con servoarmadura y armadura de exterminador, dos armas a elegir, retrorreactor o moto) y sus costes. Se excluyen arma reliquia, armadura artesanal, armas digitales, munición infierno y lanzagranadas auxiliar. Conserva el *par de cuchillas relámpago* (+30), propio de AO.
- **Bibliotecario** (modificada): coste base 120 → **100**; grupo Armadura, Epistolario (+50) y costes iguales a los del Bibliotecario de ME. Se mantienen sus poderes psíquicos, la capucha y el arma psíquica de AO. Desaparecen las bombas de fusión, que ME no ofrece.
- **Capellán Interrogador** (modificada): mismas opciones y costes que el Capellán de ME, con armadura de exterminador (+30) y armas digitales (+10). Base sin cambios (120).
- **Capellán** (modificada, solo costes): puño de combate +25 → +15, combifusión, combilanzallamas y combiplasma +10 → +15, bólter de asalto +5 → +3, retrorreactor +20 → +15, moto +30 → +35. No puede llevar armadura de exterminador ni armas digitales.
- **Combiarmas (combifusión, combilanzallamas, combiplasma):** +15 con servoarmadura en el Bibliotecario, el Capellán y el Capellán Interrogador; solo el Señor de la Compañía las mantiene en +10. Con armadura de exterminador: +5 (Señor de la Compañía e Interrogador) y +10 (Bibliotecario, 35 pts con la armadura, como en ME).
- Límite conocido: el *par de cuchillas relámpago* cuenta como una sola arma del grupo de dos armas, aunque ocupa las dos manos.

### Ángeles Oscuros — Dreadnought alineado con Marines Espaciales (revisión 2)

- **Dreadnought** (modificada): base 125 → **105** y mismas opciones y costes que el Dreadnought de ME: cápsula de desembarco asignada (+35, con baliza localizadora y arma principal, y el perfil de transporte de ME), blindaje adicional, brazo cuerpo a cuerpo (cañón automático acoplado, lanzamisiles, arma de combate con bólter de asalto o lanzallamas pesado) y arma a distancia (lanzallamas pesado acoplado, bólter pesado acoplado, cañón de fusión, plasma, asalto, láser acoplado y cañón automático acoplado). Desaparece la opción «Venerable» (+20).
- **Dreadnought Venerable** (nueva, Élite): entrada propia por tener un perfil distinto (HA 5 y HP 5), copia la de ME: base 165 y mismas opciones que el Dreadnought, con el brazo y el arma a distancia de ME.
- **Cápsula de desembarco única:** todas las unidades de AO que la llevan (Dreadnought, Veteranos, Escuadra Táctica, Asalto, Devastadores y Mando) usan ahora la de ME: +35 pts, baliza localizadora (+10), arma principal (bólter de asalto o lanzamisiles viento de muerte +20), HP 4 y capacidad 12. Se elimina la cápsula propia de AO (+50, HP 2, capacidad 10). El orden de los transportes asignados queda Cápsula, Rhino y Razorback.
- Las armas y el equipo que ya existían en AO (cañones, lanzallamas, lanzamisiles, blindaje, bólter de asalto) se reutilizan; se añaden las entradas de ME que AO no tenía (cápsula de desembarco de ME con su perfil y reglas, baliza localizadora y grupos asociados).

### Ángeles Oscuros — Escuadra Táctica igual a la de Marines Espaciales (revisión 2)

- **Escuadra Táctica** (modificada, Línea): misma estructura y costes que la de ME. Marine Espacial +15 → **+16** y Sargento +30 → **+26** (el mínimo sigue en 90 pts). El sargento pasa a un único grupo de armas (bólter y pistola bólter por defecto, espada sierra, bólter de asalto +10, combifusión, combilanzallamas y combiplasma +10, arma de energía +15, pistola de plasma +15, puño de combate +25) y gana la baliza de teleportación (+15). Se mantiene el «arma de energía» de AO en lugar de la espada de energía de ME (mismas reglas).
- **Armas de la escuadra:** arma especial y arma pesada solo en escuadra de diez, como en ME (en AO la especial se podía llevar con cualquier tamaño). Costes de ME: lanzallamas 0, rifle de fusión +5, rifle de plasma +10; bólter pesado, cañón de fusión y lanzamisiles 0, cañón de plasma +5, cañón láser +10.
- **Transportes:** la cápsula de desembarco solo se ofrece con diez marines, como en ME. El **Razorback pasa de +50 a +40** (como en ME) en todas las unidades que lo llevan, porque es una entrada compartida.
- No se añade la regla «Tácticas de Combate», que en ME es propia del codex y no existe en AO.

### Ángeles Oscuros — Escuadra de Asalto igual a la de Marines Espaciales (revisión 2)

- **Escuadra de Asalto** (modificada, Ataque Rápido): misma estructura y costes que la de ME. Marine Espacial de Asalto +22 → **+18**, Sargento +37 → **+28** y escudo de combate del sargento +10 → **+5** (el mínimo baja de 125 a **100** pts).
- **Sargento:** un único grupo de armas (dos a elegir, espada sierra y pistola bólter por defecto) con cuchilla relámpago +15, escudo de tormenta +15, arma de energía +15, pistola de plasma +15, puño de combate +25 y martillo de trueno +30. Mantiene el arma de energía de AO en lugar de la espada de energía de ME.
- **Marines:** arma especial **una por cada cinco miniaturas** (en lugar de un máximo fijo de dos pistolas de plasma): lanzallamas +10, pistola de plasma +15 y, **nuevo, rifle de plasma +15**.
- Conserva la regla «Despliegue Rápido» de AO y no añade «Tácticas de Combate» (propia del codex de ME).

### Ángeles Oscuros — Escuadrón de Apoyo del Ala de Cuervo con los costes de los Land Speeders de ME (revisión 2)

- **Escuadrón de Apoyo del Ala de Cuervo** (modificado, Ataque Rápido): costes y opciones de armas como el Escuadrón de Land Speeders de ME, **manteniendo hasta 5 Land Speeders** por unidad (en ME son 3). Land Speeder +65 → **+50** (mínimo 65 → 50 pts).
- **Arma principal:** bólter pesado por defecto, lanzallamas pesado +0 (nuevo) y cañón de fusión +0 → **+10**.
- **Lanzamisiles Tifón:** +10 → **+40**.
- **Modelo Tornado:** sus armas se amplían a las de ME, con sus costes: bólter pesado +10 (nuevo, por defecto), lanzallamas pesado +10, cañón de fusión +20 (nuevo) y cañón de asalto +35 → **+40**.
- **Sin límite por escuadrón:** como en ME, cualquier Land Speeder puede llevar una mejora (Tifón o Tornado); se elimina el límite de AO de un Tifón y un Tornado por unidad. Se añade la regla **«Despliegue Rápido»** al Land Speeder, como en ME.

### Ángeles Oscuros — Escuadrón de Ataque del Ala de Cuervo con los costes de las motocicletas de ME (revisión 2)

- **Escuadrón de Ataque del Ala de Cuervo** (modificado, Ataque Rápido; también su copia de Línea): sin coste base, como el Escuadrón de Motocicletas de ME. Antes costaba 120 pts fijos por el sargento y dos motoristas; ahora el **Sargento del Ala de Cuervo cuesta +40** y cada **Motorista +25**, así que el mínimo baja de 120 a **90** pts.
- **Motoristas:** de 2 a **7** en un único bloque, como los marines motorizados de ME (unidades de hasta 8 con el sargento). Desaparece la opción «Tres Motoristas del Ala de Cuervo adicionales (+100)».
- **Armas de los motoristas:** todos llevan siempre la **pistola bólter** (equipo fijo, como en ME) y pueden añadir además un **arma especial** (lanzallamas +5, rifle de fusión +10 o rifle de plasma +15), **una por moto** y hasta dos por escuadrón. Se elimina la opción de espada sierra.
- **Motocicleta de Ataque:** +50 → **+40**, y el cañón de fusión +0 → **+10**.
- **Sargento:** un único grupo de armas, como en ME: pistola bólter por defecto, combifusión, combilanzallamas y combiplasma **+10** (nuevas), arma de energía +15 (la de AO en lugar de la espada de energía de ME), pistola de plasma +15 y puño de combate +25. Se elimina la opción de espada sierra, que ME no tiene. Mantiene la baliza de teleportación y las bombas de fusión.
- **Land Speeder (a partir de 6 miniaturas):** +100 → **+50**, con las mismas opciones que el Escuadrón de Apoyo (arma principal bólter pesado / lanzallamas pesado / cañón de fusión +10, Lanzamisiles Tifón +40 y modelo Tornado) y la regla «Despliegue Rápido».
- **Land Speeder compartido:** el Land Speeder del Escuadrón de Apoyo y el de las motos del Ala de Cuervo (también el de Línea) son ahora **una única entrada compartida** con coste, perfil, «Despliegue Rápido» y todas las opciones de arma, así que cualquier cambio en sus armas o costes se aplica a las tres unidades. Cada unidad conserva sus propios límites: de 1 a 5 en el Escuadrón de Apoyo y uno solo (oculto hasta 6 miniaturas) en las motos.
- Se conservan las opciones propias de AO: Apotecario (+15), Estandarte del Ala de Cuervo (+25) y baliza de teleportación.

### Ángeles Oscuros — Escuadra de Devastadores igual a la de Marines Espaciales (revisión 2)

- **Escuadra de Devastadores** (modificada, Apoyo Pesado): misma estructura y costes que la de ME. Marine Espacial +15 → **+16**, Sargento +30 → **+26** y lanzamisiles +20 → **+15** (el mínimo sigue en 90 pts). Resto de armas pesadas sin cambios (bólter pesado y cañón de fusión +15, cañón de plasma +25, cañón láser +35).
- **Sargento:** un único grupo de armas, como en ME (bólter y pistola bólter por defecto, espada sierra, bólter de asalto +10, combifusión, combilanzallamas y combiplasma +10, arma de energía +15, pistola de plasma +15, puño de combate +25) y **Signum** como equipo fijo, igual que en ME. Se mantiene el arma de energía de AO en lugar de la espada de energía de ME.
- Los transportes asignados (cápsula +35, Rhino +35, Razorback +40) ya coincidían con ME. No se añade la regla «Tácticas de Combate», propia del codex de ME.

### Ángeles Oscuros — vehículos de Apoyo Pesado con el equipo y los puntos de Marines Espaciales (revisión 2)

- **Land Raider, Land Raider Cruzado, Predator, Vindicator y Whirlwind** (modificados): el grupo de equipo opcional pasa a ser el de ME. El **misil cazador asesino baja de +15 a +10** y el «bólter de asalto en afuste exterior» (+5) se sustituye por el **bólter de asalto (+10)** de ME. El blindaje adicional (+15) y la pala excavadora (+5, solo en Predator, Vindicator y Whirlwind) no cambian.
- **Vindicator** 125 → **115** pts, como en ME. El **Predator** se queda en 70 pts.
- **Vindicator y Predator:** ganan un **bólter de asalto adicional** (+10) además del que llevan de serie (el Predator lo lleva ahora de serie). El Vindicator gana además el **escudo de asedio** (+10).
- **Land Raider:** capacidad **10 → 12** miniaturas (las de armadura de exterminador siguen contando como dos; el Cruzado ya tenía 16) y **cañón de fusión opcional (+10)**. El Land Raider Cruzado ya lleva un cañón de fusión de serie, así que no se le añade otro.
- **Armas sin tocar:** se mantienen los costes de las armas de AO (cañón láser acoplado del Predator +35, etc.).
- No se añade el Hermano-Sargento Chronus de ME.

### Sistema de juego propio (2026-11-27)

- El `.gst` pasa a llamarse **«Warhammer 40,000 5ª Edición Ampliada»** (fichero `Warhammer 40,000 5ª Edición Ampliada.gst`), con descripción propia y un `id` nuevo (`310af520-2d8e-4c1d-b969-d49b4f3ad0f9`). Los 16 catálogos apuntan a ese `gameSystemId`.
- Así el sistema no se confunde con el de `wh40k-5ed` (antes compartían el id `8cf6-c83d-3eeb-e95c`). El contenido de reglas y perfiles del sistema no cambia; las revisiones del `.gst` y de los catálogos no cambian por este motivo.
