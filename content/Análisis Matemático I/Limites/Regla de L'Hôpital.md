
> [!warning] La regla de L'Hôpital
> Aplica para indeterminaciones [[Indeterminación Infinito sobre Infinito|infinito sobre infinito]] y [[Limite con Indeterminación 0 sobre 0| 0 sobre 0]]
> **También es necesario saber derivar**

La **Regla de L'Hôpital** permite evaluar ciertos límites que resultan en **indeterminaciones** de la forma:

- $\frac{0}{0}$
- $\frac{\infty}{\infty}$

Si al intentar evaluar el límite de una función racional $\frac{f(x)}{g(x)}$ se obtiene una indeterminación, y si $f$ y $g$ son derivables en un intervalo alrededor del punto, entonces:

$$
\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{f'(x)}{g'(x)}
$$

*(Siempre que este nuevo límite exista o sea infinito).*

---

#### Condiciones necesarias

- El límite original debe dar una **indeterminación**.
- Las funciones $f(x)$ y $g(x)$ deben ser **derivables** en el entorno del punto de interés.
- El **límite del cociente de derivadas debe existir** (o tender a infinito).

---

#### Ejemplo 1: Indeterminación $\frac{0}{0}$

Calcular:

$$
\lim_{x \to 0} \frac{\sin(x)}{x}
$$

**Paso 1:** Evaluación directa

$$
\frac{\sin(0)}{0} = \frac{0}{0} \quad \text{(indeterminación)}
$$

**Paso 2:** Aplicamos L’Hôpital

$$
\lim_{x \to 0} \frac{\sin(x)}{x} = \lim_{x \to 0} \frac{\cos(x)}{1} = \cos(0) = 1
$$


---

#### Ejemplo 2: Indeterminación $\frac{\infty}{\infty}$

Calcular:

$$
\lim_{x \to \infty} \frac{x}{e^x}
$$

**Paso 1:** Evaluación directa

$$
\frac{x}{e^x} \to \frac{\infty}{\infty} \quad \text{(indeterminación)}
$$

**Paso 2:** Aplicamos L’Hôpital

$$
\lim_{x \to \infty} \frac{x}{e^x} = \lim_{x \to \infty} \frac{1}{e^x}
$$

$$
\frac{1}{e^x} \to 0 \quad \text{(cuando } x \to \infty \text{)}
$$




> [!important] Observaciones
> - A veces es necesario **aplicar L’Hôpital más de una vez** si la indeterminación persiste.
>- No se debe usar L’Hôpital si no hay indeterminación.
>- Existen otras indeterminaciones que **requieren manipulación previa** antes de aplicar L’Hôpital: $0 \cdot \infty$, $\infty - \infty$, etc.


