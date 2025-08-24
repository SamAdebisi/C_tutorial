# for Loop in C Programming

 **Syntax** :

```c
for (initializationExpression; testExpression; updateExpression) {
  // code inside the for loop
}

```

### Example 1 : print numbers from 0 to 9
```c
#include <stdio.h>

int main() {

  for (int i = 0; i < 10; i++) {
    printf("%d ", i);
  }

  return 0;
}

```

**Output**
```
0 1 2 3 4 5 6 7 8 9 

```

### Example 2 : print a message multiple times
```c
#include <stdio.h>

int main() {

  for (int i = 0; i < 10; i++) {
    printf("Emergency condition \n");
  }

  return 0;
}

```

**Output**
```
Emergency condition 
Emergency condition 
Emergency condition 
Emergency condition 
Emergency condition 
Emergency condition 
Emergency condition 
Emergency condition 
Emergency condition 
Emergency condition

```
### Sum of all the numbers from 1 to 100

```c
#include <stdio.h>

int main() {
  
  int sum = 0;
  
  for (int i = 1; i <= 100; i++) {
    sum = sum + i;
  }

  printf("Sum: %d", sum);
  return 0;
}

```
**Output**
```
Sum: 5050
```

### Sum of Even Numbers

```c
#include <stdio.h>

int main() {
  
  int sum = 0;
  
  for (int i = 2; i <= 100; i = i + 2) {
    sum = sum + i;
  }

  printf("Sum: %d", sum);
  return 0;
}

```
**Output**
```
Sum: 2550

```
---
