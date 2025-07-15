
- **Con radicales**: multiplicar por el conjugado para transformar la diferencia en un cociente.
- **Sin radicales**: combinar los términos en una sola fracción y luego aplicar álgebra (factorización, simplificación, o [[Regla de L'Hôpital|L’Hôpital]] si aplica).

---

#### Ejemplo 1: Con radicales → Multiplicamos por el conjugado

Calcular:

$$
\lim_{x \to \infty} \left( \sqrt{x^2 + x} - x \right)
$$

**Paso 1: Evaluación directa**

$$
\sqrt{x^2 + x} \to \infty \quad \text{y} \quad x \to \infty \quad \Rightarrow \quad \infty - \infty
$$

Indeterminación.

**Paso 2: Multiplicamos por el conjugado**

Multiplicamos arriba y abajo por el conjugado:

$$
\left( \sqrt{x^2 + x} - x \right) \cdot \frac{\sqrt{x^2 + x} + x}{\sqrt{x^2 + x} + x}
$$

Aplicamos la identidad de diferencia de cuadrados:

$$
\frac{(x^2 + x) - x^2}{\sqrt{x^2 + x} + x} = \frac{x}{\sqrt{x^2 + x} + x}
$$

**Paso 3: Simplificamos**

Factorizamos $x$ dentro de la raíz:

$$
\sqrt{x^2 + x} = x\sqrt{1 + \frac{1}{x}}
$$

Sustituimos:

$$
\frac{x}{x \left( \sqrt{1 + \frac{1}{x}} + 1 \right)} = \frac{1}{\sqrt{1 + \frac{1}{x}} + 1}
$$

**Paso 4: Tomamos el límite**

Cuando $x \to \infty$, $\frac{1}{x} \to 0$, así que:

$$
\lim_{x \to \infty} \frac{1}{\sqrt{1 + \frac{1}{x}} + 1} = \frac{1}{1 + 1} = \frac{1}{2}
$$

---

#### Ejemplo 2: Sin radicales → Reescribimos como fracción

Calcular:

$$
\lim_{x \to \infty} \left( \ln(x + 1) - \ln(x) \right)
$$

**Paso 1: Evaluación directa**

$$
\ln(x + 1) \to \infty \quad \text{y} \quad \ln(x) \to \infty \quad \Rightarrow \quad \infty - \infty
$$

Indeterminación.

**Paso 2: Aplicamos propiedades de logaritmos**

Usamos:

$$
\ln(a) - \ln(b) = \ln\left( \frac{a}{b} \right)
$$

Entonces:

$$
\ln(x + 1) - \ln(x) = \ln\left( \frac{x + 1}{x} \right) = \ln\left( 1 + \frac{1}{x} \right)
$$

**Paso 3: Evaluamos el nuevo límite**

Cuando $x \to \infty$, $\frac{1}{x} \to 0$:

$$
\lim_{x \to \infty} \ln\left( 1 + \frac{1}{x} \right) = \ln(1) = 0
$$


