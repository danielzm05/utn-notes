## Combinacionales

En los circuitos combinacionales, **las salidas siempre van a depender de la combinación de las variables de entrada**. 

---
#### Circuito semisumador


![[6-Lógica Digital.png]]

**Tabla de Verdad**

| **A** | **B** | **Suma** | **Carry out** |
| ----- | ----- | -------- | ------------- |
| 0     | 0     | 0        | 0             |
| 0     | 1     | 1        | 0             |
| 1     | 0     | 1        | 0             |
| 1     | 1     | 0        | 1             |


---

#### Circuito sumador completo

A diferencia del semisumador, nos permite incluir en la suma de dos bits el **acarreo** de una suma anterior a través de una entrada que se llama $Cin$, con lo que ya podremos realizar cualesquiera sumas.

Según lo dicho, tendremos tres variables de entrada, a las que llamaremos A, B y la propia $Cin$ y dos de salida: **S**, la suma y Cout**, el acarreo de la misma (si procede). Entonces, la tabla de verdad quedará:

| **A** | **B** | **Cin** | **S** | **Cout** |
| ----- | ----- | ------- | ----- | -------- |
| 0     | 0     | 0       | 0     | 0        |
| 0     | 0     | 1       | 1     | 0        |
| 0     | 1     | 0       | 1     | 0        |
| 0     | 1     | 1       | 0     | 1        |
| 1     | 0     | 0       | 1     | 0        |
| 1     | 0     | 1       | 0     | 1        |
| 1     | 1     | 0       | 0     | 1        |
| 1     | 1     | 1       | 1     | 1        |

---

#### Circuito generador de paridad 

Permite la detección de error en la transmisión de información entre un emisor y un receptor de información binaria cuyo coeficiente de probabilidad de error sea menor o igual a un bit.

![[Pasted image 20250623171334.png|400]]


---

#### Circuito comparador de magnitud

Es común que se necesite comparar dos números binarios de n bits para saber si éstos son iguales, o si uno es mayor o menor que otro. Podemos simplificar el problema analizando la comparación de dos bits.

![[Pasted image 20250623171622.png]]


#### Circuito decodificador de código

Existe otro tipo de decodificadores que permiten señalar en una de sus salidas qué combinación binaria se dio en la entrada. Los decodificadores de este tipo se denominan “nX2n” (se lee “n x 2 a la n” o “n a 2 a la n”) y contemplan una salida activa para cada posible combinación de entradas.

---

#### Multiplexor 

Circuito combinacional cuya función digital es “encaminar” las señales binarias de 1 de 2E líneas posibles de entrada en una única línea de salida. La línea de entrada de dato se “elige” a partir de los valores que puedan tomar las n líneas de selección.



#### Otros tipos de circuitos combinacionales

- Circuito codificador y decodificador
- Memoria ROM
- Circuito convertidor de código
- Circuito decodificador a 7 segmentos (El de números digitales)

---
## Secuenciales

En los circuitos secuenciales, a diferencia de los combinacionales, **la salida no solo dependerá de las variables de entrada, sino también dependerá del estado en que se encontraba su salida**. Es por eso que a estos circuitos también se los conoce como circuitos con memoria, circuitos biestables o simplemente FLIP FLOP.

#### Tipos

**Circuitos secuenciales sincrónicos:** los cambios se producen cuando se establecen las entradas y además se genera una transición de señal de reloj

**Circuitos secuenciales asincrónicos:** los cambios se producen únicamente por activación de alguna de las entradas sin necesidad de una señal de reloj.


#### Biestables o flip-flops

Circuito capaz de almacenar un bit. Tiene dos salidas, una para el valor del bit almacenado y otra que representa su complemento. Su denominación sugiere que el biestable tiene sólo dos estados posibles de funcionamiento, permaneciendo en cualquiera de ellos si los niveles lógicos de las entradas no fuerzan su cambio.

![[6 Lógica Digital.png]]


> [!warning] Agregar tabla de verdad



#### Flip-flops D-Sincrónico

Su funcionamiento es muy simple. La salida sigue a la entrada, mientras el Clock esté activado por nivel, por ejemplo en 1 o por flanco.

> La D es de Delay. Demora el pasaje de dato.

![[6 Lógica Digital-1.png]]

> [!warning] Agregar tabla de verdad


#### Registro Paralelo-Paralelo

Cumplen la función de transferir la información que viene por las líneas de entrada en paralelo a salidas en paralelo. Estos registros reciben el nombre de paralelo - paralelo. En este ejemplo se utilizaron biestables D.


#### Registro de desplazamiento

Algunos registros cumplen la función de desplazar la información dentro del mismo, ingresando un nuevo bit que viene por la línea de entrada. Estos registros reciben el nombre de registros de desplazamiento o Shift Register. En este ejemplo se utilizaron biestables D.

En el set de instrucciones de una computadora hay instrucciones de desplazamiento, casi todos los procesadores actuales permiten el desplazamiento de varios bits en ambos sentidos

- **DESPLAZAMIENTOS LOGICOS**: Cuando el bit del extremo queda libre y se rellena con un 0, se indica que el registro produce un desplazamiento lógico.

- **DESPLAZAMIENTOS CIRCULARES:** Cuando en un registro de desplazamiento los n bits que se vacían en un extremo se completan con los que salen por el otro, no hay pérdida de bits, sino que éstos circulan a través del registro

- **DESPLAZAMIENTOS ARITMETICOS:** Los desplazamientos aritméticos afectan a números que pueden ser o no signados. Son parecidos a los desplazamientos lógicos, pero mantienen el signo del número. Estos desplazamientos producen una multiplicación o una división por una potencia de 2

- **DESPLAZAMIENTOS CONCATENADOS:** afectan a un conjunto concatenado de dos o más elementos, que pueden ser:

a) Dos registros
b) Un registro con el biestable de acarreo
c) Un registro con el biestable de signo
d) Combinaciones de algunos de los anteriores

--- 
## Memorias RAM


#### Tipos de RAM

| **Estáticas (SRAM)**                                         | Dinámicas (DRAM)                                      |
| ------------------------------------------------------------ | ----------------------------------------------------- |
| Tienen una matriz de flip-flop                               | Tienen una matriz capacitiva                          |
| Tienen mayor capacidad                                       | Tienen menor capacidad                                |
| Es más rápida (Tiene un tiempo de acceso de 10 nanosegundos) | Más lenta (Tiempo de acceso mayor 60/70 nanosegundos) |
| Tiene memoria caché                                          | Tiene circuito de refresco                            |

**Memoria caché:** memoria de acceso rápido y temporal que almacena copias de datos que se utilizan con frecuencia, permitiendo que la CPU acceda a ellos más rápido que si tuviera que buscarlos en la memoria principal (RAM).

**Circuito de refresco:** Circuito que hace un barrido de la memoria para refrescar la carga de los capacitores de la DRAM.

**Tiempo de acceso:** Intervalo entre el momento en que el procesador solicita un dato y el momento en que ese dato esta disponible en la salida de memoria.

