El **código de paridad** es un método simple de **detección de errores** en la transmisión de datos. Consiste en añadir un **bit de paridad** a un conjunto de bits, con el fin de que la cantidad total de bits con valor 1 cumpla una determinada condición.

Existen dos tipos:

- **Paridad par**: el número total de bits 1 (incluyendo el bit de paridad) debe ser **par**.
- **Paridad impar**: el número total de bits 1 (incluyendo el bit de paridad) debe ser **impar**.

Este método permite detectar si ocurrió **un error de un solo bit**, aunque no permite corregirlo.

---

## Paridad Vertical
La **paridad vertical** se aplica a cada **palabra (byte o bloque de bits)** por separado. Se agrega un **bit de paridad** al final de cada palabra.

**Ejemplo:**

Supongamos que transmitimos 4 palabras de 7 bits:

|Palabra original|Cant. de 1|Bit de paridad|Palabra transmitida|
|---|---|---|---|
|1010101|4|0|10101010|
|1100001|3|1|11000011|
|0111010|4|0|01110100|
|0001111|4|0|00011110|

En todos los casos, el número total de 1 (incluyendo el bit de paridad) es par.
Si al recibir una palabra el total de 1 es impar, se detecta un error.

---

## Paridad Entrelazada (Bidimensional)

La **paridad entrelazada** combina **paridad vertical y horizontal**. Se organizan los bits en una **matriz** (por ejemplo, 4x7), se agrega un **bit de paridad por fila** y un **bit de paridad por columna**.

Esto permite **detectar y localizar errores** en la intersección entre fila y columna errónea.

### Ejemplo:

Matriz de datos originales (4 filas, 7 columnas):

```
Fila 1:  1 0 1 0 1 0 1
Fila 2:  1 1 0 0 0 0 1
Fila 3:  0 1 1 1 0 1 0
Fila 4:  0 0 0 1 1 1 1
```

- Se agrega un **bit de paridad por fila** (paridad par)
    
- Se agrega una **fila extra con bits de paridad por columna**

Resultado:

```
1 0 1 0 1 0 1 | 0
1 1 0 0 0 0 1 | 1
0 1 1 1 0 1 0 | 0
0 0 0 1 1 1 1 | 0
--------------
1 0 0 0 0 0 1
```

Este sistema permite detectar y localizar un error puntual en la intersección de una fila y una columna con paridad incorrecta.

---

## Ventajas y limitaciones

**Ventajas:**

- Simple de implementar.
- Detección de errores en transmisiones digitales.

**Limitaciones:**

- No detecta errores si hay un número par de bits erróneos.
- No permite corregir errores (solo detectarlos).
