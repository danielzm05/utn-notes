#### Burbujeo Creciente

```cpp
void Burbujeo(Sucursal sucursal[], int n){

  int i, j;
  Sucursal aux;


  for ( i = 1; i < n; i++)
  {
    for ( j = 1; j < n ; j++)
    {
      if(sucursal[j-1].codSucursal > sucursal[j].codSucursal){

        aux=sucursal[j-1];
        sucursal[j-1]=sucursal[j];
        sucursal[j] = aux;

      }
    }
  }
}
```


#### Burbujeo Decreciente

```cpp
void BurbujeoD(Sucursal sucursal[], int n){

  int i, j;
  Sucursal aux;

  for ( i = 1; i < n; i++) {

    for ( j = 1; j < n ; j++) {

      if(sucursal[j-1].codSucursal < sucursal[j].codSucursal){

        aux=sucursal[j-1];
        sucursal[j-1]=sucursal[j];
        sucursal[j] = aux;
      }
    }
  }
}
```

---

Ejemplo de uso:

```cpp
#include <iostream>
#include <cstring>
using namespace std;


struct Sucursal{
  int codSucursal;
  char nombre[50+1];
};

  

int main(){

  int cant,i;
  char nombre[50+1];
  void Burbujeo(Sucursal[], int);
  void Imprimir(Sucursal[], int);

  cout<<"Ingrese la cantidad de sucursales:";
  cin>> cant;

  Sucursal sucursal[cant];

  for ( i = 0; i < cant; i++){

    cout<<"Ingrese el codigo de la sucursal"<<i+1<<":";
    cin>>sucursal[i].codSucursal;
    cout<<"Ingrese el nombre de la sucursal"<<i+1<<":";
    cin>>nombre;
    strcpy(sucursal[i].nombre, nombre);
  }

  

  cout <<"Creciente:"<<endl;
  Burbujeo(sucursal, cant);
  Imprimir(sucursal, cant);

  return 0;

}

  

void Imprimir(Sucursal sucursal[], int n){

  for(int i=0; i<n; i++){
    cout<<sucursal[i].codSucursal<<endl;
  }
}

  

void Burbujeo(Sucursal sucursal[], int n){

  int i, j;
  Sucursal aux;

  for ( i = 1; i < n; i++) {
  
    for ( j = 1; j < n ; j++){

      if(sucursal[j-1].codSucursal > sucursal[j].codSucursal){

        aux=sucursal[j-1];
        sucursal[j-1]=sucursal[j];
        sucursal[j] = aux;

      }

    }

  }

}

  
```