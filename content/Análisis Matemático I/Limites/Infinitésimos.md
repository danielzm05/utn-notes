Se dice que $f(x)$ es un infinitésimo en un punto (x=a) si y solo si el limite $\lim\limits_{x\to a}f(x)=0$

**Ejemplos**

- $\lim\limits_{x\to 1} x^2-x=0$        ✅ $f(x)$ es infinitésimo cuando $x \to 1$
- $\lim\limits_{x\to 0} x^2-x=0$        ✅ $f(x)$ es infinitésimo cuando $x \to 0$
- $\lim\limits_{x\to 2} x^2-x=2$        ❌ $f(x)$  no eses infinitésimo cuando $x \to 2$

## Propiedades

- **La suma de dos infinitésimos en $x\to a$ es otro infinitésimo en el mismo punto:**

- **El producto de un escalar por un infinitésimo en $x\to a$da como resultado otro infinitésimo en el mismo punto**

- **El producto de dos infinitésimos en $x\to a$ da como resultado otro infinitésimo en el mismo punto**

- **El cociente de dos infinitésimos puede dar tres resultados:**
	- 0 Si el infinitésimo numerador es de mayor orden infinitesimal que el denominador
	
	- $\infty$ si el infinitésimo del denominador es de mayor orden infinitesimal que el numerador
	
	- Numero Real $K$, si ambos infinitésimos tienen igual orden infinitesimal
	>***Si el numero real $K$ es 1, los infinitésimos son eqivalentes***
	

## Sustitución de infinitésimos equivalentes 

Los infinitésimos son de gran ayuda a la hora de realizar calculo de limites, ya que podemos reemplazar una función por su equivalente infinitesimal, siempre y cuando la función se comporte igual en dicho punto.

**Ejemplo:**

$$
\
\lim_{x \to 0} \frac{\sin x}{x}
\
$$

Nos da una indeterminación $\frac{0}{0}$, por lo que reemplazando $\sin x$ por su equivalente infinitesimal cuando $x \to 0$ que es $x$:

$$
\
\lim_{x \to 0} \frac{\sin x}{x} \approx \lim_{x \to 0} \frac{x}{x} = 1
$$

#### Ejemplo de equivalencias

| Función Original   | Equivalencia infinitesimal cuando $x \to 0$ |
| ------------------ | ------------------------------------------- |
| $\sin x$           | $x$                                         |
| $\tan x$           | $x$                                         |
| $1 - \cos x$       | $\dfrac{x^2}{2}$                            |
| $\ln(1 + x)$       | $x$                                         |
| $e^x - 1$          | $x$                                         |
| $(1 + x)^n - 1$    | $nx$ (si $n \in \mathbb{R}$)                |
| $\arcsin x$        | $x$                                         |
| $\arctan x$        | $x$                                         |
| $\sqrt{1 + x} - 1$ | $\dfrac{x}{2}$                              |
