
- Siempre que obtengas una forma $\frac{0}{0}$, busca **manipular la expresión** para eliminar la causa de la indeterminación.
- Si hay raíces, **multiplica por el conjugado**.
- Si no hay raíces, **factoriza** el numerador o denominador.
- Una vez simplificada la expresión, **vuelve a evaluar el límite**.

---

#### Ejemplo 1: Radicales → Multiplicamos por el conjugado

Calcular:

$$
\lim_{x \to 4} \frac{\sqrt{x} - 2}{x - 4}
$$

**Paso 1:** Evaluación directa

$$
\frac{\sqrt{4} - 2}{4 - 4} = \frac{0}{0} \quad \text{(indeterminación)}
$$

**Paso 2:** Multiplicamos por el conjugado del numerador

> Multiplicamos arriba y abajo por $\sqrt{x} + 2$:

$$
\frac{\sqrt{x} - 2}{x - 4} \cdot \frac{\sqrt{x} + 2}{\sqrt{x} + 2}
= \frac{(\sqrt{x} - 2)(\sqrt{x} + 2)}{(x - 4)(\sqrt{x} + 2)}
$$

Simplificamos el numerador usando diferencia de cuadrados:

$$
\frac{x - 4}{(x - 4)(\sqrt{x} + 2)} = \frac{1}{\sqrt{x} + 2}
$$

**Paso 3:** Evaluamos el límite

$$
\lim_{x \to 4} \frac{1}{\sqrt{x} + 2} = \frac{1}{2 + 2} = \frac{1}{4}
$$


---

#### Ejemplo 2: Sin radicales → Factorizamos

Calcular:

$$
\lim_{x \to 2} \frac{x^2 - 4}{x - 2}
$$

**Paso 1:** Evaluación directa

$$
\frac{2^2 - 4}{2 - 2} = \frac{0}{0} \quad \text{(indeterminación)}
$$

**Paso 2:** Factorizamos el numerador

$$
x^2 - 4 = (x - 2)(x + 2)
$$

Entonces:

$$
\frac{(x - 2)(x + 2)}{x - 2}
$$

Cancelamos el factor común $(x - 2)$:

$$
= x + 2
$$

**Paso 3:** Evaluamos el límite

$$
\lim_{x \to 2} x + 2 = 4
$$


---


> [!important] Regla de L'Hôpital
> Recuerda que para resolver este tipo de indeterminaciones también puedes usar la [[Regla de L'Hôpital]]



