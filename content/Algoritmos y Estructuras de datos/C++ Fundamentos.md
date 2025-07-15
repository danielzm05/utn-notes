
#### Estructura básica de un programa en C++

Un programa típico en C++ comienza con la inclusión de bibliotecas necesarias, seguido del espacio de nombres (`namespace`) y la función principal `main`.

```cpp
#include <iostream> // Biblioteca para entrada/salida

using namespace std;

int main() { //punto de entrada
    // Código aquí
    return 0;
}
```


---
#### Variables y declaración

Una **variable** es un espacio en memoria donde se almacena un valor. En C++, antes de usar una variable, se debe declarar su tipo.

Ejemplos:

```cpp
int edad = 25;         // Variable entera 
float altura = 1.75;   // Variable decimal 
char letra = 'A';      // Variable de un solo carácter 
bool activo = true;    // Variable booleana
```

---
#### Comentarios

Los comentarios sirven para documentar el código y no se ejecutan.

```cpp
// Esto es un comentario de una línea

/* 
   Esto es un comentario
   de múltiples líneas
*/
```

---
#### Entrada y salida estándar

- `cout`: muestra información al usuario
- `cin`: recibe información del usuario

```cpp
int edad;
cout << "Introduce tu edad: ";
cin >> edad;
```


---

#### Operadores lógicos

Se utilizan para construir expresiones lógicas:

- `&&`: AND lógico (ambas condiciones deben ser verdaderas)
- `||`: OR lógico (al menos una condición debe ser verdadera)
- `!`: NOT lógico (niega una condición)


---

#### Condicionales

Permiten ejecutar código dependiendo de una condición.

```cpp
if (condicion) {
    // Código si la condición es verdadera
} else {
    // Código si la condición es falsa
}
```

También se puede usar `else if` para múltiples condiciones:

```cpp
if (edad < 18) {
    cout << "Es menor de edad.";
} else if (edad == 18) {
    cout << "Tiene justo 18 años.";
} else {
    cout << "Es mayor de edad.";
}
```

---
Otros conceptos:
- [[Bucles en C++]]
- [[Funciones en C++]]
