## Multiplicación de matrices

Sean $A \in \mathbb{R}^{m \times n}$ y $B \in \mathbb{R}^{n \times p}$, el producto $AB$ es una matriz $C \in \mathbb{R}^{m \times p}$, donde:

${c_{ij} = \sum_{k=1}^{n} a_{ik} \cdot b_{kj}}$

### Condición:
El número de columnas de $A$ debe ser igual al número de filas de $B$.

---

### Propiedades de la multiplicación de matrices

1. **No conmutativa:** En general, ${AB \neq BA}$
2. **Asociativa:** ${A(BC) = (AB)C}$
3. **Distributiva:**  
   - Respecto a la suma: ${A(B + C) = AB + AC}$
   - ${(A + B)C = AC + BC}$
4. **Elemento neutro:**  
   ${AI_n = I_m A = A}$ si las dimensiones son compatibles
5. **Producto por la matriz nula:**  
   ${A \cdot 0 = 0 \cdot A = 0}$

---

## Matriz inversa

Una matriz cuadrada $A \in \mathbb{R}^{n \times n}$ es **invertible** si existe otra matriz $A^{-1}$ tal que:

${A \cdot A^{-1} = A^{-1} \cdot A = I_n}$

**Condición:** $A$ es invertible $\iff \det(A) \neq 0$

> [!important] Matriz Singular
> Es aquella matriz que no admite inversa por lo que su $\det(A) = 0$

#### Propiedades

- $(A^{-1})^{-1}=A$
- $(k \cdot A)^{-1}=\frac{1}{k}\cdot A^{-1}$
- $(A^{t})^{-1}=(A^{-1})^{t}$
- $(A\cdot B)^{-1}=A^{-1}\cdot B^{-1}$
---

## Determinante de una matriz

### Caso 2×2:

Si  
$A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$  
entonces  
$\det(A) = ad - bc$

---

### Regla de Laplace (caso general)

Para $A \in \mathbb{R}^{n \times n}$, el determinante puede calcularse desarrollando por una fila o columna:

${\det(A) = \sum_{j=1}^{n} (-1)^{i+j} \cdot a_{ij} \cdot \det(M_{ij})}$

Donde:

- $a_{ij}$ es el elemento de la fila $i$, columna $j$
- $M_{ij}$ es el menor: submatriz que resulta al eliminar la fila $i$ y columna $j$

---

## Matriz adjunta

La **matriz adjunta** de $A$ es la transpuesta de su **matriz de cofactores**.

1. Cofactor:  
   ${C_{ij} = (-1)^{i+j} \cdot \det(M_{ij})}$

2. Matriz de cofactores:  
   ${C = (C_{ij})}$

3. **Adjunta:**  
   ${\text{adj}(A) = C^t}$

---

### Inversa con adjunta y determinante:
Si $A$ es invertible:

${A^{-1} = \dfrac{1}{\det(A)} \cdot \text{adj}(A)}$

$\begin{pmatrix} 1& 0&0&0\\-1&0&K&-1\\2&1&0&0\\1&K&1&K\end{pmatrix}$