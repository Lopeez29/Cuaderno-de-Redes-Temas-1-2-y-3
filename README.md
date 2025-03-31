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

#### Modulaciones aplicadas:

- Modulación en Fase

- Modulación en Frecuencia (FM)

#### b) Recuperación de la información:

Para extraer ambas señales, se deben aplicar filtros adecuados:


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

# Ejercicio 8 ✅
## - Transmisión vía Satélite

# Enunciado
Un sistema satélite divide la información de la capa 3 en bloques de 1904 bits, a los que añade una cabecera de 64 bits.
Cada trama tarda en transmitirse 20 ms y la latencia del satélite es de 85 ms.
Se desea saber cuánto tiempo se tardará en transmitir 5 MBytes de información.

# Datos
Tamaño de bloque de datos = 1904 bits

Cabecera por trama = 64 bits

Tamaño total por trama = 1904 + 64 = 1968 bits

Tiempo de transmisión por trama = 20 ms

Latencia satélite (ida) = 85 ms

Total de datos a enviar = 5 MBytes = 5 × 1024 × 1024 Bytes = 5,242,880 Bytes = 41,943,040 bits
## Cálculos
1. Conversión de datos a bits:
5 MBytes = 5 × 1024 × 1024 Bytes = 5,242,880 Bytes
5,242,880 Bytes × 8 = 41,943,040 bits

2. Número de tramas necesarias:
Cada trama transporta 1904 bits de datos útiles (sin contar la cabecera)
Número de tramas = ceil(41,943,040 / 1904) = 22,040 tramas

3. Tiempo de transmisión de todas las tramas:
Cada trama tarda 20 ms
Tiempo de transmisión = 22,040 × 20 = 440,800 ms

4. Tiempo total con latencia:
Latencia del satélite = 85 ms (se suma una sola vez)
Tiempo total = 440,800 + 85 = 440,885 ms

5. Conversión a segundos:
440,885 ms ÷ 1000 = 440.885 segundos

   # Ejercicio 9
   ## -  Resultado de un paquete de datos

   
   # Enunciado
Calcular el resultado de un paquete de datos “1111011101010101” en un sistema de 
enlace de datos con las siguientes especificaciones: 
• Secuencia de inicio de trama “010101010”. 
• Protección frente a errores H(7,4). 
• Tamaño máximo por trama de 4 bytes.


en un sistema de enlace de datos con las siguientes especificaciones:

1. **Secuencia de inicio de trama**: `010101010` (9 bits)  
2. **Protección frente a errores**: Código Hamming \[7,4\] (cada 4 bits de datos se codifican en 7 bits)  
3. **Tamaño máximo por trama**: 4 bytes (32 bits de datos).  
   - En este caso, solo tenemos 16 bits de datos, por lo que todo cabe en una única trama.

## 1. División de los datos en nibbles (4 bits)

Los 16 bits se dividen en 4 grupos de 4 bits:
Nibble 1: 1111 Nibble 2: 1011 Nibble 3: 0101 Nibble 4: 0101

## 2. Codificación Hamming (7,4)

El **Hamming (7,4)** agrega 3 bits de paridad a cada nibble, generando 7 bits totales por cada grupo de 4 bits.

### 2.1 Convenciones usadas

- Se asume **paridad par**
- Orden típico de bits en H(7,4):
Posición: 1 2 3 4 5 6 7 Tipo: P1 P2 D1 P3 D2 D3 D4
- `D1, D2, D3, D4` son los 4 bits originales de datos.
- `P1, P2, P3` son bits de paridad que cubren distintas posiciones.

### 2.2 Cálculo de paridades

**Fórmulas de paridad** (para paridad par):
- `P1` cubre bits 1, 3, 5, 7
- `P2` cubre bits 2, 3, 6, 7
- `P3` cubre bits 4, 5, 6, 7

