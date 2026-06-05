# proyecto-02

## Grupo

Número de grupo: 03

Tema del grupo: Oscila02

Integrantes:

- Vanessa García / vanessagarciaM
- Antonia Loch / antoloch
- Carla Núñez / ccarlabelenn
- Ariel Orozco / arielorozco024
- Narely Riquelme / Narelyriquelme

## Circuito 1

Título módulo 1
-
### Descripción general/conceptual 1

¿Qué hace el circuito? Intentar explicarlo para gente que no sabe electrónica. Ejemplo: escucha los impactos sobre sí mismo y lo convierte en señales de aviso para otras cosas

### Descripción de funcionamiento 1



### Esquemático 1


![esquemático circuito](./imagenes/esquematico-1.jpg)


### PCB 1

+ Front
  
![pcb front](./imagenes/pcb-1.jpg)

+ Back
  
![pcb back](./imagenes/pcb-3.jpg)


### Documentación audiovisual funcionamiento protoboard 1

<https://youtu.be/w_llKDzQWCs?si=krRRTBGmpJ4E8jTr>

## Circuito 2

Título módulo 2

### Descripción general/conceptual 2

Este circuito es un generador de pulsos eléctricos rítmicos cuya velocidad puede ser controlada manualmente. Funciona de forma similar al latido de un corazón, produce una señal que sube y baja de forma continua. La velocidad de ese latido eléctrico puede ajustarse girando un potenciómetro, y la señal resultante sale por un conector de audio. Además de generar el pulso principal, el circuito es capaz de dividirlo en pulsos más lentos y secuenciales, lo que permite obtener múltiples ritmos derivados de una sola oscilación base.  

| Bloque | Nombre | Descripción |
|--------|--------|-------------|
| 1 | Alimentación | Recibe energía por conectores barrel jack con interruptor SW3. El diodo 1N4007 protege contra inversión de polaridad, el regulador L7805 entrega +5V estables y condensadores de filtrado eliminan el ruido. Un LED indica que el circuito está encendido. |
| 2 | Núcleo Oscilador (CD4046) | El CD4046 genera una señal cuya frecuencia depende del voltaje en su pin VCOin. RV1 controla ese voltaje manualmente, R1 y R2 (470kΩ) definen el rango de frecuencias, y C1 y C2 determinan los tiempos de oscilación. |
| 3 | Divisor de Frecuencia (CD4017) | Recibe la señal del CD4046 y la distribuye en 10 salidas secuenciales, generando subritmos y divisiones de frecuencia a partir de la oscilación base. |
| 4 | Buffers (CD40106) | Los inversores Schmitt trigger limpian y acondicionan la señal. RV2 y C3 moldean su forma antes de la salida, y un LED indica actividad en la señal procesada. |
| 5 | Salida | La señal sale por un conector de audio jack de 3.5mm (J4) y un conector auxiliar de 3 pines (J5) para integración con otros módulos. |

### Descripción de funcionamiento 2

El nucleo del módulo es el chip CD4046, cuya frecuencia de oscilación varía según el voltaje que recibe como input, voltaje que el usuario controla girando el potenciómetro RV1 para determinar el tono, grave o agudo. Internamente, el chip CD4017 toma esa oscilación base y la divide para crear subritmos y variaciones, mientras que el CD40106 convierte la señal en algo más ordenado y preciso. El output es esa señal acondicionada que sale por el conector de audio, lista para ser procesada por el resto del sintetizador. Algo que descubrimos en el camino es que pequeñas variaciones en las conexiones de la protoboard podían hacer que el circuito dejara de oscilar por completo. A futuro, este módulo podría conectarse a un teclado o secuenciador que envíe voltajes de control precisos, permitiendo tocar notas musicales específicas en lugar de un tono fijo.

## Fases de desarrollo 

+ Fase 1: Diseño del esquemático: Realizado en KiCad 8.0.2, basándose en las hojas de datos principales para determinar los valores de componentes.
+ Fase 2 Prototipo en protoboard: El circuito se ensambló en protoboard para verificar su funcionamiento, ajustar valores y detectar errores antes de fabricar la PCB.
+ Fase 3 Diseño y fabricación de PCB: Validado el prototipo, se diseñó el layout en KiCad aplicando buenas prácticas de ruteo y planos de tierra, resultando en una PCB compacta con todos los bloques integrados y gráfica 

### Esquemático 2


![esquemático circuito](./imagenes/esquematico-2.jpg)


### PCB 2

+ Front
  
![pcb front](./imagenes/pcb2-1.jpg)

+ Back
  
![pcb back](./imagenes/pcb2-2.jpg)


### Documentación audiovisual funcionamiento protoboard 2

<https://youtu.be/CfhnyoPfrF4?si=XYL1ljWvHR_3fHHc>

## Otros circuitos

Para probar los inputs y outputs de nuestro módulo VCO utilizamos un circuito de salida de audio basado en el amplificador LM386 que utilizamos en el proyecto 01, conectado a un parlante. Este circuito recibía la señal de nuestro oscilador a través de una entrada MIX, permitiéndonos escuchar directamente si el VCO estaba generando la oscilación correctamente y verificar los cambios de frecuencia al girar los potenciómetros.

![imagenes](./imagenes/salida.jpg)

## Colaboración con otros grupos

### ¿Cómo ayudé a otro grupo?

Le proporcionamos ayuda al grupo que tambien estaba haciendo osciladores, prestandole potenciometros. 

### ¿Cómo me ayudó otro grupo?

Le daremos créditos especiales al grupo de piezos, quienes fueron de gran ayuda, ya que gracias a ellos resolvimos muchas dudas que nos surgieron a lo largo del proyecto. Al haber pasado por los mismos problemas que nosotros, nos prestaron potenciómetros, resolvieron dudas de bitácora y nos brindaron mucho apoyo emocional. También nuestro compañero Nicolás Miranda nos ayudó con las conexiones de la protoboard, ya que al inicio no logramos que sonara como oscilador, no existían variaciones y nos frustramos. Consultamos con Nico y él revisó el esquemático y la protoboard, llegando a la conclusión de que teníamos cables mal conectados, además nos ayudó a resolver como mejorar la gráfica de la pcb. 

## Bibliografía
