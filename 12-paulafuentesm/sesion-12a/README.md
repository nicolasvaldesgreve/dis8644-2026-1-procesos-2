# sesion-12a

## Pre-Solemne / 2 junio 

La clase estuvo enfocada en revisar las propuestas, realizar los cambios que queríamos implementar y comprobar si la propuesta 2 estaba funcionando correctamente con los componentes que teníamos disponibles.

---
### Propuesta 01

No hubo mayores problemas con esta propuesta. Al principio estábamos preocupados porque, al alcanzar el máximo nivel de oscilación, no sonaba como esperábamos. Según nosotros, debía producir un sonido parecido a un “brrr”, pero no ocurría. Después de revisarlo con más detalle y agregar resistencias para compensar los potenciómetros, el circuito comenzó a comportarse correctamente y todo funcionó según lo previsto.

[Haz clic aquí para ver el video oscilador 2 fallido](https://youtube.com/shorts/u7n1Udp8zkw)

---
### Propuesta 02

Complicaciones

Al inicio de la clase, la propuesta sonaba muy sucia y no oscilaba de la forma que debía. Nunca llegó a sonar con la intensidad esperada ni de manera estable. Revisamos el esquemático varias veces, pero no encontramos una solución. También desmontamos y volvimos a armar el circuito en cuatro ocasiones, obteniendo siempre el mismo resultado.

Hacia el final de la clase logramos que oscilara como cualquier oscilador convencional y que cambiara entre distintas formas de onda. Sin embargo, el sonido seguía siendo sucio y se cortaba constantemente, por lo que terminamos la sesión sin resolver completamente el problema.

Al volver a armar el circuito en nuestras casas, este dejó de sonar por completo. Pensamos que podría existir algún componente malo, ya que incluso después de reconstruirlo nuevamente el problema persistía.

Después de conversar varias veces como grupo y analizar las posibles causas, decidimos abandonar ese esquemático y optar por una alternativa más donde podemamos entender mejor el chip  y más fácil de implementar. Consideramos que seguir insistiendo con la propuesta anterior solo nos estaba haciendo perder tiempo y complicando el proceso.

![oscilador2](https://github.com/paulafuentesm/dis8644-2026-1-procesos-2/blob/4c65159b001f830d585a13df748b2130b1dba9a2/12-paulafuentesm/sesion-12a/imagenes/oscilador2.jpg)

[Haz clic aquí para ver el video oscilador 2](https://youtu.be/k1RPwMvWIzI)


---
### Propuesta 2.0

**El esquemático fue obtenido de la web Hackaday, específicamente del artículo "Logic Noise: Sweet, Sweet Oscillator Sounds", donde pudimos analizar qué función cumplía el chip y comprender cómo era su funcionamiento.**

Finalmente, decidimos trabajar únicamente con el chip 40106 y aprovechar las ondas cuadradas que este generaba. Esta solución resultó mucho más sencilla y menos estresante para todos. Además, nos permitió comprender mejor el funcionamiento del circuito y prepararnos de mejor manera para explicarlo durante la solemne.

Tomamos la decisión de priorizar el entendimiento del chip y sus funciones por sobre simplemente replicar un circuito más complejo que no lográbamos hacer funcionar de forma estable.

Una vez armado de esta manera, el sintetizador sonaba de la siguiente forma:

Después de un tiempo, el circuito dejó de sonar nuevamente. Se revisó y se volvió a armar varias veces para intentar encontrar el problema, pero durante las pruebas comenzó a salir un olor a quemado. En ese momento no estaba claro qué había ocurrido ni qué componente podía estar causando la falla.

Al día siguiente realizamos una prueba más detallada en protoboard y notamos que se había quemado. Una vez reemplazada por una nueva, el circuito volvió a oscilar con normalidad y recuperó su funcionamiento.

Con el circuito ya listos, decidimos experimentar con distintos valores de condensadores para observar cómo afectaban el comportamiento del sonido. Notamos que los condensadores de valores más altos, como los de 100 µF, generaban oscilaciones más lentas, con cambios de tono poco fluidos y una respuesta que no se ajustaba a lo que buscábamos.

Posteriormente reemplazamos estos condensadores por uno de 1 µF. El cambio fue inmediato: la oscilación se volvió mucho más rápida y el sonido pasó a ser más agudo e intenso. El resultado nos recordó a señales de interferencia electrónica, tonos telefónicos y sonidos característicos de equipos de comunicación antiguos. Esta característica nos pareció especialmente interesante ( espacial será un concepto importante de mencionar durante la solemne ).

![oscilador2.0](https://github.com/paulafuentesm/dis8644-2026-1-procesos-2/blob/6c2a9d3a54912818a887c4877530343c189bfcf8/12-paulafuentesm/sesion-12a/imagenes/oscilador2.0.jpg)

[Haz clic aquí para ver el video oscilador 2.0](https://youtube.com/shorts/4hJ7gwfARJY)
