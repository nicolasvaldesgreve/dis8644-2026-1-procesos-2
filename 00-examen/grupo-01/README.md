# examen-grupo-01

## integrantes


- Benjamín Alonso Álvarez Pavez / [benjaminalvarez21](<https://github.com/disenoUDP/dis8644-2026-1-procesos-2/tree/main/03-benjaminalvarez21>)
- Anays Valentina Cornejo Candia / [Anaysval](<https://github.com/disenoUDP/dis8644-2026-1-procesos-2/tree/main/09-Anaysval>)
- Bruno Ferrari Meyer / [chknngttts](<https://github.com/disenoUDP/dis8644-2026-1-procesos-2/tree/main/11-chknngttts>)
- Lucas Ignacio Ortiz Aguirre / [ryukivol](<https://github.com/disenoUDP/dis8644-2026-1-procesos-2/tree/main/21-ryukivol>)
- Nicolás Elías Valdés Greve / [nicolasvaldesgreve](<https://github.com/disenoUDP/dis8644-2026-1-procesos-2/tree/main/31-nicolasvaldesgreve>)


## criterios de diseño del sistema

inspiración para construir, desde donde partieron

contexto desde Chile, desde nuestra disponibilidad material

nombre de sistema/instrumento construido por medio de módulos

## placas soldadas

principio de funcionamiento de cada una, qué tipo de señal entrega a la salida, qué recibe
lista de materiales con costos. Incluir tiempo de soldadura


### Placas armadas


- Maincra
- Registro de desplazamiento estático (Nyan cat)
- Comando estelar
  

  ### BOM PCB MAINCRA

| Componente | Cantidad | PCB | Valor unitario | Link | ¿Hay stock en LID? |
| --- | --- | --- | --- | --- | --- |
| Chip NE555P | 1 | U1 | $490 | <https://www.victronics.cl/circuitos-integrados/lm555cngeneralpurposebipolartimerdip8/> | Sí |
| Chip TL072CP | 1 | U4 | $990 | <https://www.victronics.cl/circuitos-integrados/tl072cpdualjfetlowpoweropamplifierdip8/> | No |
| Regulador L7805CV | 1 | U3 | $350 | <https://www.victronics.cl/reguladores/reguladorvoltl7805cv5v-15ato220/> | No |
| Diodo 1N4007 | 1 | D5 | $200 | <https://www.mechatronicstore.cl/diodo-rectificador-in4007-1n4007-4007/> | Sí |
| Diodo 1N5819 | 2 | D6, D7 | $586 | <https://cl.rsdelivers.com/product/nexperia/bat85113/nexperia-diodo-bat85113-diodo-schottky-200-ma-30-v/0300978> | No |
| Transistor 2N2222 | 1 | Q1 | $200 | <https://www.mechatronicstore.cl/transistor-2n2222/> | Sí |
| Potenciómetro B10K | 1 | RV1 | $495 | <https://altronics.cl/potenciometro-lineal-10k-b10k> | No |
| Potenciómetro B500K | 1 | RV2 | $495 | <https://altronics.cl/potenciometro-lineal-500k-b500k?search=b500k> | Sí |
| LED 3mm | 3 | D1, D2, D8 | $100 | <https://www.mechatronicstore.cl/led-3mm-5mm/> | Sí |
| Resistencia 47 Ω | 1 | R12 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | No |
| Resistencia 100 Ω | 1 | R18 |  $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 220 Ω | 1 | R14 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 1 KΩ | 6 | R1, R3, R6, R7, R8, R11 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 2,2 KΩ | 1 | R13 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | No |
| Resistencia 10 KΩ | 2 | R4, R5 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 100 KΩ | 3 | R2, R16, R17 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 2,2 MΩ | 1 | R15 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | No |
| Condensador cerámico 1 µF | 1 | C9 | $100 | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/> | No |
| Condensador cerámico 4.7 nF | 1 | C12 | $100 | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/> | No |
| Condensador cerámico 10 nF | 1 | C13 | $100 | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/> | No |
| Condensador cerámico 100 nF | 3 | C1, C7, C10 | $100 | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/> | Sí |
| Condensador polarizado 10 µF | 2 | C9, C11 | $100 | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> | Sí |
| Condensador polarizado 100 µF | 3 | C2, C3, C5 | $100 | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> | Sí |
| Piezo | 1 | J8 | $990 | <https://www.mechatronicstore.cl/sensor-piezoelectrico-27mm-con-cable/> | Sí |
| Cables dupont 40 uni. | 1 | - | $2.990 | <https://mcielectronics.cl/shop/product/cable-dupont-macho-macho-20cm-pack-40-unidades-2/> | Sí |
| Batería 9V recargable | 1 | BT1 | $7.990 | <https://www.sodimac.cl/sodimac-cl/articulo/110251085/bateria-recargable-9v/110251089> | Sí |
| Interruptor Switch | 1 | SW3 | $570 | <https://www.katode.cl/switches/1339-interruptor-switch-2-pines-on-off-corto.html?srsltid=AfmBOorJlIeUySzAORFwXSattHKE4BKH2LmhhXZS_8fZ4MW-G6kwnxqA> | No |

### BOM PCB 02, GRUPO 02: REGISTRO DE DESPLAZAMIENTO ESTÁTICO / NYAN CAT

| Componente | Cantidad | PCB | Valor unitario | Link | ¿Hay stock en LID? |
| --- | --- | --- | --- | --- | --- |
| Chip 4015 | 1 | U2 | $1.400 | <https://www.mactronica.com.co/cd4015?srsltid=AfmBOopMDQhFv0vy6tj-sATCKe9rcEpOGbsfz7VMFRrBPl9Yq3KS80wU> | No |
| Regulador L7805CV | 1 | U4 | $350 | <https://www.victronics.cl/reguladores/reguladorvoltl7805cv5v-15ato220/> | No |
| Transistor 2N2222 | 8 | Q3, Q4, Q5, Q6, Q7, Q8, Q9, Q10 | $220 | <https://www.cabezacuadrada.cl/product/pn2222a/> | Sí |
| Transistor BC548 | 1 | Q1 | $200 | <https://www.mechatronicstore.cl/transistor-bc548/?srsltid=AfmBOorIdGTZFY0mLCpBPP8JWl9WGDELQa-iZIZ95pKPjncWCgmXklr3> | No |
| LED 3mm | 9 | D1, D2, D3, D4, D5, D6, D7, D8, D12 | $100 | <https://www.mechatronicstore.cl/led-3mm-5mm/> | Sí |
| Resistencia 220 Ω | 8| R4, R5, R6, R7, R8, R9, R10, R11 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 1 KΩ | 18 | R3, R12, R15, R16, R17, R18, R19, R20, R21, R22, R23, R24, R25, R26, R27, R28, R29, R30 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 10 KΩ | 1 | R2 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Resistencia 100 KΩ | 1 | R13 | $90 | <https://www.electroardu.cl/resistencias-1k-ohm?srsltid=AfmBOor81HKrzfoOTnLK3FU6ObPuf1EPUVMS0naCwqMNIzGt8LYDiUYt> | Sí |
| Diodo 1N4007 | 1 | D11 | $200 | <https://www.mechatronicstore.cl/diodo-rectificador-in4007-1n4007-4007/> | Sí |
| Condensador cerámico 100 nF | 1 | C9 | $100 | <https://www.mechatronicstore.cl/condensadores-ceramicos-distintos-valores/> | Sí |
| Condensador polarizado 10 µF | 1 | C8 | $100 | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> | Sí |
| Condensador polarizado 100 µF | 1 | C7 | $100 | <https://www.mechatronicstore.cl/condensador-capacitorio-de-electrolitico-por-unidad-varios-valores/> | Sí |
| Interruptor Switch | 1 | SW4 | $570 | <https://www.katode.cl/switches/1339-interruptor-switch-2-pines-on-off-corto.html?srsltid=AfmBOorJlIeUySzAORFwXSattHKE4BKH2LmhhXZS_8fZ4MW-G6kwnxqA> | No |

### BOM PCB 03, GRUPO 03: COMANDO ESTELAR 
(hay q organizarlo aun)
| Componente | Cantidad | PCB | Valor unitario | Link | ¿Hay stock en LID? |
| --- | --- | --- | --- | --- | --- |
| Chip CD4046 | 1 | U1 | $700 | Electrónica Real | |
| Chip CD40106 | 1 | U4 | $1200 | Electrónica Real | |
| L7805 | 1 | U2 | $350 | Victronics | |
| Diodo 1N4007 | 1 | D1 | $790 | Victronics | |
| LED | 1 | D2 | $920 | Electrónica Real | |
| Resistencia 100kΩ | 1 | R1 | $890 | Electrónica Real | |
| Resistencia 1kΩ | 1 | R2 | $890 | Electrónica Real | |
| Potenciómetro 100Ω | 2 | RV1, RV2 | $500 | Afel a Ingeniería | |
| Capacitor 10nF | 1 | C1 | $520 | Victronics | |
| Capacitor 100nF | 1 | C5 | $500 | Victronics | |
| Capacitor 100uF | 2 | C2, C6 | $670 | Victronics | |
| Capacitor 10uF | 2 | C3, C4  | $330 | Victronics | |
| Capacitor 1uF | 1 | ?? | $300 | Victronics | |
| Jack DC | 2 | J2, J3 | $150 | Electrónica Real | |
| Jack de audio | 1 | J1 | $150-$300 | Victronics | |

 Según yo esto no va 
 
| Interruptor de palanca SPDT ON-ON | 1 | SW1 | $590 | Electrónica Real | |
| Separador o tornillo de montaje (M3*8) | 4 | 4 | $54 | Pernos Alameda | |
| Cable Dupont | 19 | 19 | $1190 (pack 10) | MCI Electronics | |



## carcasa

decisiones materiales y formales de la carcasa
inspiración y referentes (con cita)

Carcasas individuales para cada PCB, se busca celebrar el diseño de las mismas mediante la transparencia del acrilico, rompiendo la caja negra e invitando a la apreciación integra de cada PCB y sus distintos componentes

## composición
partitura e interpretación
detallar operación de la partitura, como se creó, cuales fueron los referentes (citando), cual es la simbología


- Referentes

 
- Simbología

  
---

#### Integración a la vida diaria



---

#### Ping Pong

(ver. literal examen) Como grupo-01 vamos a ir a República 180, Santiago de Chile con “maincra” (piezo-01), el parlante, RELO (Reloj 555 Monoestable) y “nyan cat” (secuenciador-2). Poner un piezo en cada lado superior de la mesa al centro, y pegarlo en la mesa con cinta adhesiva. Jugar una partida con paletas y pelota de Ping Pong que se piden donde los guardias. Con el impacto de la pelota en la mesa el secuenciador avanza, haciendo que el oscilador pueda funcionar. Jugar durante 5 minutos. Al perder, se cambian los jugadores. Al finalizar los 5 minutos se devuelven las paletas y pelota a los guardias. 

(ver. literal 2) Como grupo-01 vamos a ir a República 180, Santiago de Chile con “maincra” (piezo-01), el parlante, RELO y “nyan cat” (secuenciador-2). Poner un piezo en cada lado superior de la mesa al centro, y pegarlo en la mesa con cinta adhesiva. Jugar una partida completa de Ping Pong de 21 puntos con las paletas y pelota que se piden con los guardias. Con el impacto de la pelota en la mesa el secuenciador avanza, haciendo que el oscilador pueda funcionar. Al terminar la partida devolver las paletas y pelota a los guardias.

(ver. poética)

>**Ve a República 180 y ubica el piezo en la mesa de ping pong**

>**Invita a alguien a jugar**

>**Jueguen durante 5 minutos o hasta que se aburran**

## bibliografía
