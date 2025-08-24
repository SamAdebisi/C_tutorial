# while loop in C Programming

### Syntax :

```c
while (condition) {
    // statements inside while
}


```

### Example 1 : infinite while loop
```c
#include <stdio.h>

int main() {

  while (1 < 5) {
    printf("while loop in C \n");
  }

  return 0;
}

```

**Output**
```
while loop in C 
while loop in C 
while loop in C 
while loop in C 
....

```

### Example 2 : while loop
```c
#include <stdio.h>

int main() {

  int count = 1;

  while (count < 5) {
    printf("while loop in C \n");
    printf("Count = %d \n", count);
    count = count + 1;
  }

  return 0;
}

```

**Output**
```
while loop in C 
Count = 1
while loop in C 
Count = 2
while loop in C 
Count = 3
while loop in C 
Count = 4

```
## Create Multiplication Table

```c
#include <stdio.h>

int main() {

  int number;
  printf("Enter the number: ");
  scanf("%d", &number);

  int count = 1;

  while (count <= 10) {
    int product = number * count;
    printf(" %d * %d = %d \n", number, count, product);
    count = count + 1;
  }

  return 0;
}


```
**Output**
```
Enter the number: 8
 8 * 1 = 8 
 8 * 2 = 16 
 8 * 3 = 24 
 8 * 4 = 32 
 8 * 5 = 40 
 8 * 6 = 48 
 8 * 7 = 56 
 8 * 8 = 64 
 8 * 9 = 72 
 8 * 10 = 80 

```

## do...while Loop

**Syntax :**

```c
do {
    // body of loop
} while(condition);
```
### Example 1: do..while
```c
#include <stdio.h>

int main() {

  int count = 1;

  do {
    printf("%d \n", count);
    count = count + 1;
  } while (count < 5);

  return 0;
}


```
**Output**
```
1 
2 
3 
4 

```
### Example 2: do...while loop with false condition
```c
#include <stdio.h>

int main() {

  int count = 5;

  do {
    printf("%d \n", count);
    count = count + 1;
  } while (count < 5);

  return 0;
}

```

**Output**
```
5 
```
---
