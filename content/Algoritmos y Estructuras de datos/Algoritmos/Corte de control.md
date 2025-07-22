El corte de control es un proceso en el cual los registros del archivo se encuentran
agrupados u ordenados por el valor de uno o más campos, denominados campos clave o
llave, si hay ordenamiento este puede ser ascendente –el más común- o descendente.

Este tipo de proceso generalmente es utilizado para realizar informes o reportes, en el cual se deba emitir de cada grupo –formado por el mismo valor del campo clave-
totales, promedios, máximos o mínimos, etc

```c++
void corteControl(tr v[], int N)
{
    int i = 0;
    int control;
    while(i < N){
        control = v[i].id;
        cout << control << endl;
        
        while(i < N && control == v[i].id){
            cout << v[i].id;
            // ....................
            i++;
        }

        // Mostrar datos del subconjunto
    }

    // Mostrar datos totales
}
```

