# sesion-11b

- ## avance 1 entrega 2!!!
  - primero que todo la sala estaba llena de trabajos y materiales botados
    - sacamos todo para tener una sala digna del taller
      - ![basura 1](./imagenes/basura-1.jpg)
      - ![basura 2](./imagenes/basura-2.jpg)
  - nos juntamos como grupo para avanzar en el piezo 1
    - nos falta ver bien el tema del piezo y que tán sensible es a las vibraciónes
      - la idea de tener el 4017 activado por la voz es media dificil
        - ![piezo voz intento](./imagenes/piezo-voz.gif)
          - (no se ve pero Benja / benjaminalvarez21 tiene el piezo pegado a su cuello intentando que el 4017 avance)
        - no funciona porque la señal que sale del piezo es muy debil y probablemente tiene mucho ruido no deseado del ambiente
          - una idea que se nos ocurrió fue añadir un pre-amp y un filtro low-pass para tener una señal funcional con el 4017
          - ![lowpass calculator](./imagenes/lowpass.png)
            - sentimos que alrededor de 500hz es optimo para que funcione
  - estabamos cansados y con hambre.... menos mal los profen trajeron donas
    - ![donas](./imagenes/donas.jpg)
      - muchas gracias, ahora tenemos energía para todo el dia
  - con la energía de la dona decidímos hacer el regulador de voltaje que se pide para todos los circuitos
    - ![regulador 5v](./imagenes/switch-regulador.gif)
      - nos funcionó con un switch, fuimos felices ya que era la primera vez que conectabamos uno
     
 - ## avance 2 entrega 2!!!
   - nos juntamos el lunes 01 para avanzar en el piezo 1
     - ![v03 sin pre-amp](./imagenes/v03-sin-pre.jpg)
   - probamos añadir un 2n2222 como amplificador del piezo pero no funcionó
     - la señal no pasaba y sentímos que quizás no era el amplificador adecuado para lo que queremos
       - ![2n2222](./imagenes/intento-2n2222.jpg)
   - tambíen probamos con un lm386 pero al conectarlo el resto del circuito dejó de funcionar
     - algo pasó, pero al excluirlo y alimentar el circuito base, todo volvió a la normalidad
   - **si** acertamos con un tl072
     - un IC amp dual que se suele usar para pedales de efectos 
       - ![tl072 1](./imagenes/tl072-1.jpg)
         - funcionó **muy** bien
           - detectaba golpes a varios centimetros
             - al ponerlo en nuestro cuello detectaba el puslo
               - eso sí, no es muy estable y a unos minutos el 4017 empieza a avanzar sin ritmo y sin input directo del piezo
      - lo intentamos una segunda vez pero ahora no prendía el 4017
        - ![tl072 2](./imagenes/tl072-2.jpg)
          - el circuito que usamos fue este 
            - ![tl072 circuit](./imagenes/tl072-circuit.jpg)
           
--------------------------------
  
  - ### ejemplos del circuito funcionando (sin pre-amp)
    - alargamos la distancia del piezo para poder situarlos a extremos de la sala al momento de la entrega
      - esto lo hace más interactivo y nos da la opción de adaptarlo a un choker si el pre-amp llegase a funcionar antes de la entrega
        - ![piezo largo 1](./imagenes/piezo-largo-1.gif)
        - ![piezo largo 2](./imagenes/piezo-largo-2.gif)
      - la idea es tener uno en la entrada, quizas el piso para que se active con los pasos y el otro al otro extremo de la sala, en una mesa o muralla

--------------------------------
     
  - ### 3 albumes flash que a mi parecer son buenos!!!!!!!
    - "Getting Killed - Geese"
      - ![Getting Killed](./imagenes/geese.jpg)
        - banda gringa con lider Cameron Winter
          - Indie-Rock / Blues
    - "Time 'n' Place - Kero Kero Bonito"
      - ![Time 'n' Place](./imagenes/kkb.jpg)
        - banda de Sarah Bonito, Gus Lobban y Jamie Bulled
          - Twee Pop / Indie Pop / Noise Pop
    - "Ceres & Calypso in the Deep Time - Candy Claws"
      - ![Ceres & Calypso in the Deep Time](./imagenes/candy-claws.jpg)
        - banda de Ryan Hover, Karen Hover y Hank Bertholf
          - Dream Pop / Shoegaze / Noise Pop
