# Aleunda · Mundo 1: El Bosque Sagrado

Un juego de plataformas 3D por mundos, al estilo de los clásicos del género, con temática celta. Aleunda recorre el Bosque Sagrado con Lúa, un hada compañera, para devolver la luz a los anillos de hadas que apagó la Banshee.

Todo el juego vive en un solo archivo, [`index.html`](index.html): el 3D está hecho a mano con WebGL, la música y los sonidos se sintetizan con Web Audio, y no usa librerías, imágenes ni audio externos.

## Cómo abrirlo

- **Lo más fácil:** abre `index.html` con doble clic en un navegador reciente (Chrome, Edge, Firefox o Safari) con WebGL activado.
- **Con un servidor local** (útil para probar cambios):

  ```bash
  python3 -m http.server 8000
  ```

  y abre <http://localhost:8000>.

El sonido empieza con la primera tecla que pulses, porque los navegadores no dejan que una página suene sola.

El progreso se guarda en el navegador (`localStorage`). Cada navegador y cada dirección tienen su propia partida: abrir el archivo con doble clic y abrirlo por `localhost` son partidas distintas.

## Controles

### Dentro de un nivel

| Acción | Teclado | Mando |
|---|---|---|
| Moverse | Flechas o WASD | Stick izquierdo o cruceta |
| Saltar (mantén para llegar más alto) | Espacio, K o Z | A |
| Correr (mantén) | Shift o L | RB o RT |
| Voltereta (en el aire da un impulso hacia arriba, una vez por salto) | J o X | X o B |
| Pausa | P, Esc o Enter | Start |
| Volver al mapa (desde la pausa) | M | Select |
| Avanzar un diálogo | Enter o Espacio | A |

### En el mapa del mundo

| Acción | Teclado | Mando |
|---|---|---|
| Elegir camino | Flechas o WASD | Stick o cruceta |
| Entrar al nivel o asomarse al pozo | Enter o Espacio | A |
| Abrir la bolsa de objetos | B o I | Y |
| Cambiar de capucha | V | LB |
| Volver a la portada | Esc | — |

En la portada, **Enter** empieza o continúa la partida y **N** la borra para empezar de cero.

## De qué va

La Banshee apagó los anillos de hadas del Bosque Sagrado y hechizó a los púcas, unas liebres negras de ojos dorados. Lúa despierta a Aleunda para recuperar la luz: las setas luminosas y los trisqueles dorados guardan la luz robada. Al final del mundo espera el Gran Púca, el antiguo guardián del bosque, con una corona de espinas en la cabeza.

## Cómo funciona un nivel

- **La meta** es un menhir alto con un estandarte. Hay que tocarlo antes de que amanezca: hay 300 segundos, o 200 en el nivel secreto. Cuanto más alto lo toques, más puntos (arriba del todo, vida extra), y el tiempo que sobra se suma a los puntos.
- **Tréboles:** Aleunda aguanta 3 golpes. Algunas runas sueltan un trébol que recupera uno. Con el último trébol, la música se apaga como oída desde lejos y suena un latido.
- **Vidas:** se empieza con 5. Se pierde una al quedarse sin tréboles, al caer al vacío o al agua, o si se acaba el tiempo. Cada 100 setas dan una vida, igual que las bellotas doradas. Sin vidas se vuelve al mapa, pero el progreso queda guardado.
- **Lúa al rescate:** en el 1-1, en el 1-2 y en el claro secreto, tras una caída, Lúa devuelve a Aleunda al último suelo firme a cambio de un trébol. Solo se pierde la vida si ya no quedaba más que uno.
- **Menhir de control:** a mitad de nivel. Al tocarlo se enciende y, si pierdes una vida, vuelves a empezar desde ahí.
- **Carteles de consejo:** postes de madera que brillan hasta que los lees. Al acercarte muestran una pista. El 1-1 los usa como tutorial.

