# Diseño: Aleunda y el Bosque Sagrado

## Los seis ingredientes

- **Concepto:** Aleunda cruza el Bosque Sagrado recogiendo setas luminosas y trisqueles dorados hasta liberar el primer anillo de hadas del Gran Púca.
- **Core loop:** correr, saltar y pisar enemigos por niveles en 3D; llegar al menhir de la meta antes de que amanezca y desbloquear el siguiente nivel en el mapa del mundo.
- **Formato:** por mundos, al estilo de los plataformas clásicos. Cada mundo tiene un mapa con caminos que se bifurcan, niveles, un jefe y algún secreto.
- **Controles:** flechas o WASD para moverse, Espacio para saltar (mantenerlo salta más alto), Shift para correr, J o X para una voltereta (vence púcas y en el aire da un pequeño impulso), P o Esc para pausar. También funciona con mando.
- **Ganar y perder:** se gana un nivel al tocar el menhir de la meta (cuanto más alto, más puntos). Aleunda aguanta 3 golpes (tréboles); caer al vacío, al agua o quedarse sin tiempo cuesta una vida. Cada 100 setas, una vida extra.
- **Curva de dificultad:** el comienzo es amable. En 1-1 y 1-2, tras una caída, las hadas devuelven a Aleunda al último suelo firme a cambio de un trébol (solo se pierde la vida con el último trébol). En 1-1 los púcas pasean sin perseguir. Desde 1-3 ya no hay rescate.
- **Estética:** 3D low-poly dibujado en código con WebGL, bosque celta de noche con niebla, paleta de verdes, dorado y azul noche; música de arpa, flauta y bodhrán generada en código.
- **Restricciones:** un solo archivo HTML, sin librerías ni imágenes ni audio externos.

## Personajes

- **Aleunda (protagonista):** capucha verde puntiaguda con un cascabel dorado, pelo largo, suelto y rizado (castaño en la raíz y miel en las puntas, con raya al medio), torque dorado al cuello y un pequeño caldero en la cadera donde guarda las setas.
- **Lúa (hada compañera):** hadita de luz con alas de libélula y vestido de hoja. Vuela siempre junto a Aleunda e ilumina el camino como un farolillo. Comenta lo que pasa en bocadillos azules (el primer pisotón, el primer trisquel, el último trébol, el amanecer, la meta a la vista…), rescata a Aleunda en las caídas de los primeros niveles y cuenta la historia en las escenas.
- **Púca (enemigo):** liebre negra de ojos dorados. Patrulla su zona y, si ve a Aleunda, sale a perseguir un momento. Algunos esperan escondidos bajo tierra y salen de golpe. Se vencen pisándolos o con la voltereta.
- **Fuego fatuo (enemigo):** luz azul que patrulla en línea o en círculo y deja estela. No se puede vencer: hay que esquivarlo.
- **El Gran Púca (jefe del Mundo 1):** un púca gigante con corona de espinas. Salta sobre Aleunda y al caer lanza ondas expansivas que hay que saltar. Tras sus saltos queda mareado: es el momento de pisarle la cabeza. Tres pisotones rompen el hechizo: la corona se quiebra y vuelve a ser una liebre blanca y buena, el antiguo guardián del bosque.
- **Los púcas hechizados:** no son malos, la Banshee los hechizó. Al vencerlos sale de ellos una lucecita blanca: su espíritu liberado.
- **La Banshee:** huye al final del Mundo 1 y anuncia el Mundo 2.

## Mundo 1: El Bosque Sagrado

- **Mapa:** isla flotante con la casa redonda de Aleunda, un río con puentes y siete nodos unidos por caminos de piedras. Las flechas eligen camino (unas flechitas doradas señalan los que están abiertos) y los caminos nuevos aparecen piedra a piedra.
- **1-1 El claro de los robles (noche):** tutorial guiado por carteles. Runas, púcas tranquilos, un primer hueco corto, escalera de piedras, una seta gigante saltarina y un menhir de control a mitad de camino.
- **1-2 El arroyo de niebla (niebla):** un vado de piedras anchas y fáciles, troncos gruesos que van y vienen despacio, maderas que se hunden, losas que suben y bajan y fuegos fatuos.
- **1-3 Las copas de los robles (alba):** se salta de copa en copa, hojas secas que caen al pisarlas, cestas colgantes y un tronco gigante que se trepa por hongos repisa.
- **1-4 El dolmen del Gran Púca (tormenta):** camino de menhires con relámpagos, púcas emboscados, piedras que se derrumban sobre el abismo y la arena del jefe.
- **1-S El anillo de las hadas (claro secreto):** nivel de regalo tras la puerta de piedra. Un gran anillo de setas, islitas encadenadas con setas gigantes, runas generosas y tres trisqueles; las hadas rescatan en las caídas.

## Estrategia en el mapa

- **Elegir ruta:** al completar el 1-1 el camino se abre en tres. El arroyo (1-2) y las copas (1-3) llevan los dos al dolmen del jefe (1-4): basta con uno, pero cada ruta tiene sus trisqueles.
- **Puerta de piedra:** desde el pozo sale un camino que se cierra con una puerta. Se abre al reunir 5 trisqueles dorados y lleva al claro secreto 1-S. Repetir niveles para buscar trisqueles vale la pena.
- **Pozo de los deseos:** el primer deseo es gratis; los demás cuestan 30 setas. Cada deseo da un objeto para la bolsa. Gastar setas en deseos significa conseguir menos vidas extra: hay que decidir.
- **Bolsa (tecla B):** caben 4 objetos. Antes de entrar a un nivel se prepara uno, que dura todo ese nivel (también tras perder una vida) y se gasta al volver al mapa.
  - **Trébol de cuatro hojas:** un trébol de más (4 golpes). Ideal para el jefe.
  - **Pluma de hada:** doble salto. Ayuda en el 1-3 y para alcanzar trisqueles altos.
  - **Farolillo de las hadas:** una estela de luz señala el trisquel más cercano que falta.

