## Sistemas Numéricos

|       | Decimal | Hexa | Octal |
| ----- | :------ | :--- | ----- |
| 0000  | 0       | 0    | 0     |
| 0001  | 1       | 1    | 1     |
| 0010  | 2       | 2    | 2     |
| 0011  | 3       | 3    | 3     |
| 0100  | 4       | 4    | 4     |
| 0101  | 5       | 5    | 5     |
| 0110  | 6       | 6    | 6     |
| 0111  | 7       | 7    | 7     |
| 1000  | 8       | 8    | 10    |
| 1001  | 9       | 9    | 11    |
| 1010  | 10      | A    | 12    |
| 1011  | 11      | B    | 13    |
| 1100  | 12      | C    | 14    |
| 1101  | 13      | D    | 15    |
| 1110  | 14      | E    | 16    |
| 1111  | 15      | F    | 17    |
| 10000 | 16      | 10   | 18    |

## [[Comparación de variables]]
Dada la resta $A-B$:

|       | Enteras Sin Signo | Enteras con signo |
| ----- | ----------------- | ----------------- |
| $A=B$ | $Z=1$             | $Z=1$             |
| $A>B$ | $C=1$             | $V=S$             |
| $A<B$ | $C=0$             | $V\neq S$         |


---
## Desbordamiento:

**OVERFLOW:** Para las formas de variable enteras cuando el resultado de una operación supera los límites definidos por el rango (mayor que el máximo o menor que el mínimo), entonces es incorrecto

**UNDERFLOW:** Solo para variables Reales, cuando el resultado de una operación cae en el hueco definido por los límites inferiores del rango (valores muy cercanos a cero, del que se excluye el cero)

![[Pasted image 20250704175307.png]]


---
## [[Código de Paridad]]

Es el método más simple para la detección de un error en la transmisión de datos. Consiste en un utilizar un "bit redundante" al conjunto de bits para conocer si ocurrió un error en uno de los bits (Si hay más de un error no lo detecta). Existen dos tipos:

- **Bit de paridad:** El bit redundante indicara si la cantidad de bits 1 es par
- **Bit de paridad:** El bit redundante indicara si la cantidad de bits 1 es par

#### Paridad Vertical
La **paridad vertical** se aplica a cada **palabra (byte o bloque de bits)** por separado. Se agrega un **bit de paridad** al final de cada palabra.

#### Paridad entrelazada
La **paridad entrelazada** combina **paridad vertical y horizontal**. Se organizan los bits en una **matriz** y se agrega un **bit de paridad por fila** y un **bit de paridad por columna**.

Esto permite **detectar y localizar errores** en la intersección entre fila y columna errónea.

---
## [[Variables BCD]]
**Decimal Codificado en Binario** es una forma de representar dígitos decimales (0 a 9) mediante grupos de bits binarios. Cada dígito decimal se representa con un nibble (4 bits).

![[Pasted image 20250622195026.png| 600]]

---
#### Circuito combinacional
Tipo de circuito lógico digital en el que **la salida depende únicamente del valor actual de las entradas.**

- Circuito generador de paridad
- Circuito comparador de magnitud
- Circuito codificador y decodificador
- Memoria ROM
- Multiplexor y Demultiplexor
- Circuito convertidor de código
- Circuito sumador completo
- Circuito decodificador a 7 segmentos (El de números digitales)

#### Circuito secuencial
Circuito lógico digital en el que **la salida depende tanto de las entradas actuales como del estado anterior**, además tiene **memoria interna** que guarda el estado anterior.

##### Tipos 
**Circuitos secuenciales sincrónicos:** los cambios se producen cuando se establecen las entradas y además se genera una transición de señal de reloj

**Circuitos secuenciales asincrónicos:** los cambios se producen únicamente por activación de alguna de las entradas sin necesidad de una señal de reloj.

