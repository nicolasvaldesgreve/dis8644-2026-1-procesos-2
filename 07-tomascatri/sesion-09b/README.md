# sesion-09b

Viernes 15 de Mayo

---

## Apuntes
En esta clase dieron feedback de errores que ocurrieron durante el encargo del PCB y enseñaron algunas especificaciones y herramientas nuevas:
* Enseñaron cómo crear componentes personalizados; esto afecta solo al esquema. 
* **Tipos de botones** = Pushbotton y Switchbotton: Push genera un pulso constante mientras se presione el switch button, si se presiona una vez sin mantener, se mantendrá apagado o prendido dependiendo de si este está pulsado o no. También existen los 3PDT, que, desglosando su significado, es 3P (Triple Pole): Tiene 3 líneas de entrada independientes, DT (Double Throw): Cada una de esas 3 líneas puede elegir entre 2 caminos de salida, por decirlo de otra manera, sería que el botón recibe 3 entradas de diferentes partes, y estas las lleva a dos caminos posibles. Un ejemplo que encontré sería un pedal de guitarra: el interruptor 1 cambia la señal de guitarra entre el circuito del efecto o dejarla pasar directo al amplificador, el segundo interruptor conecta la salida del pedal al amplificador solo cuando el efecto está encendido, así evitando que el circuito apagado ensucie el sonido, el interruptor 3 prende o apaga un LED que avisa si el pedal se encuentra activo.
* Si queremos usar un botón en un esquema, podríamos usar **SW1 SW_SPST = switchpush 6 mm**.
* El símbolo del switch es más que nada representación, pero puede ser cualquier tipo de botón.
* **Etiqueta (se presiona la L)** = hace que se puedan conectar diferentes chips de manera simbólica.
* Se pueden producir islas de cobre, las cuales no pueden aliviar térmicamente a un pin a GND porque deben estar al menos 3 conexiones. Se representa con una X en la placa de cobre en el componente al cual se conectó.
* En el pin 13 hay un círculo al inicio del pin, es rojo, se asocia a que debe ir a GND.
* Se pueden poner componentes en la parte trasera presionando F, se debe rotar para que quede con las conexiones anteriores puestas.
* Propiedades de huellas = Se puede cambiar el modelo 3D, se usó el potenciómetro como ejemplo. Lo usamos también en el modelo del terminal block.

---

## Referentes para buscar secuenciadores:
* **piruetas.xyz**, cuatro cuadras
* **make electronic music from scratch** = libro que enseña a hacer secuenciadores
* [Hackday.com, Logic Noise: Sweet, Sweet Oscillator Sounds](https://diy-synths.snnkv.com/synths/picotracker) = Enseña también a hacer secuenciadores.


## Encargo
Investigamos sobre secuenciadores, que era lo que acordamos como grupo.

Me pareció interesante el **CD4015**, ya que siento que se escuchará bien con ese efecto parecido al 4017, pero a diferencia de este, prenden y apagan en serie.


![CD4015 funcionando](./imagenes/4015.gif)

[Video referencia](https://www.youtube.com/watch?v=UFtW6kHt54g)
