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