#### Nibble 1: `1111`
- Datos: D1=1, D2=1, D3=1, D4=1
- Distribución en posiciones:
- (1) P1=? (2) P2=? (3) D1=1 (4) P3=? (5) D2=1 (6) D3=1 (7) D4=1
- - Cálculo de paridades:
- P1 cubre (1,3,5,7) = P1,1,1,1 → suma de datos = 1+1+1 = 3 (impar) → P1 = 1 para que total sea par.
- P2 cubre (2,3,6,7) = P2,1,1,1 → suma de datos = 1+1+1 = 3 (impar) → P2 = 1.
- P3 cubre (4,5,6,7) = P3,1,1,1 → suma de datos = 1+1+1 = 3 (impar) → P3 = 1.

- Resultado Hamming:  
(1)1 (2)1 (3)1 (4)1 (5)1 (6)1 (7)1 = 1111111

#### Nibble 2: `1011`
- Datos: D1=1, D2=0, D3=1, D4=1
- Distribución en posiciones:
(1) P1=? (2) P2=? (3) D1=1 (4) P3=? (5) D2=0 (6) D3=1 (7) D4=1
- Cálculo de paridades:
- P1 cubre (1,3,5,7) = P1,1,0,1 → suma de datos = 1+0+1 = 2 (par) → P1 = 0.
- P2 cubre (2,3,6,7) = P2,1,1,1 → suma de datos = 1+1+1 = 3 (impar) → P2 = 1.
- P3 cubre (4,5,6,7) = P3,0,1,1 → suma de datos = 0+1+1 = 2 (par) → P3 = 0.

- Resultado Hamming:  
(1)0 (2)1 (3)1 (4)0 (5)0 (6)1 (7)1 = 0110011

#### Nibble 3: `0101`
- Datos: D1=0, D2=1, D3=0, D4=1
- Distribución en posiciones:
(1) P1=? (2) P2=? (3) D1=0 (4) P3=? (5) D2=1 (6) D3=0 (7) D4=1
- Cálculo de paridades:
- P1 cubre (1,3,5,7) = P1,0,1,1 → suma de datos = 0+1+1 = 2 (par) → P1 = 0.
- P2 cubre (2,3,6,7) = P2,0,0,1 → suma de datos = 0+0+1 = 1 (impar) → P2 = 1.
- P3 cubre (4,5,6,7) = P3,1,0,1 → suma de datos = 1+0+1 = 2 (par) → P3 = 0.

- Resultado Hamming:  
(1)0 (2)1 (3)0 (4)0 (5)1 (6)0 (7)1 = 0100101

#### Nibble 4: `0101`
- Es igual al anterior (`0101`), por lo que el resultado Hamming también es `0100101`.

## 3. Unir los nibbles codificados

Cada nibble se convierte en 7 bits, así que el bloque de datos codificado completo (28 bits) es:
1111111 0110011 0100101 0100101

## 4. Añadir la secuencia de inicio de trama

La **secuencia de inicio** es `010101010` (9 bits). Se antepone al bloque codificado:

010101010 (inicio) + 1111111011001101001010100101 (datos codificados)

## 5. Resultado final

El **paquete de salida** (o trama) es la concatenación de la secuencia de inicio y los 28 bits de datos codificados:

0101010101111111011001101001010100101

- **Longitud total**: 9 bits de cabecera + 28 bits de datos codificados = 37 bits.

---

## Resumen

1. Se dividió el mensaje original de 16 bits en 4 nibbles de 4 bits.
2. Cada nibble se codificó con Hamming (7,4), generando 7 bits por nibble.
3. Se unieron los 4 nibbles codificados (28 bits totales).
4. Se antepuso la secuencia de inicio `010101010` (9 bits).
5. El resultado final es una única trama de 37 bits:

0101010101111111011001101001010100101



# Ejercicio 10
## calcular la trama resultante


# Enunciado
 Un fabricante indica que su sistema integra un CRC-8 con el siguiente polinomio 
