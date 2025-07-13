$$(\mathbb{V}, +, \mathbb{K}, \cdot)$$
- $\mathbb{V}:$ Conjunto de Vectores  
- $+:$ Operación Interna  
- $\mathbb{K}:$ Cuerpo  
- $\cdot:$ Operación Externa  

Para que un conjunto $\mathbb{V}$ con las operaciones $+$ y $\cdot$ sea un espacio vectorial sobre un cuerpo $\mathbb{K}$, deben cumplirse las siguientes **8 propiedades**:

#### Operaciones Internas 

1. **Ley de composición Interna**:  
   $\forall u, v \in \mathbb{V} \Rightarrow u + v \in \mathbb{V}$
2. **Asociatividad de la suma**:  
   $\forall u, v, w \in \mathbb{V} \Rightarrow (u + v) + w = u + (v + w)$

3. **Existencia del elemento neutro**:  
   $\exists 0 \in \mathbb{V} \; / \; \forall v \in \mathbb{V}, \; v + 0 = v$

4. **Existencia del elemento opuesto**:  
   $\forall v \in \mathbb{V} \; \exists (-v) \in \mathbb{V} \; / \; v + (-v) = 0$

5.  **Conmutatividad de la suma**:  
   $\forall u, v \in \mathbb{V} \Rightarrow u + v = v + u$

(Grupo si se cumplen las 3 primeras, grupo abeliano si se cumplen las 4)

#### Operación Externa

5. **Ley de composición Externa:**
   $\forall \alpha \in \mathbb{R},\forall \beta \in \mathbb{K} \Rightarrow \alpha \cdot \beta \in \mathbb{K}$

6. **Distributiva del respecto de la operación interna:**  
   $\forall \alpha \in \mathbb{K}, \forall u, v \in \mathbb{V} \Rightarrow \alpha \cdot (u + v) = \alpha \cdot u + \alpha \cdot v$  
7. **Distributiva con la suma de elemento de K**
	$\forall \alpha, \beta \in \mathbb{K}, \forall v \in \mathbb{V} \Rightarrow (\alpha + \beta) \cdot v = \alpha \cdot v + \beta \cdot v$

8. **Asociabilidad del producto de escalares**:  
   $\forall \alpha, \beta \in \mathbb{K}, \forall v \in \mathbb{V} \Rightarrow (\alpha \cdot \beta) \cdot v = \alpha \cdot (\beta \cdot v)$

9. **Elemento neutro del producto**:  
   $\forall v \in \mathbb{V} \Rightarrow 1 \cdot v = v$, donde $1$ es el neutro multiplicativo en $\mathbb{K}$


## Propiedades de los espacios vectoriales

**Todo vector multiplicado por 0 da el vector nulo:**  
$\forall u \in \mathbb{V}: 0 \cdot u = \vec{0}$

**Ejemplo 1:** Si $u = (3, 5)$, entonces $0 \cdot u = (0, 0)$  
**Ejemplo 2:** Si $u = (-2, 7, 1)$, entonces $0 \cdot u = (0, 0, 0)$

---

**El escalar negativo de un vector es el inverso aditivo del vector:**  
$\forall u \in \mathbb{V}: -u = (-1) \cdot u$

**Ejemplo 1:** Si $u = (4, -3)$, entonces $-u = (-4, 3)$  
**Ejemplo 2:** Si $u = (1, 0, -5)$, entonces $-u = (-1, 0, 5)$

---

**Multiplicación escalar distributiva respecto a la suma de vectores:**  
$\forall a \in \mathbb{F},\ \forall u,v \in \mathbb{V}: a(u + v) = au + av$

**Ejemplo 1:** Si $a = 2$, $u = (1, 2)$ y $v = (3, -1)$, entonces  

$2((1, 2) + (3, -1)) = 2(4, 1) = (8, 2)$  
y $2(1, 2) + 2(3, -1) = (2, 4) + (6, -2) = (8, 2)$

**Ejemplo 2:** Si $a = -1$, $u = (2, 3, 4)$ y $v = (0, -1, 1)$, entonces  
$-1((2, 3, 4) + (0, -1, 1)) = -1(2, 2, 5) = (-2, -2, -5)$  
y $-1(2, 3, 4) + -1(0, -1, 1) = (-2, -3, -4) + (0, 1, -1) = (-2, -2, -5)$

---

**Multiplicación escalar distributiva respecto a la suma de escalares:**  
$\forall a,b \in \mathbb{F},\ \forall u \in \mathbb{V}: (a + b)u = au + bu$

**Ejemplo 1:** Si $a = 2$, $b = 3$, $u = (1, 0)$, entonces  
$(2 + 3)(1, 0) = 5(1, 0) = (5, 0)$  
y $2(1, 0) + 3(1, 0) = (2, 0) + (3, 0) = (5, 0)$

**Ejemplo 2:** Si $a = -1$, $b = 4$, $u = (2, -2)$, entonces  
$(-1 + 4)(2, -2) = 3(2, -2) = (6, -6)$  
y $-1(2, -2) + 4(2, -2) = (-2, 2) + (8, -8) = (6, -6)$

---

**Asociatividad del producto escalar:**  
$\forall a,b \in \mathbb{F},\ \forall u \in \mathbb{V}: a(bu) = (ab)u$

**Ejemplo 1:** Si $a = 2$, $b = 3$, $u = (1, 4)$, entonces  
$2(3(1, 4)) = 2(3, 12) = (6, 24)$  
y $(2 \cdot 3)(1, 4) = 6(1, 4) = (6, 24)$

**Ejemplo 2:** Si $a = -1$, $b = 5$, $u = (0, 1, -1)$, entonces  
$-1(5(0, 1, -1)) = -1(0, 5, -5) = (0, -5, 5)$  
y $(-1 \cdot 5)(0, 1, -1) = -5(0, 1, -1) = (0, -5, 5)$

---

**Elemento neutro del producto escalar:**  
$\forall u \in \mathbb{V}: 1 \cdot u = u$

**Ejemplo 1:** Si $u = (3, -1)$, entonces $1 \cdot u = (3, -1)$  
**Ejemplo 2:** Si $u = (0, 0, 7)$, entonces $1 \cdot u = (0, 0, 7)$