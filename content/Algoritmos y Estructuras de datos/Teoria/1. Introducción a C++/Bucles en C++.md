Permiten repetir instrucciones múltiples veces de forma controlada. En C++ existen tres tipos principales de bucles: `for`, `while` y `do-while`. 

Los bucles son útiles para:

- Repetir tareas una cantidad específica de veces
- Recorrer estructuras de datos (como vectores, listas, arreglos)
- Ejecutar acciones hasta que se cumpla una condición

---

#### Bucle `for`

El bucle `for` se usa cuando se conoce de antemano cuántas veces se debe ejecutar una instrucción.

**Estructura**

```
for (inicialización; condición; incremento) {
    // Código a repetir
}
```

**Ejemplo**

```cpp
#include <iostream>
using namespace std;

int main() {
    for (int i = 0; i < 5; i++) {
        cout << "Iteración: " << i << endl;
    }
    return 0;
}
```

---

#### Bucle `while`

Se ejecuta **mientras** la condición sea verdadera. La condición se evalúa antes de cada iteración.

>Este tipo de bucle es útil cuando **no se conoce con certeza cuántas veces** se debe repetir una instrucción, pero sí se conoce la condición de parada.


```cpp

#include <iostream>
using namespace std;

int main() {
    int i = 0;
	while (i < 5) {
		cout << "Iteración: " << i << endl;
		i++;
	}
}

```


#### Bucle `do-while`

Similar al `while`, pero la condición se evalúa **después** de ejecutar el bloque de código. Por lo tanto, se ejecuta al menos una vez.

```cpp
int i = 0;
do {
    cout << "Iteración: " << i << endl;
    i++;
} while (i < 5);
```


---

 **Instrucciones `break` y `continue`**
 
 - `break`: finaliza el bucle actual inmediatamente.
- `continue`: salta el resto del bloque y pasa a la siguiente iteración.

```cpp
for (int i = 0; i < 10; i++) {
    if (i == 5) break;       // Sale del bucle cuando i es 5
    if (i % 2 == 0) continue; // Salta los números pares
    cout << i << " ";
}
```


