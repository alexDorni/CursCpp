1. Se dau numerele:
```cpp
 int a = 9996677889911556;
 int b = 9996677889911556;
```
Cerinta va fi data ulterior.

2. Verificati daca un numar este patrat perfect fara a folosi o bucla. 

3.  Realizati un program care umple un vector de 5 elemente cu o anumita valoare in felul urmator. Citeste un numar de la tastatura iar daca numarul este:
1 - vectorul va fi umplut cu 5;
3 - vectorul va fi umplut cu 4;
7 - vectorul va fi umplut cu  7;
0 in orice alt caz.

4. Ce va afisa urmatorul program?
```cpp
void functie (int a) {
    a++;
}

int main()
{
    int a = 5;
    functie(a);
    cout << a;
    return 0;
}
```

5. Ce va fisa urmatorul program?
```cpp
void functie (int a[5]) {
    for (int i = 0; i < 5; i++) {
        a[i]++;
    }
}

int main()
{
    int a[5] = {12, 5, 6, 8, 7};
    functie(a);
    for (int i = 0; i < 5; i++) {
        cout <<a[i]<<" ";
    }
    return 0;
}
```
