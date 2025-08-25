## ¿Qué es un puntero?

Un **puntero** es una variable especial que **almacena la dirección de memoria** de otra variable.  
En lugar de guardar un valor directo (por ejemplo, un número), un puntero guarda _dónde_ está almacenado ese número.

**Ejemplo:**

```c++
int x = 10;       // variable normal
int* p = &x;      // puntero a entero que guarda la dirección de x
```

## Declaración de punteros

```
tipo* nombrePuntero;
```

```c++
int* p;
cout << "variable sin asignar:" << p << endl;
p=new int();
cout << "variable con espacio reservado:" << p << endl;
```

```c++
int* p;
cout << "variable sin asignar:" << p << endl;
p=new int();

int a=20;
cout << "ref de a:" << &a << endl;
p=&a;
cout << "variable con espacio reservado:" << p << endl;
a=35;
cout << "dato apuntado por puntero:" << *p << endl;
```

```c++
void push(nodo*& pila,int info){ 
//crear el nodo nodo* p=new nodo(); 
//guardar la info 
p->info = info; p->sgte = pila; 
//apuntar pila al nodo nuevo 
pila=p; 
return; 
}
```

```c++
int pop(nodo*& pila){ 
int aux; 
nodo* p=pila; aux=p->info; 
pila=p->sgte; 
delete p; 
return aux; 
}
```


```c++
void queue(nodo*& cfte,nodo*& cfin, int info){ 
nodo* p=new nodo(); //guardar la info 
p->info = info; p->sgte = NULL; 
if(cfte==NULL){ 
	cfte=p; 
} else { cfin->sgte=p; } cfin = p; }
```


```c++
int unqueue(nodo*& cfte,nodo*& cfin) {
 //auxiliares 
int aux; 
nodo* p=cfte;
aux=p->info; 
cfte = p->sgte; 
if(cfte==NULL) {
 cfin=NULL; 
 } 
 delete p; 
 return aux; }
```


```c++
nodo* cfte=NULL;
	nodo* cfin = NULL;
		cout << "***************" << endl;
	info=20;
	queue(cfte,cfin,info);
	info=30;
	queue(cfte,cfin,info);
	info=40;
	queue(cfte,cfin,info);
	info=50;
	queue(cfte,cfin,info);
	cout << "COLA " << endl;
	cout << "***************" << endl;
	while(cfte!=NULL){
	 cout << unqueue(cfte,cfin) << endl;
	}
```