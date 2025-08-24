# C Standard Library Functions

## Math Header File
**Example 1:** 
```c
#include <stdio.h>
#include <math.h>

int main() {

  int num = 25;
  printf("Square root is %lf", sqrt(num));

  return 0;
}

```

**Output**
```
Square root is 5.000000
```

**Example 2:**
```c
#include <stdio.h>
#include <math.h>

int main() {

  int num = 27;
  printf("Cube root is %lf", cbrt(num));

  return 0;
}
```

**Output**
```
Cube root is 3.000000
```
**Example 3:**
```c
#include <stdio.h>
#include <math.h>

int main() {

  int a = 5;
  int b = 2;

  double result = pow(a, b);
  printf("Power: %lf", result);

  return 0;
}
```
**Output**
```
Power: 25.000000
```

## Ctype Header File
```c
#include <stdio.h>
#include <ctype.h>

int main() {

  char alph = 'e';

  char upper = toupper(alph);
  printf("%c", upper);

  char lower = tolower(upper);
  printf("\n%c", lower);

  return 0;
}

```

**Output**
```
E
e
```
---
