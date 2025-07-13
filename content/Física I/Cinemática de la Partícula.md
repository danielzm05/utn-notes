**Partícula:** Objeto de dimensiones muy pequeñas que puede ocupar distintas posiciones en el espacio ( el tamaño y la forma no se tienen en cuenta)

**Vector Posición $\vec{r}(t)$:** Segmento orientado que parte de un punto de referencia (llamado origen de coordenadas) y termina en la partícula.
![[Pasted image 20250509081242.png|600]]
**Vector Desplazamiento $\vec{Δr}$:** Representa la variación del vector posición entre el tiempo $t$ y $t+Δt$, y se calcula: $\vec{Δr}= \vec{r}(t+Δt)-\vec{r}(t)$


> [!INFO] ¿Quién es $Δt$?
> Es la variación del tiempo y se calcula: $Δt=t_{2}-t_{1}$ donde $t_{2}>t_{1}$

---

**Velocidad Media $\vec{vm}$:** Es un vector que me indica cual es la velocidad promedio de un objeto entre dos puntos.
$$\vec{vm}=\frac{\vec{Δr}}{Δt} = \frac{ \vec{r}(t+Δt)-\vec{r}(t)
}{t_{2}-t_{1}}$$
> [!info]
> $\vec{vm}$ tendrá igual dirección y sentido que $\vec{Δr}$

---
**Velocidad Instantánea:** Velocidad que tiene un objeto en un instante especifico de tiempo. Se calcula como el limite del vector $\vec{vm}$ cuando el intervalo de tiempo tiende a 0.
$$\vec{v}=\lim\limits_{x\to 0}\frac{\vec{Δr}}{Δt} =\lim\limits_{x\to 0}\frac{ \vec{r}(t+Δt)-\vec{r}(t)
}{t_{2}-t_{1}}=\frac{d\vec{r}}{dt}$$
>[!INFO]
> La velocidad instantánea es *siempre* tangente a la trayectoria

**Vector variación de la velocidad instantánea**:
Representa la variación de velocidad en un intervalo de tiempo.

$$Δ\vec{v}= \vec{v}(t+Δt)-\vec{v}(t)$$

---
**Vector Aceleración:** Nos indica como cambia la velocidad en el tiempo.

$$\vec{a}(t)=\frac{d\vec{v}}{dt}$$

- Si $\vec{a}(t)=0$ la velocidad es **constante**
- Si $\vec{a}(t) \neq 0$ la velocidad **cambia** (aumenta o disminuye)

**Vector Aceleración Media:**

$\vec{a_{m}}=\frac{Δ\vec{v}}{Δt}$