generador: 𝐺(𝑥) = 𝑥^8 + 𝑥^7 + 𝑥^2 + 1. Plantear los pasos que se deben realizar para 
calcular la trama resultante, considerando que el CRC se aplica al final de la trama 2 
del ejercicio anterior. 

# Cálculo de la trama resultante con CRC-8 (Polinomio \(x^8 + x^7 + x^2 + 1\))

En este ejercicio se parte de la **trama final** obtenida en el anterior (la “Trama 2”), a la cual ahora se le debe añadir un **CRC-8** calculado con el polinomio generador:
\[
G(x) \;=\; x^8 \;+\; x^7 \;+\; x^2 \;+\; 1
\]

> **Nota**: La trama de entrada (del ejercicio anterior) tenía 37 bits. A estos 37 bits se les aplicará el proceso estándar de CRC-8:  
> 1. Se añaden 8 bits (ceros) de relleno al final.  
> 2. Se realiza la división polinomial (XOR) entre ese bloque de datos (ahora de 45 bits) y el polinomio generador \(G(x)\).  
> 3. El **residuo** (remainder) resultante de 8 bits es el CRC-8.  
> 4. Dicho CRC (8 bits) se anexa al **final** de la trama original de 37 bits, obteniendo así la **trama definitiva** de 45 bits.

---

## 1. Polinomio generador en notación binaria

El polinomio:
\[
G(x) = x^8 + x^7 + x^2 + 1
\]
se representa habitualmente en binario (9 bits si contamos el bit de \(x^8\) hasta el de \(x^0\)) como:
110000101


---

## 2. Trama a la que se aplica el CRC-8

Supongamos que la **trama** obtenida en el ejercicio anterior (Trama 2) es (37 bits):
0101010101111111011001101001010100101
Para aplicar un CRC de grado 8 (CRC-8), se deben realizar los pasos siguientes:

1. **Convertir la trama en una secuencia binaria** (ya la tenemos de 37 bits).  
2. **Anexar 8 ceros** al final (uno por cada bit de CRC que vamos a calcular).  
   - Ahora el bloque temporal a dividir tiene 37 + 8 = 45 bits.
3. **Dividir** ese bloque de 45 bits entre el polinomio generador \(G(x)\) (mediante XOR, sin acarreo).  
   - El método típico es la “división polinomial” bit a bit: se alinea el polinomio con el primer 1 significativo, se hace XOR, se avanza un bit y se repite hasta recorrer los 45 bits.  
4. **Obtener el residuo (remainder)** de 8 bits que queda tras la división.  
5. **Anexar** esos 8 bits (CRC) a la **trama original** de 37 bits. El resultado final será de 37 + 8 = 45 bits.

---
## 4. Resultado final

- **CRC-8**: es un valor de 8 bits, que se representa en binario u ocasionalmente en hexadecimal.  
- La **trama definitiva**:  


- **37 bits** → Datos originales  
- **8 bits**  → CRC calculado

Por lo tanto, la trama completa tiene:

37 bits + 8 bits = **45 bits en total**

Se puede expresar de la siguiente manera:

**Trama final** = [37 bits de datos] + [8 bits de CRC] = 45 bits


Resumen del calculo:

1. **Tomar la trama de 37 bits**:  
0101010101111111011001101001010100101
   2. **Añadir 8 ceros** (bits de relleno) → 45 bits.  
3. **Dividir** por \(G(x) = 110000101\) (XOR).  
4. **El residuo** (8 bits) se llama CRC.  
5. **Anexar** ese CRC al final de la trama original.

# Ejercicio 11
## Nº Errores para H(15,11) y CRC-32


# Enunciado
¿Cuántos errores pueden llegar a corregir la codificación H(15,11) y el CRC-32? 

# Respuesta
- Hamming(15,11): puede corregir 1 bit erróneo por bloque de 15 bits (y detectar hasta 2 bits erróneos).

- CRC-32: no corrige errores por sí mismo; es un método de detección de errores muy robusto (con baja probabilidad de no detectar errores), pero no los corrige.

