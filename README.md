[# Cuaderno-de-Redes-Temas-1-2-y-3](https://github.com/Lopeez29/Redes-CuadernoDeEjerciciosParte1.git
# Redes Cuaderno De Ejercicios Parte 1.
#### Alumno: López Díaz Álvaro.

# Ejercicio 1

# Cálculo del Ancho de Banda y Tipo de Medio Guiado

## Enunciado

**1. Para un sistema de comunicaciones con 17 niveles de señal, que funciona en banda base, calcular el máximo ancho de banda si el ruido es despreciable y la tasa de transmisión es de 10 Mbits/s. ¿Qué tipo de medio guiado se podría utilizar para el sistema?**

## Consideraciones

- Se asume que el ruido es despreciable, por lo que la ecuación de Nyquist puede aplicarse para el cálculo del ancho de banda.
- Se analizarán diferentes medios guiados en función de su capacidad de transmisión y compatibilidad con la banda base.

## Resolución

-----------------------------------------------------------------------------------------------------------------
# Ejercicio 2

# Cálculo de la Tasa de Transmisión Máxima en un Canal Óptico con Fibra

## Enunciado
Determinar la tasa de transmisión máxima en un canal óptico con fibra que cumple con las siguientes características:

- **Ancho de banda:** 1 THz
- **Conversores optoeléctricos:** 100 Gbaudios
- **Relación señal a ruido (SNR):** 15 dB
- **Modulación utilizada:** 4 símbolos en cuadratura

## Resolución

## Cálculo de la Tasa de Transmisión Máxima
La tasa de transmisión máxima se puede calcular utilizando la ecuación de Shannon:

\[ C = B \( log_2 \) (1 + SNR) ]

Donde:
- \( B \) es el ancho de banda del canal en Hz
- \( SNR \) es la relación señal a ruido expresada en valor lineal 
- \( log_2 \) representa el logaritmo en base 2.

--------------------------------------------------------------------------------------------------------------------------------------------

# Ejercicio 3

## Enunciado

Si en el sistema anterior se introduce un conector de fibra con un **20% de pérdidas**, responder a las siguientes cuestiones:

- ¿Se verá afectada la tasa de transmisión máxima?
- ¿Qué velocidad máxima se tendrá en la salida?

## Resolución

--------------------------------------------------------------------------------------------------------------------------------------------



---

# Análisis de Diagramas de Constelación

# Ejercicio 4  ✅

## Enunciado:
Indicar el tipo de modulación que se está utilizando y los problemas que plantea en los casos **B** y **C**.



## Análisis

### Caso A

- **Tipo de modulación:** 16-QAM (Quadrature Amplitude Modulation).  
- **Resolución:** Se observan 16 puntos claramente definidos y distribuidos en una cuadrícula regular. Esto corresponde a 16 combinaciones posibles de amplitud en fase (I) y cuadratura (Q).



### Caso B

- **Tipo de modulación:** 16-QAM.  
- **Problema:** Ruido en el canal.  
- **Resolución:** Aunque se mantiene la estructura de 16 puntos, los símbolos están dispersos en torno a sus posiciones ideales. Esto sugiere la presencia de ruido aditivo (como ruido blanco gaussiano), que afecta la claridad y puede provocar errores de decodificación.



### Caso C

- **Tipo de modulación:** 16-QAM.  
- **Problema:** Desajuste de fase (rotación de constelación).  
- **Resolución:** La constelación está girada respecto a los ejes I y Q. Esto ocurre por una desincronización en la fase del oscilador local del receptor, lo cual dificulta la correcta interpretación de los símbolos y puede causar errores graves.
  
  ![image](https://github.com/user-attachments/assets/7be312c8-06ca-41e5-8d2c-a0556b6a18c3)


--------------------------------------------------------------------------------------------------------------------------------------------

# Ejercicio 5 ✅

## Modulación de Señales

# Enunciado
- Sabiendo que se transmiten dos señales de forma simultánea y que se aplican dos modulaciones diferentes:
a) Indicar qué dos modulaciones se están aplicando.
b) Recuperar la información de ambas señales.

## Resolución
#### a) Identificación de las modulaciones:

Analizando la señal en la imagen, se pueden observar dos tipos de variaciones:

Variación en la frecuencia: hay segmentos donde la frecuencia (cantidad de oscilaciones por segundo) cambia bruscamente.

Variación en la amplitud: varía de forma suave.

#### Modulaciones aplicadas:

- Modulación en Amplitud (AM)

- Modulación en Frecuencia (FM)

#### b) Recuperación de la información:

Para extraer ambas señales, se deben aplicar filtros adecuados:

Recuperación de la señal AM:

Aplicar un detector de envolvente para extraer la envolvente de la señal modulada.

La envolvente corresponde directamente a la señal original moduladora.

Recuperación de la señal FM:

Aplicar un discriminador de frecuencia (demodulador FM) para detectar los cambios de frecuencia.

Este proceso extrae la señal que moduló la frecuencia.

![image](https://github.com/user-attachments/assets/a44b86c3-1dc8-4995-bda4-9a9a9b92bd7c)


--------------------------------------------------------------------------------------------------------------------------------------------

# Ejercicio 6
## - Longitudes de onda en redes WDM
# Enunciado
Indicar las longitudes de onda que se transmiten en cada uno de los puntos marcados en el esquema.

## Resolución
Descripción del esquema:
El diagrama muestra una red WDM (Multiplexación por División en Longitud de Onda), donde:

Fiber 1 a Fiber 4: cada fibra lleva una longitud de onda distinta:

Fiber 1 → λ₁

Fiber 2 → λ₂

Fiber 3 → λ₃

Fiber 4 → λ₄

Combiner: combina todas las longitudes de onda en una sola fibra compartida:

Salida del combiner: λ₁ + λ₂ + λ₃ + λ₄

Splitter: divide la señal combinada en varias fibras.
Como es un splitter pasivo, todas las salidas contienen todas las longitudes de onda.

Es decir, todas las salidas marcadas con flechas negras llevan de manera simultánea las longitudes de onda.
![image](https://github.com/user-attachments/assets/79abddf9-f821-4831-992c-a38ec573bea8)


--------------------------------------------------------------------------------------------------------------------------------------------

)
