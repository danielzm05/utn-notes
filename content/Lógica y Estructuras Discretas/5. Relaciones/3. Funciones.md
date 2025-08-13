Sea una relación $F: A \to B$. Diremos que $F$ es función

1) **Cumple con Existencia:** Significa que todo elemento del primer conjunto debe relacionarse por lo menos con alguno del segundo.

$$
\forall x \in A: \exists y \in B: (x,y)\in F
$$

2) **Cumple con Unicidad:** Significa que un mismo elemento del primer conjunto no puede relacionarse con dos distintos del segundo, o sea debe tener imagen única.

$$
\forall x \in A: \forall y_{1}, y_{2} \in B: (x, y_{1})\in F ∧ (x, y_{2}) \in F \to y_{1}=y_{2}
$$


**Ejemplos:** 

$A$ = { 1 ,2,3} en $B$ = { 3, 4}

$F$ = { (1;3) , (2;4) , (3;4) } ✅**Es función**
$R$ = { (1;3) , (1;4) , (2;3) , (3;4) } ❌**No es función. No cumple con unicidad** (El $1$ tiene dos imágenes distintas)
$S$ = { (1;3) , (2;4) } ❌ **No es función. No cumple con el requisito de existencia** (el 3 no tiene imagen)

---
## Clasificación de funciones

#### Inyectiva
Elementos distintos del dominio tienen imágenes distintas. No pueden compartir imagen.

$$
\forall x_{1},x_{2} \in A, y\in B: F(x_{1})=y \land F(x_{2})=y \to x_{1}=x_{2}
$$
> *Si dos elementos del dominio se mapean al mismo valor, entonces deben ser el mismo elemento*


#### Sobreyectiva
Todos elementos de $B$ son imagen de por lo menos un elemento de $A$

$$
\forall y\in B: \exists x\in A \land F(x)=y \Longleftrightarrow \mathrm{Img}(F)=B
$$

#### Biyectiva
Cuando es inyectiva y sobreyectiva a la vez

> [!tip] Para que $F$ sea biyectiva  entre dos conjuntos finitos sus cardinalidades deben ser iguales

**Ejemplo:** Dados los conjuntos: $A$ = { a, b, c} y $B$ = { 1, 2, 3}

Como $|A|=|B|$ la función $F$ = {(a;1) , (b;3) , (c;2) } es biyectiva