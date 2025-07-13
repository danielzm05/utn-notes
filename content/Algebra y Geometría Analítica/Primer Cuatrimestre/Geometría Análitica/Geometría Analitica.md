**Elementos de un vector: [[Geometría Analitica| Norma, dirección, sentido, modulo]]**
**Modulo del vector:** $|\vec{v}|=\sqrt{{v_{x}}^{2} +{v_{y}}^{2} }$
**Tipos de Vectores:** [[Versor , Vector Nulo , Opuesto y Equipolente]]

**Método del Paralelogramo**

![[Pasted image 20250602172612.png|300]]

**Multiplicación de un vector por un escalar**
$K*\vec{a}=(K*a_{x}, K*a_{y}, K*a_{z})$

**Producto Escalar**
$\vec{a}*\vec{b}=|\vec{a}|*|\vec{b}|*\cos(a)$

- $\vec{a}*\vec{a}=|a|^{2}$
- Si $\vec{a}*\vec{b}=0$  $\to \vec{a} \perp \vec{b}$
- Angulo entre vectores: $\cos(a)= \frac{\vec{a}*\vec{b}}{|\vec{a}|*|\vec{b}|}$ 

**Producto Vectorial**
$\vec{a} \times \vec{b}$
- Norma: $\|\vec{a} \times \vec{b}\| = \|\vec{a}\| \cdot \|\vec{b}\| \cdot \sin(\theta)$
-  Si $\vec{a}\times  \vec{b}=0$ entonces $\vec{a} \parallel  \vec{b}$

**Producto Mixto**

$(\vec{a}\times \vec{b} )\cdot \vec{c}=0$
- Si $(\vec{a}\times \vec{b} )\cdot \vec{c}=0$ Entonces $\vec{a},\vec{b}, \vec{c}$ son coplanares
---
### Vector Proyección
$$\vec{\text{proj}}_{\vec{b}} \vec{a} = \left( \frac{\vec{a} \cdot \vec{b}}{|\vec{b}|^{2}} \right) \vec{b}$$
- Donde $\vec{\text{proj}}_{\vec{b}} \vec{a}$ $\parallel \vec{b}$

- **Módulo del vector Proyección**
$\left\| \vec{\text{proj}}_{\vec{b}} \vec{a} \right\| = \frac{|\vec{a} \cdot \vec{b}|}{\|\vec{b}\|}$

---
### Ecuaciones de la recta

- **Ecuación vectorial paramétrica** $r=\vec{\theta P_{0}}+\lambda\vec{v}$

- **Ecuación vectorial cartesiana paramétrica** $r\begin{cases} x = x_0 + \lambda v_{x} \\y = y_0 + \lambda v_{y} \\z = z_0 + \lambda v_{z} \end{cases}$

- **Ecuación simétrica**: $\frac{x - x_0}{v_{x}} = \frac{y - y_0}{v_{y}} = \frac{z - z_0}{v_{z}}$

#### Rectas Alabeadas
Dos rectas serán alabeadas si $\vec{v_{1}} \times \vec{v_{2}}  \cdot  \vec{P_{1}P_{2}}\neq0$
![[Pasted image 20250606170000.png]]

**Distancias entre rectas alabeadas**
$d= \frac{|\vec{v_{1}} \times \vec{v_{2}}  \cdot  \vec{P_{1}P_{2}}|}{| \vec{v_{1} \times \vec{v_{2}}|}}$

### Distancia de un punto a una recta 

$d= \frac{|\vec{Pop} \times \vec{v}|}{|\vec{v}|}$

---
### Distancia de un punto a un plano

$d=\frac{|A \cdot P_{x}+B\cdot P_{y}+C\cdot Pz+D|}{\sqrt{ A^{2}+B^{2}+C^{2}}}$

---
### Ecuaciones del Plano

- **Ecuación Normal** $\vec{Pop} \cdot    \vec{n}$
- **Ecuación General** $ax + by + cz + D = 0$ ($(a,b,c)$ es el vector director)
- **Ecuación Vectorial** $Po + \alpha \cdot \vec{v_{1}}+ \beta \cdot \vec{v_{2}}$


## Intersección entre recta y plano
Recta:  ${x = 1 + 2t,\ y = -1 + t,\ z = 3 - t}$

Plano:  ${x + y + z - 4 = 0}$

Sustituimos:
$$(1 + 2t) + (-1 + t) + (3 - t) - 4 = 0 \Rightarrow t = 1$$

Punto de intersección:
${x = 3,\ y = 0,\ z = 2}$ → **(3, 0, 2)**


