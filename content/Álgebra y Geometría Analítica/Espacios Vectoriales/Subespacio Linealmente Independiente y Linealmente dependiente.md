
## Subespacio linealmente independiente

Un subespacio es **linealmente independiente** si el conjunto de vectores que lo genera es linealmente independiente, es decir, **ninguno de los vectores del conjunto se puede escribir como combinación lineal de los demás**.  

**Ejemplo:**  
En $\mathbb{R}^3$, los vectores $v_1 = (1, 0, 0)$ y $v_2 = (0, 1, 0)$ forman un conjunto linealmente independiente.  
No se puede escribir uno como combinación lineal del otro, y cualquier combinación $a(1, 0, 0) + b(0, 1, 0) = (0, 0, 0)$ solo se cumple si $a = b = 0$.

---

## Subespacio linealmente dependiente

Un subespacio es **linealmente dependiente** si el conjunto de vectores que lo genera **contiene al menos un vector que puede expresarse como combinación lineal de los otros**.  


**Ejemplo:**  
En $\mathbb{R}^3$, los vectores $v_1 = (1, 2, 3)$, $v_2 = (2, 4, 6)$ y $v_3 = (0, 0, 1)$ son linealmente dependientes, ya que:  $v2=2⋅v1v_2 = 2 \cdot v_1v2​=2⋅v1​$ 
Por tanto, $v_2$ es combinación lineal de $v_1$, y el conjunto no es independiente.



> [!tip] Determinantes
> Un conjunto de vectores es linealmente dependiente (LD) si el determinante de la matriz formada por esos vectores ==es igual a cero==. Si el determinante es distinto de cero, el conjunto es linealmente independiente (LI).