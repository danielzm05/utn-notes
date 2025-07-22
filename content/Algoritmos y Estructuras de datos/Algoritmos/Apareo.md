El **algoritmo de apareo** es un procedimiento utilizado para combinar dos conjuntos de datos **homogéneos**, representados como archivos o vectores, **ordenados por un mismo campo clave**, con el objetivo de generar un **nuevo conjunto único** que contenga **todos los elementos de ambos conjuntos originales**, manteniendo el **orden ascendente según el campo clave**.

```c++
void apareo(tr v1[], int N, tr v2[], int M)
{
    int i = 0;
    int j = 0;
    
    while(i < N && j < M){
        if(v1[i].id < v2[j].id){
            procesar v1[i];
            i++;
        }
        else{
            procesar v2[j];
            j++;
        }
    }
    while(i < N){
        procesar v1[i];
        i++;
    }
    while(j < M){
        procesar v2[j];
        j++;
    }
    return;
}
```


**Otro Modelo:**

```c++

void apareo(tr v1[], int N, tr v2[], int M)
{
    int i = 0;
    int j = 0;
    while(i < N || j < M){
        if(j == M || (i < N && v1[i].c1 < v2[j].c1)){
            procesar v1[i];
            i++;
        }
        else{
            procesar v2[j];
            j++;
        }
    }
    return;
}
```
