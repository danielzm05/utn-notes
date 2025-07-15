## Definición general de matriz

Una **matriz** es un **arreglo rectangular de números reales** dispuestos en **filas** y **columnas**.  
Se representa como:  
${A = (a_{ij})_{1 \leq i \leq p,\ 1 \leq j \leq n}}$  
donde $a_{ij}$ indica el número en la **fila $i$ y columna $j$**.

El conjunto de matrices reales de $p$ filas y $n$ columnas se denota:  
${\mathbb{R}^{p \times n}}$

---

## Matriz columna

Es una matriz de tamaño ${p \times 1}$, es decir, **una sola columna**.

Ejemplo:  
$\begin{pmatrix} 2 \\ -1 \end{pmatrix} \in \mathbb{R}^{2 \times 1}$

---

## Matriz fila

Es una matriz de tamaño ${1 \times n}$, es decir, **una sola fila**.

Ejemplo:  
$\begin{pmatrix} 0 & -4 \end{pmatrix} \in \mathbb{R}^{1 \times 2}$

---

## Matriz cuadrada

Tiene el **mismo número de filas y columnas**: ${n \times n}$.

Ejemplo:  
$\begin{pmatrix} -1 & 3 \\ \frac{1}{2} & 0 \end{pmatrix} \in \mathbb{R}^{2 \times 2}$

---

## Diagonal principal

En una matriz cuadrada, es el conjunto de elementos con subíndice fila igual a columna:  
${\text{diag}(A) = \{a_{11}, a_{22}, \dots, a_{nn}\}}$

---

## Traza de una matriz cuadrada

Es la **suma de los elementos de la diagonal principal**:  
${\text{tr}(A) = a_{11} + a_{22} + \dots + a_{nn} = \sum_{i=1}^{n} a_{ii}}$

---

## Matriz triangular superior

Es una matriz cuadrada donde **todos los elementos debajo de la diagonal principal son cero**:  
${a_{ij} = 0 \quad \text{para todo } i > j}$

Ejemplo:  

$\begin{pmatrix} 3 & 2 & 4 \\ 0 & 5 & 8 \\ 0 & 0  & 3 \end{pmatrix}$

---

## Matriz triangular inferior

Es una matriz cuadrada donde **todos los elementos por encima de la diagonal principal son cero**:  
${a_{ij} = 0 \quad \text{para todo } i < j}$

Ejemplo:  
$\begin{pmatrix} 3 & 0 & 0 \\ 3 & 5 & 0 \\ 4 & 6  & 3 \end{pmatrix}$

---

## Matriz diagonal

Es una matriz cuadrada donde **todos los elementos fuera de la diagonal principal son cero**:  
${a_{ij} = 0 \quad \text{para todo } i \neq j}$

Ejemplo:  
$\begin{pmatrix} 4 & 0 \\ 0 & -2 \end{pmatrix}$

---

## Matriz escalar

Es una **matriz diagonal** donde **todos los elementos de la diagonal principal son iguales**:  
${a_{ii} = k \quad \text{para todo } i,\ \text{con } k \in \mathbb{R}}$

Ejemplo:  
$\begin{pmatrix} 3 & 0 \\ 0 & 3 \end{pmatrix}$

---

## Matriz identidad

Es una **matriz escalar** donde ${k = 1}$, es decir, los elementos de la diagonal principal son 1.  
Notación: ${I_n}$

Ejemplo:  
$\begin{pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix} = I_3$

---

## Matriz nula

Es una matriz donde **todos los elementos son cero**:  
${a_{ij} = 0 \quad \forall i,j}$

Ejemplo:  
$\begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}$

---

## Igualdad de matrices

Dos matrices ${A, B \in \mathbb{R}^{p \times n}}$ son **iguales** si:

1. Tienen **el mismo orden** (mismo número de filas y columnas)
2. Cada uno de sus elementos correspondientes es igual:  
${a_{ij} = b_{ij} \quad \forall i,j}$


---

**Matriz Involutiva:** $A\cdot A=I$
**Idempotencia:** $A^{2}=A$
**Permutables:** $AB=BA$