## Objetos

- **Seta luminosa:** 10 puntos; 100 setas dan una vida.
- **Trisquel dorado:** 3 escondidos por nivel (15 en el mundo, contando el claro secreto); quedan guardados y abren la puerta de piedra.
- **Runa:** bloque de piedra con marcas ogham que se golpea desde abajo; suelta setas, un trébol (recupera un golpe) o una bellota dorada (vida extra).
- **Seta gigante:** rebota muy alto.
- **Menhir de control:** si Aleunda pierde una vida, vuelve a empezar desde ahí.
- **Cartel de consejo:** poste de madera con runas que brilla mientras no se ha leído; al acercarse aparece un bocadillo con una pista. El 1-1 los usa como tutorial (moverse, runas, púcas, correr, trisqueles, control, setas gigantes, voltereta y meta).
- **Menhir de la meta:** al tocarlo sube el estandarte; el tiempo que sobra se suma a los puntos.

## Cosas por descubrir

- **Caminos de hadas:** losas invisibles que solo aparecen cuando Aleunda se acerca. Antes de verse, delatan su sitio con destellos verdes en el aire (y la sombra de Aleunda se posa sobre ellas). Cada nivel tiene uno que lleva a una zona secreta, y un cartel del 1-1 enseña a buscarlos.
- **Runas escondidas:** bloques invisibles que se atraviesan desde arriba y aparecen al golpearlos desde abajo. Hay una por nivel, con setas, un trébol o una bellota dorada, y de vez en cuando dejan un destello blanco.
- **Bellotas de plata:** una por nivel (5 en el mundo), al final de cada camino de hadas. Dan 2000 puntos, quedan guardadas y se ven en el HUD y en las etiquetas del mapa.
- **Capuchas (recompensa):** con 2 bellotas se gana la capucha de otoño, con 4 la de la noche y con las 5 la dorada, que deja chispas. Se cambian con la tecla V en el mapa y también cambian el retrato.
- Lúa celebra cada hallazgo y suena una melodía propia de «secreto descubierto».

## Historia y emoción

- **Escenas cortas** con franjas de cine, retratos y texto que aparece letra a letra (Enter o Espacio para seguir). Cada una se ve una sola vez y queda guardada:
  - **Prólogo** (al empezar): Lúa despierta a Aleunda; la Banshee apagó los anillos de hadas y hechizó a los púcas.
  - **Tras el 1-1:** el camino brilla otra vez; Lúa explica la bifurcación y el pozo.
  - **Tras el arroyo o las copas:** el bosque canta más fuerte; quién era el Gran Púca; la puerta de los cinco trisqueles.
  - **Puerta abierta:** detrás está el claro de la familia de Lúa.
  - **Jefe:** el Gran Púca ruge y Lúa explica cómo romper el hechizo.
  - **Final:** la liebre liberada da las gracias y cuenta adónde huyó la Banshee; Aleunda y Lúa deciden seguir el viaje hacia el Mundo 2, siempre en compañía.
- **Tarjeta de entrada:** antes de cada nivel, Lúa dice una frase sobre lo que viene.
- **El mundo despierta:** los niveles completados muestran en el mapa un anillo de luces doradas que gira, y el cielo de la isla se acerca al amanecer con cada nivel. En el final, la tormenta del dolmen se convierte en amanecer.
- **Música que reacciona:** la música del mapa gana instrumentos con el progreso (bajo tras el primer nivel, campanas tras el tercero); con un solo trébol la música se apaga como oída desde lejos y suena un latido; al tomar un trisquel la música se aparta para que se oiga el tesoro.

## Escenario

- Caminos de tierra flotando sobre un mar de niebla, con robles altísimos que nacen de abajo.
- Anillos de hadas: setas en círculo con florecitas que brillan entre ellas.
- Trisqueles y marcas ogham talladas en las piedras y en la interfaz.
- La niebla baja se espesa en las zonas hondas; cada nivel tiene su propio cielo y su música.

## Prompt de esta versión

Convierte el juego en 3D (WebGL puro, sin librerías) con formato de mundos al estilo de los plataformas clásicos.
Aleunda es quien protagoniza. Crea el Mundo 1 completo: mapa del mundo con caminos y cuatro niveles,
el último con jefe. Mantén la temática celta (setas, púcas, fuegos fatuos) y que todo viva en index.html.

## Bitácora

| Versión | Qué cambié | Qué aprendí |
|---|---|---|
| v0 | Recolección vista desde arriba y luego en vista lateral, con el gnomo | |
| v1 | Salto a 3D: Aleunda, mapa del Mundo 1, cuatro niveles y jefe | |
| v1.1 | Inicio más sencillo: carteles de consejo, rescate de las hadas en caídas (1-1 y 1-2), púcas tranquilos en 1-1, primer hueco más corto, vado del 1-2 fácil con teclado | |
| v1.2 | Mapa estratégico: caminos que se bifurcan (arroyo o copas), pozo de los deseos, bolsa con tres objetos, puerta de 5 trisqueles y claro secreto 1-S | |
| v1.3 | Más emocional: Lúa, el hada compañera; escenas de historia; púcas hechizados que se liberan; final al amanecer; mapa y música que reaccionan | |
| v1.4 | Cosas por descubrir: caminos de hadas invisibles, runas escondidas, una bellota de plata por nivel y capuchas nuevas como recompensa | |