# Ejercicio 12
## datos útiles que se han transmitido


# Enunciado
Se recibe la trama “1111111101011010101011” y se conoce que el protocolo está 
constituido por una cabecera “11111111” y que los datos están codificados con 
H(14,10), ¿cuáles son los datos útiles que se han transmitido? 

---

# Resultado 
se recibe una trama binaria: 111111101010101010101

y se sabe que:

1. El **protocolo** añade una **cabecera** de 8 bits, indicada como `11111111`.
2. Los **datos** van codificados mediante un **Hamming(14,10)**, es decir, cada bloque de 14 bits contiene 10 bits de información y 4 bits de paridad.

El objetivo es **determinar los 10 bits de datos originales** (los “datos útiles”).

---

- La cabecera ocupa los **primeros 8 bits**.
- Aunque en la trama recibida se observa `11111110` al inicio, se asume (según la descripción del protocolo) que la intención es que esos 8 bits correspondan a `11111111` (pudiera haber un error de un bit en la cabecera, pero el ejercicio no se centra en ello).

Tomando la idea de que los **8 bits de cabecera** son fijos (`11111111`), se separan de la secuencia.  
En total, la trama tiene 21 bits, por lo que, tras la cabecera, **restan 13 bits**.  

Para H(14,10) harían falta **14 bits** de datos codificados. Es posible que exista un bit perdido o un pequeño desajuste en el enunciado. Aun así, se entiende que el bloque Hamming debería ser de 14 bits.
**H(14,10)**, **siempre** habrá **10 bits** de información
Tras calcular la paridad junto con los datos he llegado a la conclusión de que tal como está redactado el ejercicio presenta un ligero desfase (21 bits en vez de 22), lo que sugiere que puede faltar un bit en la trama recibida o existir un error en la cabecera.
(- **Cabecera**: 8 bits (`11111111`).  
- **Bloque Hamming(14,10)**: 14 bits totales, de los cuales **10** son datos útiles y **4** son de paridad.  )

---


# Ejercicio 13
## Protocolo capa de enlace 
# Enunciado
 ¿A qué protocolo de la capa de enlace de datos corresponde el siguiente esquema 
temporal? 


