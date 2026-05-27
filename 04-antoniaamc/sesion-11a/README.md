# sesion-11a

# Guía rápida filtros LPF / HPF para sintetizador (filtro de sonido)

## Alimentación del sistema

* Fuente general: 5V a 12V
* Regulación: STMicroelectronics L7805
* Salida regulada:

5V

* El regulador estabiliza:

  * osciladores
  * filtros
  * LM324
  * evita ruido y variaciones

---

# Conceptos básicos

## VIN

Señal de entrada:

* oscilador
* audio
* generador de funciones

## VOUT

Señal filtrada de salida.

## GND

Tierra común del sistema.

---

# Frecuencia de corte

Punto donde el filtro empieza a atenuar frecuencias.

Fórmula general:

f_c=\frac{1}{2\pi RC}

Variables:

* R = resistencia
* C = capacitor

---

# Low Pass Filter (LPF)

## Función

* deja pasar frecuencias bajas
* reduce frecuencias altas

## Circuito básico

```text
VIN ── R ──┬── VOUT
           |
           C
           |
          GND
```

## Funcionamiento

* capacitor deriva agudos a tierra
* sonido más oscuro/suave

---

# LPF activo del proyecto

## Componentes principales

| componente | valor |
| ---------- | ----- |
| R1         | 10k   |
| R2         | 10k   |
| R3         | 10k   |
| C1         | 370nF |
| C2         | 23nF  |
| Op-Amp     | LM324 |

## Características

* filtro activo
* usa alimentación
* utiliza realimentación
* más estable y profesional

---

# High Pass Filter (HPF)

## Función

* deja pasar frecuencias altas
* reduce frecuencias bajas

## Circuito básico recomendado

```text
VIN ── C ──┬── VOUT
           |
           R
           |
          GND
```

## Valores sugeridos

| componente | valor |
| ---------- | ----- |
| R          | 10k   |
| C          | 100nF |

Frecuencia aproximada:

f_c\approx159Hz

---

# HPF variable (recomendado)

## Circuito

```text
VIN ── C ──┬── VOUT
           |
         POT
           |
          GND
```

## Componentes

| componente    | valor |
| ------------- | ----- |
| capacitor     | 100nF |
| potenciómetro | 10k   |

## Qué hace el potenciómetro

Controla:

* resistencia
* frecuencia de corte

## Resultado

* cutoff bajo → sonido completo
* cutoff alto → sonido brillante/delgado

---

# Diferencia entre filtros

| Tipo | Deja pasar | Atenúa |
| ---- | ---------- | ------ |
| LPF  | graves     | agudos |
| HPF  | agudos     | graves |

---

# Filtros pasivos vs activos

| Tipo | Usa op-amp | Alimentación | Complejidad |
|---|---|---|
| Pasivo | no | no | baja |
| Activo | sí | sí | media |

---

# LM324

Características:

* op-amp utilizado en el proyecto (amplificador operacional -> chip que amplifica la diferencia de voltaje entre sus dos terminales de entrada, produciendo una señal de salida mucho mayor.)  
* funciona con 5V  
* sirve para:

  * amplificación  
  * filtros activos  
  * buffers  

Alimentación:

* VCC = +5V  
* GND = 0V  

---

# Recomendación para el proyecto

## Circuito 1

LPF activo (actual)

## Circuito 2

HPF variable

* complementa el LPF
* fácil de protoboard
* fácil de escuchar y medir
* modular para sintetizador

---

# Ideas futuras

* filtro variable con cutoff
* resonancia
* múltiples etapas RC
* control por potenciómetro
* integración con VCO/osciladores 
