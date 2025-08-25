
**BCD (Binary Coded Decimal)** o **Decimal Codificado en Binario** es una forma de representar dígitos decimales (0 a 9) mediante grupos de bits binarios. Cada dígito decimal se representa con un nibble (4 bits).

|     | BCD Natural |
| --- | ----------- |
| 0   | 0 0 0 0     |
| 1   | 0 0 0 1     |
| 2   | 0 0 1 0     |
| 3   | 0 0 1 1     |
| 4   | 0 1 0 0     |
| 5   | 0 1 0 1     |
| 6   | 0 1 1 0     |
| 7   | 0 1 1 1     |
| 8   | 1 0 0 0     |
| 9   | 1 0 0 1     |


> En el **BCD natural**, solo se usan las combinaciones binarias de 0000 a 1001 (0 a 9). Las combinaciones de 1010 a 1111 son consideradas inválidas.

**Ejemplo:** Representar 714

BCD Natural:  0111   0001   0100

---

## Tipos de Representación BCD

**BCD Empaquetado (Packed)**
- 2 Decimales x Byte
- El signo va al final
	- **+:** 1011
	- **-:** 1101

**BCD Desempaquetado (Unpacked)**
- 1 Decimal x Byte
- El signo va al inicio con zona dos
	- **+:** 0010  1011
	- **-:** 0010  1101
- Se le agrega la zona: Valor constante para definir el desempaquetado.

---
![[Pasted image 20250622195026.png|]]