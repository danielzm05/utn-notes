Un **haz de planos** es un conjunto infinito de planos que pasan por una recta común (intersección de dos planos). Se puede escribir como una **combinación lineal** de dos planos dados:

## Fórmula general del haz de planos:

$\alpha \cdot \pi_1 + \beta \cdot \pi_2 = 0 \quad \text{con } \alpha, \beta \in \mathbb{R}, \text{ no ambos cero}$

Si:

- $\pi_1: a_1x + b_1y + c_1z + d_1 = 0$
- $\pi_2: a_2x + b_2y + c_2z + d_2 = 0$

Entonces el haz de planos es:

$\alpha(a_1x + b_1y + c_1z + d_1) + \beta(a_2x + b_2y + c_2z + d_2) = 0$

## ¿Qué representa?

Cada valor distinto de $\dfrac{\alpha}{\beta}$ (o viceversa) define un plano distinto dentro del haz, **todos ellos comparten la misma recta de intersección entre $\pi_1$ y $\pi_2$**.

---

## ¿Cómo se obtiene el vector normal de un plano del haz?

Cada plano en el haz tiene como **vector normal** una **combinación lineal** de los normales de $\pi_1$ y $\pi_2$.

### Fórmulas:

- Normal de $\pi_1$: $\vec{n}_1 = (a_1, b_1, c_1)$
- Normal de $\pi_2$: $\vec{n}_2 = (a_2, b_2, c_2)$
- Entonces, la normal de un plano cualquiera del haz es:

$\vec{n} = \alpha \cdot \vec{n}_1 + \beta \cdot \vec{n}_2$

---

## Observación

Para que el haz **represente realmente una familia de planos**, $\pi_1$ y $\pi_2$ deben ser **distintos y no paralelos**, es decir, sus normales **no deben ser proporcionales**.