![image](https://github.com/user-attachments/assets/344b244a-09af-4c7e-b3ed-8e1d81ebf742)


# Respuesta 
El diagrama muestra un intercambio de tramas entre dos estaciones (A y B).
Se observa que:
- A envía “Frame 0” a B.  
- B responde con “ACK 1”, indicando que espera la próxima trama con número de secuencia 1.  
- A envía “Frame 1”.  
- B responde con “ACK 0”, indicando que espera la siguiente trama con número de secuencia 0.  
- El proceso se repite.
  Por tanto, se trata del protocolo Stop-and-Wait ARQ (Alternating Bit Protocol)


  # Ejercicio 14
  ## Adaptabilidad del Alternating Bit protocol
  # Enunciado

  ¿Se puede aplicar el protocolo del ejercicio anterior en el siguiente escenario?

  
  ![image](https://github.com/user-attachments/assets/4497623d-8f24-41c6-b2a1-3ea22e02e159)


  # Respuesta
  Se observa que:
  - El **Emisor** envía:
  - **Frame 0**, con número de secuencia \(S=0\).
  - **Frame 1**, con número de secuencia \(S=1\), que se **pierde** en la red.
- El **Receptor**:
  - Recibe correctamente el **Frame 0** y envía un **ACK 1**.
  - No recibe el **Frame 1**, así que no puede responder con el **ACK 0** esperado.
    Por tanto, **sí** se puede aplicar el mismo protocolo en este escenario: el proceso de temporización y reenvío cubre la situación de que una trama se pierda en el camino.
  - El **Stop-and-Wait ARQ** (Alternating Bit Protocol) **funciona** incluso si hay tramas perdidas o ACKs perdidos.
- La clave es el **temporizador** en el emisor, que provoca el **reenvío** cuando no llega el ACK esperado.


# Ejercicio 15 
## Diagrama de ventana deslizante 
# Enunciado 
Dibujar un diagrama de ventana deslizante con un receptor con buffer para tres tramas 
y un transmisor que dispone de 5 tramas desordenadas que llegan en el orden 0, 3, 2, 
4, 1. 

(Diagrama)


| Llegan       | 0   | 3     | 2       | 4         | 1            |
|--------------|-----|-------|---------|-----------|--------------|
| Ventana      | ↓   | ↓     | ↓       | ↓         | ↓            |
| Espera       | 0 → 1 → 5 (tras liberar 1,2,3,4)                         |
| Buffer       | [ ] | [3]   | [3,2]   | [3,2,4]   | [ ]          |
| Entregados   | 0   | -     | -       | -         | 1,2,3,4      |


# Ejercicio 16 
## Canal coaxial con FMD
# Enunciado
16. Un canal coaxial con FDM con una tasa de transmisión de 500 Mbit/s, con una longitud media de trama de 
1
𝜇
=
12584
μ
1
​
 =12584 bits y una tasa de llegada de trama 
𝜆
=
20000
λ=20000 tramas/s:

a) ¿Qué retardo tendrá?
D = 1 / (μ - λ)

Donde:

- **μ** es la tasa de servicio (en tramas por segundo)
- **λ** es la tasa de llegada (también en tramas por segundo)
- **D** es el retardo promedio en segundos

Primero calculamos μ a partir de la tasa de transmisión y el tamaño promedio de trama:

μ = (500 × 10⁶ bits/s) / (12584 bits/trama) ≈ 39725.37 tramas/s



Luego aplicamos la fórmula del retardo:


D = 1 / (39725.37 - 20000) ≈ 5.07 × 10⁻⁵ s = 50.7 μs



**Resultado final**:  
**Retardo medio ≈ 50.7 microsegundos**


b) Si lo comparten entre 256 usuarios, ¿cuántas portadoras serán necesarias?

256 portadoras


c) ¿Cuánto tiempo tardará un nodo en detectar una colisión?


T = 12584 bits / 500,000,000 bits/s ≈ 25.17 μs

---


# Ejercicio 17 
## - Codificación Manchester y Manchester Diferencial

# Enunciado

Representar la trama `1111111101011010101011` con codificación:
- Manchester
- Manchester Diferencial

 **Indicar las unidades y magnitudes en los ejes.**

---

## Codificación Manchester

La codificación Manchester consiste en una transición en el **medio del bit**:
- Bit `1`: transición de **bajo a alto**.
- Bit `0`: transición de **alto a bajo**.

Cada bit se representa en **1 unidad de tiempo**, con cambio de nivel en la mitad del intervalo.

### Ejemplo de representación (simplificada):

| Bit     | Nivel lógico | Codificación Manchester |
|---------|--------------|--------------------------|
| `1`     | ↧↥           | Bajo → Alto              |
| `0`     | ↥↧           | Alto → Bajo              |
| ...     | ...          | ...                      |

---

## Codificación Manchester Diferencial

En Manchester diferencial:
- **Bit 1**: hay **transición al inicio** del bit.
- **Bit 0**: **no hay transición** al inicio.
Siempre hay una transición en la mitad del bit (igual que en Manchester estándar).

### Lógica:
- Se parte de un nivel inicial (por ejemplo, bajo).
- Se alterna o mantiene dependiendo del bit recibido.

---

## Representación gráfica

- **Eje X**: Tiempo (en unidades de bit)
- **Eje Y**: Nivel de voltaje (por ejemplo, +V / 0V)
- El gráfico debe mostrar los cambios de nivel según las reglas de cada codificación.

---

 **Nota:** Para una visualización completa, se recomienda usar herramientas como Python con `matplotlib` o software como Wireshark (en modo simulación) para representar los cambios de señal.





