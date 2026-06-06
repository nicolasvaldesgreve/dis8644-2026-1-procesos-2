# produccion-pcbs

jornada maratónica sábado 06 junio 2026

equipo docente toma todos los proyectos de kicad entregados el día anterior, de proyecto-02, y con eso edita, revisa, y envía a producción.

hay 6 grupos de trabajo con una temática en particular, cada grupo realizó 2 esquemáticos con sus respectivas placas, en varias versiones que subieron a la carpeta 00-proyecto-02.

a continuación los apuntes de las distintas revisiones hechas de estos proyectos, para prepararlos para su producción física.

en este repo creamos 3 carpetas:

- 0-versiones-estudiantes: archivos de kicad con las versiones más recientes de proyectos de estudiantes
- 1-versiones-profes: archivos de kicad con las versiones revisadas y realizadas por equipo docentes
- 2-archivos-produccion: gerbers de producción, etiquetados como revA.

## grupo-01: piezos

- benjaminalvarez21
- Anaysval
- chknngttts
- ryukivol
- nicolasvaldesgreve

### g-01-pie-01-rev-a

- cambiamos tamaño r15
- cambiamos conector de entrada
- cambiamos nomenclatura de "100 u" a "100u"
- cambiamos huella de transistor Q1, porque era la equivocada

### g-01-pie-02-rev-a

- no fue enviado a producción porque no tenemos garantía de que funcionara según lo visto en protoboard.

## grupo-02: secuenciadores

- isidoraalvarez
- tomascatri
- dayanapanitrur
- Estrabismx
- angel-udp

### g-02-sec-01-rev-a

en esquemático:

- agregamos resistor de clock in a ground, para pulldown.
- agregamos resistor entre 4040 Q0 patita 9 y salida
- agregamos resistor a cada salida de jack switch.
- cambiamos huellas de transistores a versión inline_wide para que tengan más espacio
- agregados mounting hole faltantes

en pcb:

- actualizamos conectores jack a la huella de la biblioteca, para poder rutear bien los nuevos resistores y no perdernos.

### g-02-sec-02-rev-a

en esquemático:

- agregamos también resistores de protección en entradas y salidas.
- agregados mounting hole faltantes

en pcb:

- actualizamos conectores jack a la huella de la biblioteca, para poder rutear bien los nuevos resistores y no perdernos.

## grupo-03: osciladores 1

- vanessagarciaM
- antoloch
- ccarlabelenn
- arielorozco024
- Narelyriquelme

### g-03-osc-01-rev-a

- C1 estaba rotado, fue corregido.
- audio jack de entrada y salida estaban mal conectados
- condensador de salida fue cambiado por uno no polarizado

### g-03-osc-02-rev-a

- renombrar C3 a 4u7
- cambiado C1 por condensador polarizado
- 40106 fue usado como dos chips distintos, en vez de usar varios schmitt triggers desde un mismo chip, tuvimos que hacer esos cambios
- volvimos a rutear casi todo, ya que se bajó de 2 chips a 1

## grupo-04: osciladores 2

- antokiaraa
- santiagocifuvelez
- paulafuentesm
- kristelagj
- catalinaoyanedel
- yairaruiz

### g-04-osc-01-rev-a

- borramos amplificador para que esté en otro módulo
- agregamos resistencia de salida
- conectamos bien el jack de salida de audio que tenía problemas

### g-04-osc-02-rev-a

- borramos amplificador para que esté en otro módulo
- agregamos valor a diodo faltante
- corregimos símbolo de los potenciómetros
- agregamos resistencia de salida
- agregamos jack de salida de audio

## grupo-05: filtros

- antoniaamc
- Catabalboa
- sebastianguevaralarotta
- CatalinaJeria
- Luisaatoro9

### g-05-fil-01-rev-a

- error grave en la nomenclatura de los proyectos: el 01 en su README dicen que es el activo, pero en Kicad es el pasivo
- cambiamos C1 por condensador no polarizado
- conectamos patita del medio de potenciómetro
- confusión en los tamaños de los condensadores C4 y C5
- los tamaños de las pistas usados no fueron los indicados en clases ni en estandarización
- faltó el paso de agregar tierra a la placa, no está hecho

### g-05-fil-02-rev-a

- error grave en la nomenclatura de los proyectos: el 01 en su README dicen que es el activo, pero en Kicad es el pasivo
- no fue enviado a producción, ya que no funcionó en protoboard

## grupo-06: percusiones

- terroiblea
- martinaechavarria-stack
- Nicolas-Miranda1312
- paredesvania
- Coff4

### g-06-perc-01-rev-a

- agregamos jack de entrada de audio que reemplace la oscilación de entrada
- agregamos ground a los integrados que no están siendo usados

### g-06-perc-02-rev-a

- agregamos el detalle de las entradas de las compuertas lógicas no usadas, fueron conectadas a tierra, para definir sus estados
- C7 estaba en el esquemático pero no en la placa, tuvimos que agregarlo
- C4 le faltaba una conexión en la PCB, la agregamos