### Enemigos y objetos

| | Qué es | Qué hacer |
|---|---|---|
| **Púca** | Liebre negra hechizada que patrulla y, si te ve, te persigue un momento. Algunos esperan bajo tierra. En el 1-1 solo pasean. | Pisarla o darle una voltereta. Si encadenas pisotones sin tocar el suelo, los puntos se duplican, y al sexto ganas una vida. |
| **Fuego fatuo** | Luz azul que patrulla en línea o en círculo. | No se puede vencer: hay que esquivarlo. |
| **Runa** | Bloque de piedra con marcas que brillan. | Golpéala con la cabeza, saltando desde abajo: suelta setas, un trébol o una bellota dorada. |
| **Seta gigante** | Seta violeta enorme. | Rebota muy alto; si mantienes el salto, sube más. |
| **Plataformas** | Troncos y losas que se mueven, maderas y hojas que se hunden poco después de pisarlas, cestas colgantes. | Calcula el momento y no te quedes encima de las que se hunden. |

## El mapa del mundo

El mapa es una isla flotante con caminos de piedras. Para seguir más allá de un nivel hay que completarlo. Los caminos nuevos aparecen piedra a piedra, y unas flechitas doradas junto a Aleunda señalan los que están abiertos.

- **Elegir ruta:** después del 1-1 el camino se divide. El arroyo (1-2) y las copas (1-3) llevan al dolmen del jefe (1-4): basta con completar uno de los dos.
- **Pozo de los deseos:** el primer deseo es gratis y los siguientes cuestan 30 setas. Cada deseo da un objeto para la bolsa. Como las setas también dan vidas, gastarlas es una decisión.
- **Bolsa (hasta 4 objetos):** antes de entrar a un nivel preparas uno, que dura todo el nivel aunque pierdas una vida.
  - **Trébol de cuatro hojas:** aguantas 4 golpes en vez de 3.
  - **Pluma de hada:** doble salto (pulsa Espacio otra vez en el aire).
  - **Farolillo de las hadas:** una estela de luz te lleva al trisquel más cercano que te falta.
- **Puerta de piedra:** se abre al reunir 5 trisqueles dorados y lleva al claro secreto 1-S.
- **El mundo despierta:** cada nivel completado enciende un anillo de luces doradas en el mapa, el cielo de la isla se acerca al amanecer y la música del mapa suma instrumentos.

## Los niveles

| Nivel | Nombre | Qué tiene |
|---|---|---|
| 1-1 | El claro de los robles | Tutorial con carteles, púcas tranquilos, runas, escalera de piedras, una seta gigante y una noche de luna. |
| 1-2 | El arroyo de niebla | Vado de piedras, troncos que van y vienen, maderas que se hunden, losas que suben y bajan, y fuegos fatuos. |
| 1-3 | Las copas de los robles | Saltos de copa en copa al amanecer, hojas secas que caen, cestas colgantes y un tronco gigante que se trepa por hongos repisa. Aquí Lúa ya no rescata. |
| 1-4 | El dolmen del Gran Púca | Camino de menhires bajo la tormenta, púcas emboscados, piedras que se derrumban y la pelea contra el jefe. |
| 1-S | El anillo de las hadas | Nivel secreto de regalo, tras la puerta de piedra: muchas setas, rebotes encadenados y runas generosas. |

**El jefe:** el Gran Púca salta hacia Aleunda y al caer lanza ondas expansivas que hay que saltar. Después de sus saltos queda mareado: ese es el momento de saltarle a la cabeza. Con tres pisotones se rompe el hechizo y vuelve a ser una liebre blanca y buena.

## Secretos y coleccionables

