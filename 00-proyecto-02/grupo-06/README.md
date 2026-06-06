# proyecto-02

## Grupo

Número de grupo: 06

Tema del grupo: **Percutores**. 

Integrantes:

- Catalina Catalán / [06-terroiblea](https://github.com/terroiblea/dis8644-2026-1-procesos-2/tree/main/06-terroiblea)
- Martina Echavarría / [10-martinaechavarria-stack](https://github.com/terroiblea/dis8644-2026-1-procesos-2/tree/main/10-martinaechavarria-stack)
- Nicolás Miranda / [18-Nicolas-Miranda1312](https://github.com/terroiblea/dis8644-2026-1-procesos-2/tree/main/18-Nicolas-Miranda1312)
- Vania paredes / [24-paredesvania](https://github.com/terroiblea/dis8644-2026-1-procesos-2/tree/main/24-paredesvania)
- Carla Pino / [25-coff4](https://github.com/terroiblea/dis8644-2026-1-procesos-2/tree/main/25-Coff4)

## Circuito 1

Lub-dub.  

### Descripción general/conceptual 1

Lub-dub hace exactamente lo que hace un corazón: **bombea**. Pero en vez de bombear sangre, bombea pulsos eléctricos. En vez de mantener vivo a un organismo, **mantiene vivo el ritmo**. Lub-dub late. A veces  *Tac. Tac. Tac*. Otras, *Dumb. Dumb. Dumb*. Con la misma indiferencia biológica con que tu corazón te despertó esta mañana, Lub-dub bombea energía guiada por un compás. Es un percutor. Es un metrónomo pero con actitud.

#### ¿Qué hace Lub-dub por ti?

- Permite ajustar el tempo y el carácter del golpe, desde un latido tranquilo de persona en reposo hasta los 180bpm de alguien que acaba de ver su nota de taller.
- Es clínicamente superior a un metrónomo porque suena cool y los metrónomos no.
- Científicos del Instituto Cardiovascular de Sonidos Raros han determinado que escuchar Lub-dub mientras estudias mejora la concentración en un 340%. Este dato no ha sido verificado.

### Descripción de funcionamiento 1

Lub-dub recibe 12V por un jack de alimentación, regulados internamente a 5V con un L7805. Su output es una señal de audio por un jack estéreo. Tiene cuatro potenciómetros que en conjunto controlan el tempo y el carácter del golpe.

El corazón del circuito es un oscilador construido con inversores Schmitt-trigger de los chips 40106 y 4069UBE. Un condensador se carga y descarga continuamente a través de resistencias variables: los potenciómetros cambian esas resistencias, lo que cambia qué tan rápido se carga el condensador y por lo tanto qué tan rápido late y cómo suena ese latido. La ventaja del Schmitt-trigger es que conmuta en voltajes distintos al subir y al bajar, lo que produce ese golpe brusco y limpio en vez de una transición suave. Antes de llegar al output, la señal pasa por una red de condensadores y resistencias que recorta el pulso y lo convierte en un impulso corto y acentuado. Ese recorte es lo que transforma la oscilación en un *tac* o un *dumb* dependiendo de cómo estén ajustados los potenciómetros.

### Falstad 1

Antes de armar cada circuito realizamos un testeo del flujo de la corriente de cada circuito. 

![falstad circuito 01](./imagenes/falstad-01.gif)

### Esquemático 1

Esquemático referencia 1: Logic Noise: Filters And Drums de Hackaday.

![esquematico referencia](./imagenes/esquematico-referencia-1.PNG)

Esquemático intervenido:

![esquemático circuito](./imagenes/esquematico-1.png)

### PCB 1

La imagen de referencia para desarrollar el diseño de la PCB fue sacada de internet (link en referencias bibliográficas)

![pcb front](./imagenes/pcb-front-1.png)

![pcb back](./imagenes/pcb-back-1.png)

![pcb editable](./imagenes/pcb-editable-1.png)

### Documentación audiovisual 1

#### Video funcionamiento protoboard 1

[![video funcionando](./imagenes/video01-1.jpg)](https://youtube.com/shorts/qcpgWSdzTUw?feature=share)

#### Video proceso y cambios protoboard 1

[![video proceso](./imagenes/video01-2.jpg)](https://youtube.com/shorts/XpsWV_Oy70A?feature=share)

## Circuito 2

Barry Benson.  

### Descripción general/conceptual 2

Barry Benson no es una abeja. **Es peor que una abeja**, es una abeja con complejos, quiere ser una mosca. Tiene la capacidad sobreinsectoide de reproducir exactamente ese sonido de mosca agonizante atrapada entre tu oreja y la almohada a las 3 de la madrugada. Es la representación en silicio de ese sonido, **Barry Benson pega zumbidos**. Un zumbido ondulante que sube y baja de intensidad como si el insecto se acercara y alejara de tu oído a voluntad propia. La ciencia no puede explicar del todo por qué suena exactamente así. Nosotros tampoco. Pero lo hace.

#### ¿Qué hace Barry Benson por ti?

- Reproduce con fidelidad perturbadora el sonido de un insecto atrapado entre tu oreja y la almohada.
- Permite ajustar el zumbido con cuatro potenciómetros para encontrar el tono exacto que más molesta a tu compañero de pieza.
- Según investigaciones del prestigioso Instituto de Zumbidología Aplicada de Concepción, la exposición prenatal al sonido de Barry Benson produce niños con oído absoluto y una relación complicada con los insectos.
- Suena como *bzzzZZZzzzbzzZZZZzbzz*. Como si alguien hubiera atrapado una abeja en un sintetizador analógico y ninguno de los dos estuviera contento con la situación.
  
### Descripción de funcionamiento 2

Barry Benson recibe 12V por un jack de alimentación, que el circuito reduce internamente a 5V usando un regulador L7805. Su único output es una señal de audio por un jack estéreo.

Cuando alguien usa Barry Benson, interactúa con cuatro potenciómetros. Cada uno controla la frecuencia de un oscilador independiente, en otras palabras, es básicamente qué tan rápido vibra cada "ala" de la abeja. El chip que hace posible todo esto es el 40106, que contiene seis inversores Schmitt-trigger, componentes que deciden cuándo una señal es alta o baja, produciendo oscilaciones estables. Las cuatro señales resultantes se mezclan a través de compuertas XOR del chip 4070. Una XOR produce señal solo cuando sus entradas son distintas, así que al combinar frecuencias similares pero no idénticas, la salida fluctúa a una velocidad igual a la diferencia entre ambas. Ese fenómeno es lo que hace que el volumen suba y baje de forma orgánica y le da a Barry ese carácter de insecto vivo que ningún preset de sintetizador ha logrado replicar con tanta dignidad.

### Falstad 2

![falstad circuito 02](./imagenes/falstad-02.gif)

### Esquemático 2

Esquemático referencia: Inharmonic square waves (página 238) de Make: Electronic Music from scratch.

![esquematico referencia](./imagenes/esquematico-referencia-2.JPG)

Esquemático intervenido: 

![esquemático circuito](./imagenes/esquematico-2.png)

### PCB 2

La imagen de referencia para desarrollar el diseño de la PCB fue sacada de internet (link en referencias bibliográficas)

![pcb front](./imagenes/pcb-front-2.png)

![pcb back](./imagenes/pcb-back-2.png)

![pcb editable](./imagenes/pcb-editable-2.png)

### Documentación audiovisual 2

#### Video funcionamiento protoboard 2

[![video funcionando](./imagenes/video02-1.jpg)](https://youtube.com/shorts/eccHGz9GCeo?feature=share)

#### Video proceso y cambios protoboard 2

[![video proceso](./imagenes/video02-2.jpg)](https://youtube.com/shorts/TsO3bf-ZHFw?feature=share)

## BOM

| Componente | Tipo | Cantidad | Precio (c/u) | Comprar |
|------------|------|----------|--------------|---------|
| Chip 4069UBE | Circuito Integrado | 1 | $1.100 | [Cabeza Cuadrada](https://www.cabezacuadrada.cl/product/cd4069/) |
| Chip CD40106BE | Circuito Integrado | 2 | $750 | [Cabeza Cuadrada](https://www.cabezacuadrada.cl/product/cd40106be/) |
| Potenciómetro 100K | Potenciómetro | 4 |  $490 | [Mechatronic Store](https://www.mechatronicstore.cl/potenciometro-rotacional-10k/) |
| Potenciómetro 250K | Potenciómetro | 4 | $495 | [Altronics](https://altronics.cl/potenciometro-lineal-250k-b250k) |
| Capacitor no polarizado 100nF | Condensador Cerámico | 6 |  $100 | [Mechatronic Store](https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/) |
| Capacitor no polarizado 10nF | Condensador Cerámico | 1 | $100 | [Mechatronic Store](https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/) |
| Capacitor polarizado 10uF 50V | Condensador Electrolítico | 6 |  $100 | [Mechatronic Store](https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/) |
| Capacitor polarizado 0.22uF 50V | Condensador Electrolítico | 1 |  $100 | [Mechatronic Store](https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/) |
| Capacitor polarizado 100uF 50V | Condensador Electrolítico | 4 | $100 | [Mechatronic Store](https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/) |
| Capacitor polarizado 1uF 50V | Condensador Electrolítico | 1 | $100 | [Mechatronic Store](https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/) |
| Resistencia 100K | Resistencia 1/2W | 1 |  $100 | [Mechatronic Store](https://www.mechatronicstore.cl/resistencias-electricas-1-2-w-1-unidad/) |
| Resistencia 1K | Resistencia 3W | 4 |  $200 | [Mechatronic Store](https://www.mechatronicstore.cl/resistencias-electricas-3w-por-unidad/) |
| Diodo 1N4007 | Diodo Rectificador | 2 | $200 | [Mechatronic Store](https://www.mechatronicstore.cl/diodo-rectificador-in4007-1n4007-4007/) |
| LED 3mm/5mm | LED | 3 |  $100 | [Mechatronic Store](https://www.mechatronicstore.cl/led-3mm-5mm/) |
| Regulador de voltaje L7805 | Regulador 5V DC | 2 | $490 | [Mechatronic Store](https://www.mechatronicstore.cl/regulador-limitador-de-voltaje-5v-dc/) |
| Chip CD4070BE | Circuito Integrado | 1 | - | [Mouser](https://www.mouser.cl/ProductDetail/Texas-Instruments/CD4070BE?qs=5WY7Uqh921w5Ya0dPgjorQ%3D%3D) |
| Protoboard 830 puntos | Protoboard MB102 | 2 | $3.790 | [Mechatronic Store](https://www.mechatronicstore.cl/breadboard-830-puntos-mb102/) |
| Barrel Jack Switch | Conector | 4 | — | Extraídos del LID |
| Switch 2 pines, 2 posiciones | Interruptor On/Off | 2 | $570 | [Katode](https://www.katode.cl/switches/1339-interruptor-switch-2-pines-on-off-corto.html) |

## Otros circuitos 

### Amplificador/salida 

Usamos la base anteriormente vista en el proyecto 01 con el Chip 386; circuito temporal de amplificador para sonar más alto y poder modificar el sonido final. Al modificarse ciertos parámetros (condensadores) cada placa sonaba distinto. Barry Benson funciona mejor con condensadores menores a 100 μF y Lub-dub funciona mejor con condensadores de 100 μF.    

![esquema amplificador](./imagenes/esquema-amplificador.png)

![amplificador uso en ideas 1 y 2](./imagenes/amplificador-ejemplo.jpg) 

## Colaboración con otros grupos

### ¿Cómo ayudamos a otros grupos?

#### Carla Pino:

- Ayudó a dos grupos a subir de forma correcta las carpetas del proyecto 2, específicamente el apartado de las versiones de esquemáticos y PCB. 
- Ayudó a distintos grupos a instalar bibliotecas externas de KiCad.

#### Martina Echavarría: 

- Ayudó a *Grupo 01* a cargar su batería.

#### Vania Paredes, Catalina Catalán y Nicolás Miranda: 

- Ayudaron a *Grupo 04* en indicar e instruir cómo conectar barrel y audio jack.

#### Nicolás Miranda: 

- Ayudó a *Grupo 05* a poner y buscar huellas en KiCad. 

![trabajo en equipo](./imagenes/trabajo-en-equipo.jpg)

### ¿Cómo nos ayudó otro grupo?

- El *Grupo 01* nos ayudó con las huellas (recordar comandos). 
- El *Grupo 01* nos prestó su batería para grabar porque la de nosotros se quedó sin carga.

Agradecimiento especial a Sebastián Sáez (Sae porque sabe) que si bien no es del curso siempre está en el lid para prestarnos su super ayuda.

## Bibliografía

### Referencias Bibliográficas

- Akther, S. (s.f). *Vectores corazón real*. Vecteezy. <https://es.vecteezy.com/arte-vectorial/67973094-anatomico-humano-corazon-ilustraciones-anatomia-medico>
- Pearson, K. (2024). *Make: Electronic Music from scratch*. Make Community, LLC.  
- Stock,M. (25 de Febrero, 2026). *Silueta simple en negro y blanco de una abeja*.  Shutterstock. <https://www.shutterstock.com/es/image-vector/simple-black-white-silhouette-bee-representing-2743356303>
- Williams, E. (25 de Marzo, 2015). *Logic Noise: Filters And Drums*. Hackaday. <https://hackaday.com/2015/03/25/logic-noise-filters-and-drums/>

### Bibliografía investigación

- Klein, M. [@MoritzKlein0](10 de Agosto, 2023). *Designing a simple analog kick drum from scratch* [video]. Youtube. https://youtu.be/yz37Yz315eU
- Klein, M. [@MoritzKlein0](19 de Abril, 2024). *Designing a TR-808 style snare drum from scratch* [video]. Youtube. <https://youtu.be/hULEn2_4Unw>
- Klein, M. [@MoritzKlein0](5 de Diciembre, 2023). *Diseñando un hi-hat estilo TR-606 desde cero* [video]. Youtube. <https://youtu.be/zbBY7JL9nnQ>
- Pekkarinen, L. [@krakenpine](6 de Diciembre, 2020). *Diy Twin-T kick drum eurorack module demo* [video]. Youtube. <https://youtu.be/iETSEz60OVA>
- Pekkarinen, L. (2024). *k
rakenpine-synthing*. GitHub. 
<https://github.com/Krakenpine/krakenpine-synthing/tree/main>
- Newton C. (s.f). *Generadores de Percusión (ART858S)*. INCB. <https://www.incb.com.mx/index.php/articulos/9-articulos-tecnicos-y-proyectos/9910-generadores-de-percusion-art858s>
- Newton C. (s.f). *Generador de Percusión Para Ritmos Musicales (ART1596S)*. INCB. <https://newtoncbraga.com.mx/articulos/9-articulos-tecnicos-y-proyectos/31055-generador-de-percusion-para-ritmos-musicales-art1596s>
- Richardson, R. (23 de Marzo, 2013) *Twin T drum osc with 555 trigger*. Cirfcuit-Lab. <https://www.circuitlab.com/circuit/eykayh/twin-t-drum-osc-with-555-trigger/>
