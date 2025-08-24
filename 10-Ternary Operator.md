# Ternary Operator in C

## Syntax :

```c
test_condition ? expression1 : expression2;
```

## Example: Ternary Operator
### Example 1: 
```c
#include <stdio.h>

int main() {

  int age = 15;

  (age >= 18) ? printf("You can vote") : printf("You cannot vote");

  return 0;
}

```

**Output**
```
You cannot vote

```
### Example 2: 
```c
#include <stdio.h>

int main() {

  int age = 24;

  (age >= 18) ? printf("You can vote") : printf("You cannot vote");

  return 0;
}

```

**Output**
```
You can vote
```
## Example 3 : Using variable in ternary operator

```c
#include <stdio.h>

int main() {

  char operator = '+';

  int num1 = 8;
  int num2 = 7;

  int result = (operator == '+') ? (num1 + num2) : (num1 - num2);
  printf("%d", result);

  return 0;
}

```
**Output**
```
15
```

---
