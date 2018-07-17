### Siruri de caractere

In C++ un sir de caractere (string) este reprezentat ca un vector de char; In acest vectori vor fi retinute literele, iar la sfarsit un caracter null marcat prin `\0`.

Pentru a initializa un sir de caractere se poate folosi aceeasi metoda ca la un vector normal:
```cpp
char cuvant[6] = {'H','e','l','l','o','\0'}
```

Sau se poate declara direct sirul de carcater dar intre *ghilimele* si fara a preciza dimensiunea vectorului
```cpp
char cuvant[] = "Hello";
```

Pentru a citi de la tastatura se foloseste metoda `gets(s1)` care va citi in variabila s1 pana la primul `Enter` (`\n`)
Pentru a afisa un sir de caractere se foloseste metoda `puts(s1)` care va afisa continutul variabile `s1`

Deoarece un sir de caractere este un vector se folosesc o serie de functii pentru a realiza operatiile cele mai frecvente:

- `strcpy(s1, s2);` - Copie string-ul s2 in stringul s1;
- `strcat(s1, s2);` - Concateneaza string-ul s2 la sfarsitul string-ului s1;
- `strlen(s1);` - Returneaza dimensiunea lui s1;
- `strcmp(s1, s2);` - Compara doua string-uri si returneaza:

      - 0 daca s1 si s2 sunt egale
      
      - o valoare mai mare ca 0 daca s1>s2
      
      - o valoare mai mica decat 0 daca s1<s2
      
- `strchr(s1, ch);` - Returneaza un string de la pozitia primei aparitii a caracterului `ch` in string-ul `s1`;
- `strstr(s1, s2);` - Returneaza un string de la pozitia primei aparitii a string-ului `s2` in string-ul `s1`;

Exemple:

##### strcpy(s1, s2)

```cpp
char s1[] = "Hello world";
char s2[12];
strcpy(s2, s1);
cout << s2; // "Hello world";
```

##### strcat(s1, s2)

```cpp
char s1[] = "Hello";
char s2[] = " world";
strcat(s1, s2);
cout << s1; // "Hello world";
```

##### strlen(s1)
```cpp
char s1[] = "Hello";
char s2[] = " world";
cout << strlen(s1); // 5
```
##### strcmp(s1, s2)
```cpp
char s1[] = "Hello";
char s2[] = "world";
cout << strcmp(s1, s2); // -1 - in ASCII s1 < s2; ATENTIE. Este posibil ca valoarea returnata sa nu fie -1 ci un alt numar mai mic decat 0
```    

##### strchr(s1, ch) 
```cpp
char s1[] = "Hello";
cout << strchr(s1, 'e'); // "ello"
```

##### strstr(s1, s2) 
```cpp
char s1[] = "world";
cout << strstr(s1, "rl"); // "rld"
```




      