- **Setas luminosas:** 10 puntos cada una; 100 setas dan una vida.
- **Trisqueles dorados:** 3 escondidos en cada nivel, 15 en total. Quedan guardados y abren la puerta de piedra.
- **Caminos de hadas:** losas invisibles que aparecen cuando Aleunda se acerca. Antes se delatan con destellos verdes en el aire. Cada nivel tiene uno que lleva a una zona secreta.
- **Runas escondidas:** bloques invisibles que se atraviesan desde arriba y aparecen al golpearlos desde abajo. Hay una por nivel.
- **Bellotas de plata:** una al final de cada camino de hadas, 5 en total.
- **Capuchas:** con 2 bellotas de plata ganas la capucha de otoño, con 4 la de la noche y con las 5 la dorada, que deja chispas. Se cambian con **V** en el mapa.

## La historia

Lúa vuela siempre junto a Aleunda, ilumina el camino y comenta lo que pasa: el primer pisotón, un trisquel, el último trébol, el amanecer o la meta a la vista. Entre niveles hay escenas cortas con retratos y texto que aparece letra a letra: el prólogo, el camino que se divide, la puerta abierta, la llegada al jefe y el final. Cada escena se ve una sola vez y queda guardada. Al vencer al Gran Púca, la tormenta se convierte en amanecer y queda abierto el camino hacia el Mundo 2, que todavía no existe.

## Para modificar el juego

### Cómo está organizado `index.html`

El script está dividido en secciones con títulos en mayúsculas:

| Sección | Qué hay |
|---|---|
| Constantes de ajuste | Todo lo que se puede tocar sin programar (ver más abajo). |
| Utilidades y matemática 3D | Colores, números aleatorios repetibles y matrices 4x4. |
| WebGL | Shaders, el constructor de mallas (`Malla`: cajas, cilindros, esferas…) y los sprites que brillan. |
| Modelos 3D | Aleunda, púcas, Lúa, setas, runas y el resto de modelos, todos hechos con formas básicas. |
| Sonido | Instrumentos sintetizados (arpa, flauta, bajo, tambor, campana), las canciones y los efectos. |
| Entrada | Teclado y mando. |
| Progreso guardado | Lo que se guarda en `localStorage` y las capuchas. |
| Decorado y construcción de niveles | Árboles, menhires, dólmenes… y las funciones `L.*` para montar niveles. |
| Mundo 1 | La lista `NIVELES` con los cinco niveles. |
| Física y juego | Aleunda, colisiones, enemigos, jefe, historia de Lúa, interacciones y cámara. |
| Render 3D | Ambientes de cada nivel, luces, sombras y dibujo de la escena. |
| Mapa del mundo | Nodos, caminos, pozo, bolsa y puerta. |
| HUD | La interfaz en 2D: paneles, bocadillos, diálogos y retratos. |
| Escenas y bucle principal | Portada, mapa, intro, juego, final y fin de partida. |

### Constantes de ajuste

Al principio del script hay grupos de constantes comentadas. Por ejemplo:

- **Movimiento:** `VEL_CAMINAR`, `VEL_CORRER`, `SALTO_VEL`, `GRAVEDAD`, `COYOTE`, `BUFFER_SALTO`.
- **Partida:** `VIDAS_INICIALES`, `CORAZONES_MAX`, `SETAS_POR_VIDA`, `RESCATE_EN_CAIDAS`, `PUCAS_TRANQUILOS`.
- **Mapa:** `TRISQUELES_PUERTA`, `COSTE_DESEO`, `BOLSA_MAX`.
- **Jefe:** `JEFE_VIDA`, `JEFE_SALTO_TIEMPO`, `JEFE_ATURDIDO`.
- **Aspecto de Aleunda:** `PELO_RAIZ`, `PELO_PUNTA`, `PELO_LARGO`, `PELO_RIZO` y el balanceo de pelo, capa y capucha (`BALANCEO_*`).
- **Cámara y sonido:** `CAMARA_DISTANCIA`, `CAMARA_ALTURA`, `VOLUMEN`, `VOLUMEN_MUSICA`.

### Crear o cambiar un nivel

