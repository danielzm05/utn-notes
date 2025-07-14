Rama de la física que describe le movimiento de los objetos sin estudiar sus causas

**Partícula:** Objeto de dimensiones muy pequeñas que puede ocupar distintas posiciones en el espacio (el tamaño y la forma no se tienen en cuenta)

---

**Vector Posición $\vec{r}(t)$:** Segmento orientado que parte de un punto de referencia (llamado origen de coordenadas) y termina en la partícula.

>Nos indica dónde se encuentra un objeto, en un sistema de coordenadas

![[Cinemática.png]]


**Vector Desplazamiento $\vec{Δr}$:** Representa la diferencia entre la posición final y la posición inicial:
$$
\vec{Δr}= \vec{r}(t+Δt)-\vec{r}(t)
$$

---

## Velocidad

**Velocidad Media $\vec{{v_{m}}}$:**  Es un vector que me indica cual es la velocidad promedio de un objeto entre dos puntos. Se calcula dividiendo el vector desplazamiento $\vec{Δr}$  y el tiempo transcurrido.

$$
\vec{v_{m}}=\frac{\vec{Δr}}{Δt} = \frac{ \vec{r}(t+Δt)-\vec{r}(t)
}{t_{2}-t_{1}}
$$
> [!INFO] 
> $\vec{v_{m}}$ tendrá igual dirección y sentido que $\vec{Δr}$



**Velocidad Instantánea:** Velocidad que tiene un objeto en un instante especifico de tiempo. Se calcula como el limite del vector $\vec{v_{m}}$ cuando el intervalo de tiempo tiende a 0.
$$
\vec{v}=\lim\limits_{Δt\to 0}\frac{\vec{Δr}}{Δt} =\lim\limits_{Δt\to 0}\frac{ \vec{r}(t+Δt)-\vec{r}(t)
}{t_{2}-t_{1}}=\frac{d\vec{r}}{dt}
$$
>[!INFO] 
>La velocidad instantánea es *siempre* tangente a la trayectoria


---
## Aceleración

Aparece cuando en un movimiento, la velocidad cambia, es decir, no es constante.

> La aceleración mide la variación de la velocidad de un cuerpo con el tiempo.


**Vector Aceleración:** Nos indica como cambia la velocidad en el tiempo.

$$
\vec{a}(t)=\frac{d\vec{v}}{dt}
$$

- Si $\vec{a}(t)=0$ la velocidad es **constante**
- Si $\vec{a}(t) \neq 0$ la velocidad **cambia** (aumenta o disminuye)

**Vector Aceleración Media:**

$$
\vec{a_{m}}=\frac{Δ\vec{v}}{Δt}=\frac{v_{f}-v_{i}}{t_{f}-t_{i}}
$$
---

## MRU | Movimiento Rectilíneo uniforme

$x = x_0 + v t$
$v=$ *constante*
$a=0$

## MRUV | Movimiento Rectilíneo uniformemente variado

$x = x_0 + v_0 t + \frac{1}{2} a t^2$
$v = v_0 + a t$
$a=$ *constante*
