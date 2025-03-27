[# Cuaderno-de-Redes-Temas-1-2-y-3](https://github.com/Lopeez29/Cuaderno-de-Redes-Temas-1-2-y-3.git)
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
  

![image](https://github.com/user-attachments/assets/b575c680-9009-42da-a145-a87e91b415d2)


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
![image](https://github.com/user-attachments/assets/cff04e5d-2cf7-41c3-a8cc-87bab896170d)





--------------------------------------------------------------------------------------------------------------------------------------------

# Ejercicio 6 ✅
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

![image](https://github.com/user-attachments/assets/e6f13af4-076c-4047-b1a1-806dd6fe5baf)




--------------------------------------------------------------------------------------------------------------------------------------------

# Ejercicio 7 (Revisar)
## - Encapsulamiento en una pila de protocolos de 4 capas.
# Enunciado
Se considera una pila de protocolos de 4 capas. La capa 4 envía un bloque de 1 Kbyte. La capa 3 añade cabeceras de 256 bits y cada paquete es de 512 bytes. La capa 2 añade cabeceras de 512 bits y el campo de datos de las tramas son de 128 bytes. La capa 1 añade a cada 30 bytes de datos: 32 bits de comienzo, un byte de parada y 16 bits de CRC. Dibujar todo el proceso de encapsulamiento del sistema transmisor y calcular la eficiencia del sistema.
## Diagrama del proceso de encapsulamiento:
![image](https://github.com/user-attachments/assets/f6c61c71-6be7-4134-8d57-bc2fb83f2d77)
## Resolución
### Capa 4
- Datos enviados: 1024 bytes
- Cabecera: 256 bits = **32 bytes**
- Los datos se dividen en dos bloques de 480 bytes
- Total capa 4: 2 × (480 + 32) = **1024 bytes**

### Capa 3
- Cabecera: 256 bits = **32 bytes**
- Cada paquete: 512 bytes = 480 datos + 32 cabecera
- Cada uno se encapsula con cabecera de 64 bytes (512 bits)
- Total capa 3: 2 × (512 + 64) = **1152 bytes**

### Capa 2
- Cabecera: 512 bits = **64 bytes**
- Cada trama: 128 bytes de datos
- Los 1152 bytes se dividen en: 1152 / 128 = **9 tramas**
- Cada trama lleva 64 bytes extra ⇒ 9 × (128 + 64) = **1728 bytes**

### Capa 1
- Cada 30 bytes de datos:
  - 4 bytes inicio
  - 2 bytes CRC
  - 1 byte parada ⇒ total = **7 bytes de sobrecarga**
- 1728 bytes totales se dividen en 30 bytes → 1728 / 30 = **57.6 ≈ 58 bloques**
- Cada uno tiene 30 + 7 = **37 bytes**
- Total: 58 × 37 = **2146 bytes transmitidos**

  ## Calculo de eficiencia
  
![image](https://github.com/user-attachments/assets/25d7e18c-8ac5-4881-b18e-a84b0387a691)



