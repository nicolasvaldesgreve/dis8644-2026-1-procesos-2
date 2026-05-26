# sesion-10b

Viernes 22 de Mayo, 2026.

Nota del día: buen trabajo en equipo, solo nos falta comprar ciertos componentes.

## Referentes (y otras cosas) 

- **Robert Fripp** es un músico, compositor y productor discográfico británico famoso por su trabajo en la banda de rock progresivo King Crimson. Es el único miembro constante del grupo desde su fundación, liderándolo y siendo la fuerza creativa e impulsora de su regreso a los escenarios en varias ocasiones. (wikipedia)
- **Frippertronics y Soundscapes:** Desarrollado por Robert Fripp junto a Brian Eno, es una técnica vanguardista de bucles analógicos con cintas magnéticas que más tarde evolucionó digitalmente hacia sus célebres composiciones de "paisajes sonoros" (Soundscapes).
- Frippertronics on Midnight Special 1979 - <https://youtu.be/dAECAnlnriU>
- **kaoss pad korg** es un procesadores de efectos y samplers. Su gran innovación, introducida originalmente en 1999, fue sustituir las perillas tradicionales por una pantalla táctil X-Y, permitiendo modificar múltiples parámetros de audio simultáneamente arrastrando un dedo. 
- **Radiohead** banda británica de rock alternativo originaria de Abingdon-on-Thames, Inglaterra, formada en 1985 inicialmente como una banda de versiones. La banda redefinió los límites de la composición y rompió por completo las reglas tradicionales de la puesta en escena de una banda de rock. Mientras que la mayoría de los grupos de estadios basan su directo en la fidelidad de sus discos o en la pirotecnia visual, Radiohead concibe el escenario como un laboratorio de experimentación acústica en tiempo real, donde el riesgo de error y el azar forman parte de la obra de arte. Ejemplo: <https://youtu.be/hvMql9XgIg0> en esta presentación Thom Yorke canta frente a un piano Rhodes mientras la señal de su micrófono viaja directamente al Korg Kaoss Pad de Jonny Greenwood; este captura y samplea los fragmentos de voz en tiempo real para deconstruirlos, alterar su velocidad, reproducirlos a la inversa y generar bucles caóticos a través de la pantalla táctil X-Y, culminando el tema con Greenwood manipulando en solitario los restos flotantes de la voz mientras Yorke ya ha abandonado el escenario.
- **The king of gear** página dedicada exclusivamente a documentar de forma meticulosa y exhaustiva todo el equipamiento musical, efectos, guitarras, sintetizadores y técnicas de producción que utiliza la banda Radiohead. <https://thekingofgear.com/> 
- **Akai headrush** es un pedal de delay, simulación de eco de cinta y looper lanzado a finales de los años 90 y principios de los 2000. Aunque hoy en día está descatalogado, es considerado una leyenda de culto entre los pedales de guitarra debido a su extrema robustez, su flujo de trabajo intuitivo y, muy especialmente, por ser una pieza central en el sonido de Radiohead.

## Qué hice hoy 

Cuestionamientos grupales: ¿Cual de todos los ejemplos vamos a hacer? ¿Cómo los vamos a modificar? ¿Es realizable (considerando el conocimiento que tenemos como base)?

Con mi grupo de trabajamos vimos bien la investigación que teníamos para comenzar a decidir que vamos a realizar. Decidimos quedarnos con la referencia de Hackaday. 

### Logic Noise: Filters And Drums 

<https://hackaday.com/2015/03/25/logic-noise-filters-and-drums/> de Elliot Williams. 

Creación de sintetizadores analógicos y generadores de sonido utilizando circuitos lógicos CMOS (específicamente chips de la serie 4000 como el 4069UB y el 40106).

El objetivo principal de la explicación que da es enseñar cómo manipular y esculpir el sonido mediante el diseño de filtros y cómo usarlos para crear sonidos de percusión (tambores/baterías).

### Esquemático base 

![esquematico](./imagenes/esquematico.png)

### Simulación en falstad 

