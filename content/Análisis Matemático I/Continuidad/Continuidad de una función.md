Una función será continua en un punto $a$ sí:
- $\exists f(a)$
- $\exists \lim\limits_{x\to a}f(x)$
- $\lim\limits_{x\to a}f(x)=f(a)$

---
**Ejemplo:**

$$
f(x) = \begin{cases}
x+1 & \text{si } x < 1\\
x^2  & \text{si } x \geq 1\\
\end{cases}
$$
**Evaluamos cuando $x<1:$**
$$
	\lim\limits_{x\to a}x+1\implies a+1= f(a)
$$
✅ $f(x)$ es continua $\forall x<1$


**Ahora evaluamos cuando $x>1:$**
$$
\lim\limits_{x\to a}x^2 \implies a^2 = f(a)
$$✅ $f(x)$ es continua $\forall x>1$


**Por ultimo evaluamos cuando $x=1$**

- $\lim\limits_{x\to 1^-}x^2=1$
- $\lim\limits_{x\to 1^+}x+1=2$

Los limites laterales son distintos -> $\nexists \lim\limits_{x\to 1}f(x)$

#### Conclusión

$f$ es continua en $\mathbb{R}-${1}

---
Ver [[Discontinuidad esencial y evitable]]