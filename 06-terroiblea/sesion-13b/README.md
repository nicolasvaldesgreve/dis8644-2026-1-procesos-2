# sesion-13b

Viernes 12 de Junio, 2026. 

Nota del día: llegué muy tarde.

## Referentes (y otras cosas)

- **John Cage** Fue un compositor, filósofo y artista estadounidense, una de las figuras más influyentes del siglo XX. Pionero de la música aleatoria, de la música electrónica y del uso no estándar de instrumentos musicales (como el piano preparado), su obra más famosa es *4′33″*, una pieza que consiste enteramente en el silencio ambiental del entorno, desafiando la definición misma de lo que constituye la música.
- **Steve Reich** Es un compositor estadounidense y uno de los máximos pioneros del minimalismo musical. Su trabajo introdujo el uso de bucles de cinta adhesiva con desfase (*phasing*) y procesos matemáticos repetitivos aplicados a la percusión y la instrumentación, transformando radicalmente la música contemporánea y sirviendo de base para géneros modernos como el ambiente y la electrónica.
- **Yoko Ono** es una artista conceptual, música y activista multimedia japonesa, figura clave en el desarrollo del movimiento vanguardista *Fluxus* en la década de 1960. Su enfoque artístico prioriza la idea o la instrucción por sobre el objeto físico, integrando la música experimental, la performance participativa y el cripticismo poético mucho antes de su salto a la cultura popular masiva.
- **Pendulum Music** Es una célebre pieza conceptual creada por Steve Reich en 1968. La obra es una escultura sonora procesual que consiste en suspender varios micrófonos sobre unos parlantes; al ser soltados como péndulos, el movimiento genera acoples de retroalimentación (*feedback*audibles cada vez que pasan cerca del cono del parlante, creando un ritmo orgánico que se detiene por completo una vez que la gravedad detiene los micrófonos.
- **Lindsay Ellis** Es una crítica de cine, ensayista audiovisual y novelista estadounidense, conocida por su influyente trayectoria en YouTube analizando narrativa, cultura pop y medios de comunicación. En su video ensayo sobre Yoko Ono (*"Yoko Ono: El Arte del Insulto"*), realiza una profunda deconstrucción crítica de la misoginia, el racismo y la incomprensión pública que sufrió la artista conceptual, reevaluando su verdadero impacto e innovación en el arte contemporáneo. - <https://youtu.be/SMOABV_zgrk>
- **Manfred Werder** es un compositor y performer suizo fuertemente vinculado al colectivo internacional de música experimental *Wandelweiser*. Su obra explora los límites del minimalismo extremo, el silencio y la ecología acústica, reduciendo a menudo sus partituras a frases poéticas breves o citas literarias que invitan al intérprete a simplemente registrar, activar o escuchar los sonidos naturales que ya existen en el espacio público.

## Qué aprendí hoy

### Partituras 

¿Qué es una partitura?

- Una partitura es un documento escrito, impreso o digital que representa gráficamente una composición musical. Funciona como una especie de "mapa" o "guía" para los músicos, utilizando un sistema de notación universal con signos, símbolos y notas que detallan exactamente qué tocar y cómo hacerlo. (wikipedia)

Para el desarrollo del proyecto 03 hay que pensar fuera de lo que convencionalmente se conoce como partitura ya que hay muchas formas de escribir la música (para todo lenguaje, hay variaciones): 

Puede ser representado como: 

- instrucciones. 
- dibujos.
- reglas.
- palabras.
- sonidos.
- entre otros. 

Partitura general como un sistema completo (pero recordar: **todo sistema tiene un límite**!!)

![referentes partituras](./imagenes/referentes.png)

## Qué hice hoy

Avance proyecto 03. 

Primero terminamos de definir que placas vamos a utilizar para desarrollar nuestro sintetizador. 

- Barry benson (Abeja) - percutor.  
- Lub-dub (Corazón) - percutor. 
- Chirihue Mecanizado (Pájaro) - oscilador. (<https://github.com/terroiblea/dis8644-2026-1-procesos-2/tree/main/00-proyecto-02/grupo-04>)     

La idea es generar una especie de ecosistema (abeja + pájaro), por lo mismo todo suena superpuesto (sonidos independientes).

Para unir todo utilizaríamos más o menos un sistema así: (considerando partes de unión y partes que se manejan de forma externa cuando este la carcasa)

![unión pcb](./imagenes/union.png)

El próximo martes podrían llegar las placas (yeih), así que de momento tenemos que pensar en las otras partes del proyecto hasta que podamos soldar. Por lo mismo, ahora comenzamos con el desarrollo del BOM, tomando como base el que ya habíamos realizado en el proyecto 02.

De momento va algo así: 

| Componente | Cantidad | Precio (c/u) | Comprar |
|------------|----------|--------------|---------|
| Chip 4069UBE | 1 | $1.100 | <https://www.cabezacuadrada.cl/product/cd4069/> |
| Chip CD40106BE | 3 | $750 | <https://www.cabezacuadrada.cl/product/cd40106be/> |
| Chip LM324 | 1 | | | |
| Potenciómetro 100K | 8 | $490 | <https://www.mechatronicstore.cl/potenciometro-rotacional-10k/> |
| Potenciómetro 250K | 4 | $495 | <https://altronics.cl/potenciometro-lineal-250k-b250k> |
| Capacitor no polarizado 100nF | 6 | $100 | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/> |
| Capacitor no polarizado 10nF | 1 | $100 | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/> |
| Capacitor polarizado 10uF 50V | 6 | $100 | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> |
| Capacitor polarizado 0.22uF 50V | 1 | $100 | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> |
| Capacitor polarizado 100uF 50V | 4 | $100 | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> |
| Capacitor polarizado 1uF 50V | 1 | $100 | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> |
| Resistencia 100K | 1 | $100 | <https://www.mechatronicstore.cl/resistencias-electricas-1-2-w-1-unidad/> |
| Resistencia 1K | 4+5* | $200 | <https://www.mechatronicstore.cl/resistencias-electricas-3w-por-unidad/> |
| Diodo 1N4007 | 2 | $200 | <https://www.mechatronicstore.cl/diodo-rectificador-in4007-1n4007-4007/> |
| LED 3mm/5mm | 5 | $100 | <https://www.mechatronicstore.cl/led-3mm-5mm/> |
| Regulador de voltaje L7805 | 2 | $490 | <https://www.mechatronicstore.cl/regulador-limitador-de-voltaje-5v-dc/> |
| Chip CD4070BE | 1 | - | <https://www.mouser.cl/ProductDetail/Texas-Instruments/CD4070BE?qs=5WY7Uqh921w5Ya0dPgjorQ%3D%3D> |
| Barrel Jack Switch | 6 | — | Extraídos del LID |
| Switch 2 pines, 2 posiciones | 2 | $570 | <https://www.katode.cl/switches/1339-interruptor-switch-2-pines-on-off-corto.html> |

### Ideas generales de partituras desarrolladas hasta el momento: 

**Partitura 1:** instrucciones escritas. 

(desarrollo idea general)

- 08:00 a 12:00: El pajarito canta rapido pero volumen bajo , la abeja esta rapida pero suena bajito, y el corazón está rápido.
- 12:01 a 16:00: pajarito full, abeja más lenta pero suena más fuerte, y el corazón más lento.
- 16:01 a las 20:00: El pajarito canta lento y bajo volumen, la abeja muy lenta pero harto volumen, el corazón harto volumen pero más lento.
- 20:01 a las 07:59: Pajarito no canta, abeja en silencio y corazón muy lento y volumen un poco más bajo.

**Partitura 2:** diagrama/dibujo. 

- El corazón son puntos (un latido es como un golpe repetitivo, diagramarlo serían como puntos/los golpes representados), la abeja es un camino curvado con línea discontinua, el pajaro todavía no sé cómo se podría diagramar pero de igual forma tendría su propio lenguaje expresivo. Sería genial que cada uno tenga su propio color para poder diferenciarlo cuando estén superpuestos (por que van a sonar de forma independiente pero al mismo tiempo, superpuestos).
- Corazón rojo, abeja amarilla y pájaro naranjo. Desglose de tonos cálidos.

![idea partitura 2](./imagenes/idea.png)

## Encargo-13b 

Leer capítulo 3 y 4 del libro Pomelo de Yoko Ono, compartir apuntes y reflexiones críticas sobre el texto, prohibido usar inteligencia artificial, no sirve para este ejercicio.

### Capítulo 3: Evento. 

Mis favoritos:

- Pieza de iluminación. (Encender un fósforo y vigilar hasta que se consuma.) (que aesthetic)
- Pieza de arvejas. (Llevar una bolsa de arvejas. / Dejar una arveja en cada lugar donde se vaya.) (AMO LOS ARVEJAS !¡!¡)
- Pieza de aviso. (Hacer avisos fúnebres cada vez que uno / se muda en vez de dar / cambio la dirección. / Enviar el mismo aviso cuando muera.)
- Pieza de aviso II. (Anunciar cambio de dirección cada vez / que uno muere)
- Pieza solar. (Mirar el sol hasta que se ponga cuadrado.) (¿minecraft?)
- Pieza de lavado. (Al recibir visitas, sacar toda la / ropa sucia del día y explicarles / sobre cada prenda. Cómo y cuándo se ensució y / por qué, etc.)
- Pieza de reloj. (Adelantar todos los relojes del mundo / dos segundos sin que nadie se entere.)
- Pieza para arrojar. (Arrojar una piedra al cielo tan alto / que nunca vuelva.)
- Pieza de bruma I. (Pensar en lo que está pensando la persona de al lado.)
- Pieza de nombre. (Cambiarse el nombre por épocas. / Según la edad. / Según el año. / Según el día. / Según la ocasión. / Según el color de ropa.)

### Capítulo 4: Poesía. 

Mis favoritos:

- Pieza numeral I. (Contar todas las palabras del libro / en vez de leerlas.)
- Pieza silábica. (Decidirse a no usar una sílaba / en particular el resto de la vida. / Registrar las cosas que ocurren / como resultados de esto.)
- Un poema para ser leído por lupa. (no tengo lupa :C)

### Apuntes generales 

- Sobre Pieza de aviso II: pensé que solo morimos una vez en la vida. Aunque mi mamá siempre que alguien se muere en una película o una serie dice "y nunca antes había muerto". 
- El capítulo de eventos tiene mucha relación con la muerte, cosas fúnebres y muerte, mucha muerte.
- Muchas piezas funcionan como pequeños ¿experimentos? que alteran la forma habitual de relacionarnos con el tiempo, los objetos o las personas.
- Varias instrucciones tienen un tono chistoso, pero también esconden reflexiones más profundas sobre la identidad, la muerte o la convivencia.
- Pieza de aviso I y Pieza de aviso II me parecieron muy ingeniosas. Juegan con la relación entre mudanza y muerte, como si cambiar de vida implicara abandonar una versión anterior de uno mismo. 
- Tal vez constantemente "morimos" y renacemos a través de nuestras experiencias.
- En estos capítulos sentí que Yoko Ono se volvió más juguetona y, al mismo tiempo, más filosófica (introspección). 
- Muchas piezas me hicieron reír o pensar en referencias actuales (como Minecraft), mientras que otras me llevaron a cuestionar temas mucho más profundos, como la identidad o la muerte. 
- Me gusta que el libro hasta el momento no intenta imponer una interpretación correcta (esto porque dependiendo con quien lo he hablado opina algo distinto de las mismas piezas) permite reaccionar con humor, incomodidad o confusión, etc.
- por si no lo dije muchas veces ya: muerte. 

