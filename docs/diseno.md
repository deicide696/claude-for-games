# Diseño: AleUnda y el Bosque Sagrado

## Los seis ingredientes

- **Concepto:** AleUnda cruza el Bosque Sagrado recogiendo setas luminosas y trisqueles dorados hasta liberar el primer anillo de hadas del Gran Púca.
- **Core loop:** correr, saltar y pisar enemigos por niveles en 3D; llegar al menhir de la meta antes de que amanezca y desbloquear el siguiente nivel en el mapa del mundo.
- **Formato:** por mundos, al estilo de los plataformas clásicos. Cada mundo tiene un mapa con su camino y cuatro niveles; el último es un jefe.
- **Controles:** flechas o WASD para moverse, Espacio para saltar (mantenerlo salta más alto), Shift para correr, J o X para una voltereta (vence púcas y en el aire da un pequeño impulso), P o Esc para pausar. También funciona con mando.
- **Ganar y perder:** se gana un nivel al tocar el menhir de la meta (cuanto más alto, más puntos). AleUnda aguanta 3 golpes (tréboles); caer al vacío, al agua o quedarse sin tiempo cuesta una vida. Cada 100 setas, una vida extra.
- **Estética:** 3D low-poly dibujado en código con WebGL, bosque celta de noche con niebla, paleta de verdes, dorado y azul noche; música de arpa, flauta y bodhrán generada en código.
- **Restricciones:** un solo archivo HTML, sin librerías ni imágenes ni audio externos.

## Personajes

- **AleUnda (protagonista):** capucha verde puntiaguda con un cascabel dorado, trenzas pelirrojas, torque dorado al cuello y un pequeño caldero en la cadera donde guarda las setas.
- **Púca (enemigo):** liebre negra de ojos dorados. Patrulla su zona y, si ve a AleUnda, la persigue un momento. Algunos esperan escondidos bajo tierra y salen de golpe. Se vencen pisándolos o con la voltereta.
- **Fuego fatuo (enemigo):** luz azul que patrulla en línea o en círculo y deja estela. No se puede vencer: hay que esquivarlo.
- **El Gran Púca (jefe del Mundo 1):** un púca gigante con corona de espinas. Salta sobre AleUnda y al caer lanza ondas expansivas que hay que saltar. Tras sus saltos queda mareado: es el momento de pisarle la cabeza. Tres pisotones lo vencen.
- **La Banshee:** huye al final del Mundo 1 y anuncia el Mundo 2.

## Mundo 1: El Bosque Sagrado

- **Mapa:** isla flotante con la casa redonda de AleUnda, un río con puente y cuatro piedras de nivel unidas por caminos. Los niveles se abren al completar el anterior.
- **1-1 El claro de los robles (noche):** tutorial. Runas, púcas, escalera de piedras, una seta gigante saltarina y un menhir de control a mitad de camino.
- **1-2 El arroyo de niebla (niebla):** piedras sobre el agua, troncos que van y vienen, maderas que se hunden, losas que suben y bajan y fuegos fatuos.
- **1-3 Las copas de los robles (alba):** se salta de copa en copa, hojas secas que caen al pisarlas, cestas colgantes y un tronco gigante que se trepa por hongos repisa.
- **1-4 El dolmen del Gran Púca (tormenta):** camino de menhires con relámpagos, púcas emboscados, piedras que se derrumban sobre el abismo y la arena del jefe.

## Objetos

- **Seta luminosa:** 10 puntos; 100 setas dan una vida.
- **Trisquel dorado:** 3 escondidos por nivel (12 en el mundo); quedan guardados.
- **Runa:** bloque de piedra con marcas ogham que se golpea desde abajo; suelta setas, un trébol (recupera un golpe) o una bellota dorada (vida extra).
- **Seta gigante:** rebota muy alto.
- **Menhir de control:** si AleUnda cae, vuelve a empezar desde ahí.
- **Menhir de la meta:** al tocarlo sube el estandarte; el tiempo que sobra se suma a los puntos.

## Escenario

- Caminos de tierra flotando sobre un mar de niebla, con robles altísimos que nacen de abajo.
- Anillos de hadas: setas en círculo con florecitas que brillan entre ellas.
- Trisqueles y marcas ogham talladas en las piedras y en la interfaz.
- La niebla baja se espesa en las zonas hondas; cada nivel tiene su propio cielo y su música.

## Prompt de esta versión

Convierte el juego en 3D (WebGL puro, sin librerías) con formato de mundos al estilo de los plataformas clásicos.
La protagonista es AleUnda. Crea el Mundo 1 completo: mapa del mundo con caminos y cuatro niveles,
el último con jefe. Mantén la temática celta (setas, púcas, fuegos fatuos) y que todo viva en index.html.

## Bitácora

| Versión | Qué cambié | Qué aprendí |
|---|---|---|
| v0 | Recolección vista desde arriba y luego en vista lateral, con el gnomo | |
| v1 | Salto a 3D: AleUnda, mapa del Mundo 1, cuatro niveles y jefe | |
