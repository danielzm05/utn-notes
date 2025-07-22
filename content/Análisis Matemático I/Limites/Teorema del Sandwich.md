El **teorema del sándwich** se utiliza para evaluar límites de funciones que están "atrapadas" entre otras dos funciones, cuyos límites son iguales en un punto.

Sea el $\lim\limits_{x\to a}f(x)$ desconocido. Sean $h(x)$ y $g(x)$ tal que $\forall x, h(x)\leq f(x)\leq g(x)$

y además $\lim\limits_{x\to a}h(x)=L$ y $\lim\limits_{x\to a}g(x)=L'$ entonces $L\leq \lim\limits_{x\to a}f(x)\leq L'$

- Si $L=L'$, entonces $\lim\limits_{x\to a}f(x)=L$

> [!tip]  
> Este teorema es útil cuando no podemos evaluar el límite directamente, pero podemos encajonar la función entre otras dos que sí tienen un límite común.

---

**Ejemplo:** Determinar el límite:

$$
\lim_{x \to 0} x^2 \cdot \sin\left(\tfrac{1}{x}\right)
$$

**Solución**

Sabemos que:

$$
-1 \leq \sin\left(\tfrac{1}{x}\right) \leq 1
$$

Multiplicando por $x^2$ (que es positivo cerca de 0):

$$
-x^2 \leq x^2 \cdot \sin\left(\tfrac{1}{x}\right) \leq x^2
$$

Ahora tomamos límites:

$$
\lim_{x \to 0} (-x^2) = 0 \quad \text{y} \quad \lim_{x \to 0} x^2 = 0
$$

Por el teorema del sándwich:

$$
\lim_{x \to 0} x^2 \cdot \sin\left(\tfrac{1}{x}\right) = 0
$$




