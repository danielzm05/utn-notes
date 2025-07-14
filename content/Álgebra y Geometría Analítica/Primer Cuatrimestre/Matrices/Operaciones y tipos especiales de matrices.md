## Operaciones con matrices

### Suma de matrices

Dadas dos matrices $A, B \in \mathbb{R}^{p \times n}$, su suma $C = A + B$ se define como:

${c_{ij} = a_{ij} + b_{ij}}$ para todo $i, j$

**Propiedades:**

1. **Clausura:** ${A + B \in \mathbb{R}^{p \times n}}$
2. **Asociatividad:** ${(A + B) + C = A + (B + C)}$
3. **Elemento neutro:** existe una matriz nula $N$ tal que ${A + N = A}$
4. **Elemento opuesto:** para toda $A$ existe $-A$ tal que ${A + (-A) = 0}$
5. **Conmutatividad:** ${A + B = B + A}$

### Resta de matrices

Definida como:  
${A - B = A + (-B)}$

---

### Multiplicación de una matriz por un escalar

Dado $k \in \mathbb{R}$ y $A \in \mathbb{R}^{p \times n}$:

${(k \cdot A)_{ij} = k \cdot a_{ij}}$

Propiedades:

1. **Clausura:** ${k \cdot A \in \mathbb{R}^{p \times n}}$
2. **Asociatividad mixta:** ${k_1 (k_2 A) = (k_1 k_2) A}$
3. **Distributividad respecto a la suma de matrices:**  
   ${k (A + B) = k A + k B}$
4. **Distributividad respecto a la suma de escalares:**  
   ${(k_1 + k_2) A = k_1 A + k_2 A}$
5. **Elemento neutro:** ${1 \cdot A = A}$

Consecuencias:

- ${0 \cdot A = 0}$
- ${k \cdot 0 = 0}$
- ${-A = (-1) \cdot A}$

---

## Matriz transpuesta
La transpuesta de una matriz $A \in \mathbb{R}^{p \times n}$ es la matriz $A^t \in \mathbb{R}^{n \times p}$ tal que:

${(A^t)_{ij} = a_{ji}}$

Ejemplo:

Si  
$A = \begin{pmatrix} 1 & 0 & 3 \\ -1 & 1 & 2 \end{pmatrix}$

Entonces  
$A^t = \begin{pmatrix} 1 & -1 \\ 0 & 1 \\ 3 & 2 \end{pmatrix}$

### Propiedades de la transposición

1. ${(A^t)^t = A}$
2. ${(A + B)^t = A^t + B^t}$
3. ${(k \cdot A)^t = k \cdot A^t}$

---

## Matrices simétricas

Una matriz cuadrada $A \in \mathbb{R}^{n \times n}$ es **simétrica** si:

${a_{ij} = a_{ji}}$ para todo $i, j$  
Es decir, ${A = A^t}$

Ejemplo:

$A = \begin{pmatrix} 2 & 3 \\ 3 & 5 \end{pmatrix}=A^t$

Propiedades:

- La suma de dos matrices simétricas es también simétrica.

---

## Matrices antisimétricas
Una matriz cuadrada $A \in \mathbb{R}^{n \times n}$ es **antisimétrica** si:

${a_{ij} = -a_{ji}}$ para todo $i, j$  
Esto implica que todos los elementos de la diagonal son cero:  
${a_{ii} = -a_{ii} \Rightarrow a_{ii} = 0}$

Ejemplo:

$A = \begin{pmatrix} 0 & -3 \\ 3 & 0 \end{pmatrix}$

Propiedades:
- ${A = -A^t}$
- La suma de dos matrices antisimétricas es también antisimétrica.

