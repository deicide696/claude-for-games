# Diseño: El gnomo y el anillo de hadas

## Los seis ingredientes

- **Concepto:** un gnomo celta recoge setas luminosas de los anillos de hadas antes de que amanezca.
- **Core loop:** el jugador se mueve y recoge setas para llenar su caldero, mientras esquiva púcas y fuegos fatuos.
- **Controles:** flechas o WASD para moverse, Espacio para una voltereta corta.
- **Ganar y perder:** gana con 20 setas antes de 90 segundos. Pierde con 3 golpes o si se acaba el tiempo.
- **Estética:** pixel art dibujado en código, bosque celta con niebla, paleta de verdes, dorado y azul noche, sonidos generados en código.
- **Restricciones:** un solo archivo HTML, sin librerías ni imágenes externas.

## Personajes

- **Gnomo (jugador):** capa verde con capucha, barba pelirroja trenzada, torque dorado al cuello y un pequeño caldero donde guarda las setas.
- **Púca (enemigo):** espíritu cambiaformas con forma de liebre negra de ojos dorados. Sale de la tierra junto a las piedras, persigue un momento y se esconde.
- **Fuego fatuo (enemigo):** luz azul que flota en patrulla lenta y deja estela. No persigue, pero bloquea caminos.
- **Banshee (evento):** aparece en los últimos 20 segundos; su lamento avisa que amanece y acelera a los enemigos.

## Escenario

- Claro de bosque rodeado de robles, con menhires y un dolmen en el centro.
- Las setas brotan en círculos (anillos de hadas), no sueltas.
- Trisqueles y nudos celtas tallados en las piedras y en el borde de la interfaz.
- Niebla baja que se aclara a medida que se acerca el amanecer.

## Prompt inicial

Crea un juego de acción y recolección con vista desde arriba en un solo archivo HTML,
sin librerías ni imágenes externas.
Concepto: un gnomo celta recoge setas luminosas de los anillos de hadas antes de que amanezca.
Core loop: el jugador se mueve y recoge setas para llenar su caldero
mientras esquiva púcas que salen de la tierra y fuegos fatuos que patrullan.
Personajes y escenario: sigue las secciones "Personajes" y "Escenario" de este documento.
Controles: flechas o WASD para moverse, Espacio para una voltereta corta.
Gana si recoge 20 setas antes de 90 segundos. Pierde si recibe 3 golpes o se acaba el tiempo.
Estilo: pixel art, bosque celta con niebla, paleta de verdes, dorado y azul noche.
Sonidos generados en código, con melodía tipo arpa en escala pentatónica.
Game feel: screen shake, partículas y easing en el movimiento.
Incluye pantalla de inicio, puntaje y reinicio rápido.
Pon las constantes de ajuste (velocidad, tiempos, cantidades) juntas al inicio del código, con comentarios.

## Bitácora

| Versión | Qué cambié | Qué aprendí |
|---|---|---|
| v0 | | |