(realizado por carla pino) [https://www.falstad.com/circuit/](https://www.falstad.com/circuit/circuitjs.html?ctz=DwYwlgTgBAZgvAIgIwKgFwM6IAwDpsHZICsAbAEzGpgiLm4Ac2AzEhQCwMCc7x5pSdqhAAjOiigAHMQmLZUANwiIqUALaYVAUwC0SFAD4AUFCjBJaKAA9Eg9lFL2kXclGblU8ZKjUBDW4QEqJIA9ji4XCRMgTFEqBgANogASloYYBhovgB2IFoIAPTGpqDWiI5Qdg5OAOyknjjC4TESYArNcVAYygjyUAoAJojMuGwM7JykLKSkXKTESMyFxWYgZQjM2E5Irsx8lTsNvU3I+LHnRLo11O29ZxLdjf1DCPTMDPwkXARcv7xLRRMZgs62YpAYlTqUHYBCg5HIQlgth8-mQMWCYTuqkSKTSGSyuXygJKaxsrxqriQUM2tXqSOOUFopy2VxuHQePT6gzouHB2C4fGIkxqXGYYPqxNW63Y7khpGhFSpdK8fSZSDOFxarKgbXZ8U5iheOjeHwExG+-L+xABK3MljJCOwcIYEPILrhZCOEj8AUCGPCfC4NU1BAeSQQqXSmRyeWWQLt0tlbohnCdlGVyPUqKQ6KkmLw2PDkfxMaJttJw3BzohYJr5D6Xg8jJ55G1uruof1T25r0Ycz2Czdzhqcht8YAkut4fYJjWttDOEc+jisagABZgFRxkqTsnveyDhUHw705fhgvrzeybdmADm6wq9Yhj5hS5vwGge-ns7c4wXDDfKAehzP1JQ-aVYVTaEmGghsnmA9EwIrBB2DYaFZXYCoZSbFUTiQXQAJ1W48E7LoDWecJUIYKZmBqOx3DISIJVtAB3B9aWqOFsEI3CwLYslFQmTj9Bwxo+PYg5XAqRw33Esk5kqeUlUU2TWKnClJLcecRNU+N+LobjOPIDSZNPd99OQKZNOcSkT14tSyWU2VlLYXSSgslz5SfFSzLk4Z9hEtwqx03yHMrCFAtrOU3LMCyaTlIKIrqGLgAs7CEqipUUrSxUoUPLLQr06UFOTKBD2TbL1nyvKdmrSqyUw+x02hErPUK9ziq8sgWq8l16vC6t0NcCr2ti0F51KqKRvsoqHQ05r4vTfqNgm7rFr60bUvUykoWnaLNosvbSr22dlvK91D1rM7aqiw8YTg44-NkWr7q0mcggO8b3qdeLTs+vc-0uv8-pmjqGrQ9L9yG5aoch4HF3+xBGrKl6YMHZaoMxtG7LEsKUKwjCYOwjGicJp1UxS+89yrR1Eo9DNHttKmBrFeUor2UTGdmln6zp1nltp46ETqxGUOx1xiBqzn5Ce4ypKajSmAFxWnTYJ0ldFtWoBgrWQtBsaGthbzXsdDGjZhOnTc23wQgAV3tFQpeqJ10bMqABltzMMFRaI+gSbNzPWKpAt1nGubBuhhaF2kzfJonIIR-WtsN8nOF-GdE9x7mEAUtDFQZmW8fzzjTKT8dsgULQIDQMBslvABlEA1zUMA0AdhBFVq4Ow7PTlcFUBI0FsXk6Xt4ZcDFVAEhCbItygaeYDLiuq5ruvG+b1v25szS5ckwDEj7geh9OGZUDHjYJ6WeeZ7nhek5CKAtFn14HkkcpES8Kwr7f44VhKSR+hPAwEyKgkp-6AI2PEJkJFCBBnmBQUBtoCghFtA-J+SNrhdB-jmBERwv7BGRH-YEEDlwgJvOA24V9gEdB+HUMglB3zIOMMAAo4AIDGCAA)

![falstad](./imagenes/falstad.png)

### Componentes

Chips: 

- 4069ub (UB, no sirve el BE).
- CD40106.
- Idea: usar CD4017 (para señal inicial).
- TL074 o TL072 (recomendación misaa: no usar porque se mueven en positivos y negativos, puede ser muy complicado).

Condensadores/capacitores: 

- 10 μF - 0.01 μF (que equivale a una lenteja de 103nf)
- 0.1 μF (que equivale a una lenteja de 104nf)
- 0,22 μF (que equivale a una lenteja de 224nf o 220nf).

| Código | Valor en pF | Valor en nF | Valor en µF |
|----------|------------|------------|------------|
| 101 | 100 pF | 0,1 nF | 0,0001 µF |
| 102 | 1.000 pF | 1 nF | 0,001 µF |
| 103 | 10.000 pF | 10 nF | 0,01 µF |
| 104 | 100.000 pF | 100 nF | 0,1 µF |
| 222 | 2.200 pF | 2,2 nF | 0,0022 µF |
| 224 | 220.000 pF | 220 nF | 0,22 µF |

Además de usar resistencias de 100k + un potenciometro 100k. 

### Flujo de trabajo (qué hicimos en la clase)

- Buscar información (referentes que ya teníamos) y ver que nos servía para pode realizar o replicar.
- Hablar con misaa para que nos ayude.
- dar con el articulo de hackaday.
- ver que componentes necesitamos, ver cuales tenemos y como reemplazar los que sean más dificiles de conseguir.
- buscar en el lid algunos componentes (capacitores).
- intentar hacer un ejemplo en protoboard (pero no tenemos el chip 4069UB sino que el 4069EB), no funciono pero ya nos teníamos que ir. 

## Decisiones 

1. Quedarnos con el mismo esquemático y para las variaciones hacer cambios en el tiempo de oscilación (por ejemplo hacerlo con un 555 o un 4017 en vez de utilizar el 4016) y cambiar los valores de los capacitores para generar otros tonos. 
2. Para ver bien como podiamos seguir e intentar hacer al menos un ejemplo en la clase (en protoboard) le preguntamos a cloude que podiamos reemplazar para que funcionara. Reemplazo de Cloude: <https://claude.ai/share/8e046c83-2591-44ab-91de-587412d54970>
3. Antes de la siguiente clase si o si hay que comprar los chips: 4069UB!!
4. investigar más sobre la energía negativa (que es la razón por la cuál no podemos replicar o intentar otros esquemáticos ya que todos usan chips que requieren si o si de la energía negativa para funcionar). 

## Encargo-10b

leer capítulo 6 y 7 del libro Hacia una filosofía de la fotografía, de Vilém Flusser, compartir apuntes y reflexiones críticas sobre el texto, prohibido usar inteligencia artificial, no sirve para este ejercicio.

### Desarrollo 

