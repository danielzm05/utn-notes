La **búsqueda lineal** o la **búsqueda secuencial** es un método para encontrar un valor objetivo dentro de una vector. Ésta comprueba secuencialmente cada elemento de la lista para el valor objetivo hasta que es encontrado o hasta que todos los elementos hayan sido comparados.


> [!warning] Alto costo de rendimiento
> La búsqueda secuencial es en tiempo el peor, y marca como máximo n comparaciones, donde n es la longitud de la lista. Por lo que es aconsejable utilizarlo en listas cortas.
> 
> Para vectores de gran tamaño se aconseja utilizar [[Búsqueda Binaria]]

**Ejemplo:**

```c++
int busquedaSecuencial(int vec[], int buscado){
	for(int i=0; i<n; i++){
		if(vec[i]==buscado){
			return i;  // Se encontró la posición del dato
		}
	}
	return -1; //No se encontró
}
```

