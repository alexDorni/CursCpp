### Functii utile

##### Calculul timpului curent
- se adauga `#include <ctime>`
- timpul este dat de functia `time(0)` si este de tipul long

Exemplu de program
```cpp
#include <iostream>
#include <ctime>

using namespace std;

int main()
{
    long currentTime = time(0);
    cout << "Current time:" << currentTime;
    return 0;
}
```

##### Generarea de numere random
- se adauga `#include <ctime>` si `#include <cstdlib>`
- se initializeaza un "punct de plecare" (seed) pentru generarea valorilor random cu timpul curent `srand(time(NULL))`
- se apeleaza metoda `rand()`
- pentru a genera numere dintr-un anumit interval se foloseste formula `rand()%(maxim - minim) + minim`

Exemplu de program (genereaza 10 numere random intre 32 si 100)
```cpp
#include <iostream>
#include <ctime>
#include <cstdlib>

using namespace std;

int main()
{
    int minim = 32;
    int maxim = 100;
    srand(time(NULL));
    for (int i = 0; i < 10; i++) {
        cout << "Number:" << rand()%(maxim - minim) + minim << "\n"; // numere intre 32 si 100
    }
    return 0;
}
```
