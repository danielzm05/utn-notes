Son lenguajes para expresar cantidades. Tienen elementos (símbolos: dígitos y cero) y reglas para combinarlos. Existen:

- **Sistemas de numeración aposicionales:**  el valor del símbolo es absoluto.

- **Sistemas de numeración posicionales:** se caracterizan por asignar a cada símbolo un "peso" que depende de la posicón que ocupa. El valor de un número es la suma de cada dígito multiplicado por su peso.

$N=anbn+an−1bn−1+⋯+a1b1+a0b0+a−1b−1+…N = a_nb^n + a_{n-1}b^{n-1} + \dots + a_1b^1 + a_0b^0 + a_{-1}b^{-1} + \dots$

Donde $a_i$ es el coeficiente (dígito) y $b$ es la base.

**Base de un sistema numérico:** indica cuántos símbolos únicos (dígitos) se utilizan para representar números

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

---

## Sistemas de Numeración

### Decimal (Base 10)

- Símbolos: 0 al 9
- Ejemplo: $1025_{10} = 1 \cdot 10^3 + 0 \cdot 10^2 + 2 \cdot 10^1 + 5 \cdot 10^0$

### Binario (Base 2)

- Símbolos: 0 y 1 (bits)
- Unidades en las que trabaja la computadora:
    - 4 bits = 1 nibble
    - 8 bits = 1 byte
    - 16 bits = 1 word
    - 32 bits = 1 dword
    - 64 bits = 1 qword

- Ejemplo: $10112=1⋅23+0⋅22+1⋅21+1⋅20=11101011_2 = 1 \cdot 2^3 + 0 \cdot 2^2 + 1 \cdot 2^1 + 1 \cdot 2^0 = 11_{10}$
### Octal (Base 8)

- Símbolos: 0 al 7
- Ejemplo:
$3758=3⋅82+7⋅81+5⋅80=25310375_8 = 3 \cdot 8^2 + 7 \cdot 8^1 + 5 \cdot 8^0 = 253_{10}$

### Hexadecimal (Base 16)

- Símbolos: 0 al 9 y A=10, B=11, ..., F=15
- Ejemplo:

$2B816=2⋅162+11⋅161+8⋅160=696102B8_{16} = 2 \cdot 16^2 + 11 \cdot 16^1 + 8 \cdot 16^0 = 696_{10}$

---

## Conversión entre Sistemas

### Decimal a otra base (parte entera): Divisiones sucesivas

**Ejemplo:** Convertir $100_{10}$ a binario

- $100 \div 2 = 50$, residuo 0
- $50 \div 2 = 25$, residuo 0
- $25 \div 2 = 12$, residuo 1
- $12 \div 2 = 6$, residuo 0
- $6 \div 2 = 3$, residuo 0
- $3 \div 2 = 1.5$,  residuo 1
- $1 \div 2=0.5$, residuo 1

Resultado: $100_{10} = 1100100_2$

### Parte fraccionaria: Multiplicaciones sucesivas

Ejemplo: Convertir $0.2_{10}$ a binario

- $0.2 \times 2 = 0.4 \Rightarrow 0$
- $0.4 \times 2 = 0.8 \Rightarrow 0$
- $0.8 \times 2 = 1.6 \Rightarrow 1$
- $0.6 \times 2 = 1.2 \Rightarrow 1$

Resultado aproximado: $0.2_{10} \approx 0.0011_2$

---

## Conversión directa binario → octal/hexadecimal

- Octal: agrupar bits de a 3 desde la derecha
- Hexadecimal: agrupar bits de a 4 desde la derecha

Ejemplo:

$011001002=6416,011001002=144801100100_2 = 64_{16},\quad 01100100_2 = 144_8$

---
## Complemento

El **complemento** de un número en un sistema de numeración representa cuánto le falta a ese número para llegar a un múltiplo de la base, normalmente utilizado para facilitar la **resta** mediante una **suma**.

Se utiliza un formato $n$, que indica la cantidad de cifras consideradas. Por ejemplo, si el número es 45 y el formato es $n=3$, el valor base es $10^3 = 1000$.

#### Complemento a la base 
Denotado como $C_b(N)$:

$Cb(N)= b^n - N$

Donde:
- $b$ es la base (por ejemplo, 10 en decimal)
- $n$ es el formato (número de cifras)
- $N$ es el número original

**Ejemplo:** En base 10

- ${C_{10}(7)}$ con $n = 1$:           $10^1 - 7 = 3$

- ${C_{10}(548)}$ con $n = 3$:       $10^3 - 548 = 1000 - 548 = 452$

- ${C_{10}(05)}$ con $n = 2$:          $10^2 - 5 = 100 - 5 = 95$


#### Complemento a la base - 1 (Complemento restringido)

Denotado como $C_{b-1}(N)$:

$C_{b-1}(N)= C_b(N) - 1$

**Ejemplo:** En Sistema Decimal (10-1) conocido en este caso como Complemento a 9

- ${C_{9}(7)}$ con $n = 1$: $10 - 1 - 7 = 9 - 7 = 2$
    
- ${C_{9}(548)}$ con $n = 3$: $1000 - 1 - 548 = 999 - 548 = 451$
    
- ${C_{9}(05)}$ con $n = 2$: $100 - 1 - 5 = 99 - 5 = 94$

---

## Complemento en binario

- **C1 (Complemento a 1):** Invertir todos los bits
- **C2 (Complemento a 2):** Invertir los bits y sumar 1

Ejemplo: Dado $110_2$
- $C1 = 001$
- $C2 = 010$

---
## Operaciones en Binario

**Suma:**
- $0 + 0 = 0$
- $0 + 1 = 1$
- $1 + 0 = 1$
- $1 + 1 = 0$ (acarreo 1)

**Resta:** Se realiza como suma del complemento (ej. para $A - B$ usar $A + C2(B)$)

---

## Unidades de medida digital

| Unidad   | Equivalencia | Potencia |
| -------- | ------------ | -------- |
| Byte     | 8 bits       | -        |
| Kilobyte | 1024 bytes   | $2^{10}$ |
| Megabyte | 1024 KB      | $2^{20}$ |
| Gigabyte | 1024 MB      | $2^{30}$ |
| Terabyte | 1024 GB      | $2^{40}$ |
| ...      | ...          | ...      |

---
## Tipos de datos (bits)

- byte: 8 bits
- short: 16 bits
- int: 32 bits
- long: 64 bits
- float: 32 bits
- double: 64 bits
- boolean: 32 bits
- char: 8 bits

---

## Resumen general de conversiones

- De binario/octal/hex a decimal: **polinomio de potencias**
    
- De decimal a otra base:
    
    - Parte entera: **divisiones sucesivas**
        
    - Parte fraccionaria: **multiplicaciones sucesivas**
        
- De binario a octal o hex: **agrupaciones** (3 o 4 bits)
- De octal a hex o viceversa: **pasar por decimal o binario**


