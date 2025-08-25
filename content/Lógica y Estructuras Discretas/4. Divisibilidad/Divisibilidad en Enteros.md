## Conjunto de los enteros
El conjunto de los números enteros se representa con $\mathbb{Z}$:

$$
\mathbb{Z} = \{ \dots, -3, -2, -1, 0, 1, 2, 3, \dots \}
$$

> [!important]  El conjunto de los enteros es **infinito pero discreto**: entre dos enteros hay siempre una cantidad finita de enteros.

#### Operaciones en $\mathbb{Z}$

- La **suma, resta y multiplicación** son operaciones cerradas en $\mathbb{Z}$.  
- La **división** no siempre lo es:  
  Ejemplo: $8 \div 3$ no es un número entero.

---

## Divisibilidad

Se dice que $a$ divide a $b$ (se escribe $a \mid b$) si:

$$
\quad b = k \cdot a \ \ \ \  \ \exists k \in \mathbb{Z} 
$$

- “$b$ es divisible por $a$”  
- “$a$ es divisor de $b$”  
- “$b$ es múltiplo de $a$”

**Ejemplos:**
- $8 \mid 72$ porque $72 = 9 \cdot 8$  
- $15 \nmid 50$ porque no existe $k \in \mathbb{Z}$ tal que $50 = 15k$  

> [!important] Propiedades básicas
> 1. $a \mid a$ para todo $a \neq 0$  
> 2. $a \mid b \ \land \ b \mid c \ \Rightarrow \ a \mid c$  
> 3. $a \mid b \ \land \ a \mid c \ \Rightarrow \ a \mid (b+c)$  
> 4. $a \mid b \ \Rightarrow \ a \mid (b \cdot c)$ para todo $c \in \mathbb{Z}$  

---

## Números primos
Un número primo $p$ es un entero mayor que $1$ que solo es divisible por:

$$
\pm 1, \ \pm p
$$

Ejemplos: $2, 3, 5, 7, 11, 13, \dots$  

> [!tip]  
> Los primos son infinitos. No existe una fórmula general para obtenerlos.  
> Son fundamentales en matemáticas y en aplicaciones como la **criptografía (RSA)**.

**Propiedad clave:**  
Si $p$ es primo y $p \mid a \cdot b$, entonces:

$$
p \mid a \ \lor \ p \mid b
$$

---

## Teorema Fundamental de la Aritmética

Todo número entero $n > 1$ es:  
- Primo, o  
- Producto único de factores primos (salvo el orden).

**Ejemplo:**
- $84 = 2^2 \cdot 3 \cdot 7$  
- $105 = 3 \cdot 5 \cdot 7$  
- $36 = 2^2 \cdot 3^2$  

---

## Máximo común divisor (MCD) y mínimo común múltiplo (MCM)

- **MCD $(a,b)$**: el mayor divisor común de $a$ y $b$.  

$$
\text{mcd}(a,b)=d \ \ \to \ \ d=a \cdot q+b\cdot r
$$
$q \ \text{y} \ r \in \mathrm{Z}$ 

- **MCM $[a,b]$**: el menor múltiplo común de $a$ y $b$.  

**Propiedad fundamental:**

$$
\text{mcd}(a,b) \cdot \text{mcm}(a,b) = |a \cdot b|
$$

Si $\text{mcd}(a,b) = 1$, se dice que $a$ y $b$ son **coprimos**.


> [!important] Propiedad
>$$
> \text{mcd}(a,b)=d \ \ \to \ \ d|\ a \ \land \ d |\ b
>$$

---

## Algoritmo de Euclides

Método para hallar el mcd de dos números:

Si $a = bq + r$, entonces:

$$
\text{mcd}(a,b) = \text{mcd}(b,r)
$$

Se repite el proceso hasta que el resto sea $0$.  
El último resto no nulo es el $\text{mcd}(a,b)$.

---

## Teorema de Bézout
Dados $a,b \in \mathbb{Z}$:

$$
\text{mcd}(a,b) = 1 \iff \exists s,t \in \mathbb{Z} \ \ \ 1 = s \cdot a + t \cdot b
$$

> [!important]  El teorema de Bézout sirve para demostrar que dos números son **coprimos**.
> 

Ejemplo:  
Como $1 = 3 \cdot 8541 + (-2) \cdot 12811$, entonces:  
$\text{mcd}(8541,12811) = 1$.

---

## Propiedad final
Si $p$ es primo y $p \mid a \cdot b$, entonces necesariamente:

$$
p \mid a \ \lor \ p \mid b
$$