Cada nivel de `NIVELES` tiene un nombre, un tiempo, un ambiente de cielo y niebla (`noche`, `niebla`, `alba`, `tormenta` o `hadas`), una música (`bosque`, `arroyo`, `copas`, `dolmen`, `jefe` o `hadas`) y una función `construir(L)` que coloca las piezas.

Las coordenadas son: `x` hacia los lados (positivo a la derecha), `y` hacia arriba y `d` la distancia hacia delante desde la salida.

```js
{
  id: '1-5', nombre: 'Mi nivel', tiempo: 300, ambiente: 'noche', musica: 'bosque', semilla: 99,
  consejo: 'Texto que sale en la tarjeta de entrada',
  construir(L) {
    L.inicio(0, 0);                                        // salida en x=0, d=0
    L.tierra(-4.5, 4.5, -8, 40);                           // camino de x=-4.5 a 4.5, de d=-8 a d=40
    L.fila(0, 5, 0, 15, 0.7, 6);                           // 6 setas en fila
    L.puca(0, 20, 0, { x0: -3, x1: 3, d0: 19, d1: 21 });   // púca que patrulla esa zona
    L.trisquel(2, 3, 25); L.trisquel(-3, 2, 30); L.trisquel(0, 5, 33);
    L.meta(0, 36);
    L.bosque(-10, 50);                                     // siempre al final: rellena los lados con robles
  },
},
```

Algunas piezas disponibles:

- **Suelos y plataformas:** `L.tierra`, `L.piedra`, `L.losa`, `L.columna`, `L.copa`, `L.rama`, `L.repisa`, `L.isla`, `L.movil` (se mueve), `L.cae` (se hunde al pisarla), `L.caminoHadas` (invisible hasta que Aleunda se acerca).
- **Objetos:** `L.seta`, `L.fila`, `L.arco`, `L.anillo`, `L.columnaSetas`, `L.trisquel` (3 por nivel), `L.bellotaPlata`, `L.runa` (con `true` al final queda escondida), `L.muelle`.
- **Enemigos:** `L.puca` (en modo normal o `'emboscada'`), `L.fatuo` (en círculo o en línea), `L.arena` y `L.jefe`.
- **Hitos:** `L.inicio`, `L.control`, `L.meta`, `L.cartel`.
- **Decorado:** `L.roble`, `L.bosque`, `L.menhir`, `L.dolmen`, `L.setasDeco`, `L.farol`, `L.agua`, `L.juncos`, `L.nenufares`, `L.troncoGigante`.

Para que un nivel nuevo aparezca en el mapa, añade su nodo en `NODOS`, su camino en `ARISTAS` y sube `NUM_NIVELES`. También puedes darle una frase de Lúa en `LUA_NIVEL`.

### Documentos del proyecto

- [`docs/diseno.md`](docs/diseno.md): el diseño completo (personajes, mundo, estrategia, historia, secretos) y la bitácora de versiones.
- [`CLAUDE.md`](CLAUDE.md): las reglas de trabajo del proyecto.

## Tecnología

- **3D:** WebGL 1 escrito a mano, sin three.js ni otras librerías. Estilo low-poly con sombreado plano, las ocho luces puntuales más cercanas, niebla de distancia y niebla baja, cielo con estrellas y luna, sombras de mancha bajo los personajes y sprites que brillan para luces y partículas. Si el decorado tapa a Aleunda, se ve su silueta a través de él, y lo que roza la cámara se desvanece.
- **Sonido:** Web Audio. Instrumentos sintetizados, un secuenciador para la música de cada nivel y efectos generados en el momento.
- **Física:** pasos fijos de 120 por segundo, con tiempo de coyote, memoria del botón de salto, salto de altura variable y colisiones contra cajas y cilindros.
- **Guardado:** `localStorage`, con niveles completados, trisqueles, bellotas de plata, objetos de la bolsa, capucha y escenas vistas.
