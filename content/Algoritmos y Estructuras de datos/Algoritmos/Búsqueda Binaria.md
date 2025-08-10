La **búsqueda binaria** funciona en arreglos ordenados. Este algoritmo comienza por comparar el elemento del medio del arreglo con el valor buscado. Si el valor buscado es igual al elemento del medio, su posición en el arreglo es retornada. Si el valor buscado es menor o mayor que el elemento del medio, la búsqueda continua en la primera o segunda mitad, respectivamente, dejando la otra mitad fuera de consideración.

> [!quote] El arreglo debe ir siempre en forma ascendente

**Estructura:**

```c++
Int busBin(int v[], int aBuscar, int N, int &inicio){ 

inicio = 0;
int final = N-1;
int mitad; 

while(inicio <= final){
	mitad = (inicio + final )/2; 
	
	if (v[mitad].id == aBuscar){
		return mitad;
	}
	
	if(aBuscar>v[m].id){
		inicio = m+1; 
	}else{
		final = m-1; 
	}
}
return -1; //No se encontró la posición
}

```


**Ejemplo:**

```cpp
#include <iostream>
using namespace std;

int main(){

  int num[]={1,2,3,4,5}; 
  int inf=0, sup=5;
  int dato=4;

  return 0;
}

int BusquedaBinaria(int inf, int sup, int num[], int dato){

  int mitad;

  while(inf<=sup){

    mitad=(inf+sup)/2;
    
    if(dato == num[mitad]){
      return mitad;
      
    }

	if(dato>num[mitad]){
	  inf=mitad;
	  mitad=(inf+sup)/2;
	
	}else if(dato<num[mitad]){
	
		sup=mitad;
		mitad=(inf+sup)/2;
	}

  }

    return -1; 

}
```