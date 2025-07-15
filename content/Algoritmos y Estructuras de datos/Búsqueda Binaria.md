> [!caution] El arreglo debe ir siempre en forma ascendente


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
      
    }else{

      if(dato>num[mitad]){
      inf=mitad;
      mitad=(inf+sup)/2;

      }else if(dato<num[mitad]){

        sup=mitad;
        mitad=(inf+sup)/2;

      }

    }

  }

    return -1; //No se encontro la posición

}
```