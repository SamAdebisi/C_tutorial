# break and continue in C Programming

### break inside the loop
```c
#include <stdio.h>

int main() {

  for (int i = 1; i <= 5; i++) {
    printf("%d \n", i);
    break;
  }

  return 0;
}

```

**Output**
```
1

```

### break statement with decision making statement
```c
#include <stdio.h>

int main() {

  for (int i = 1; i <= 5; i++) {

    if (i == 3) {
      break;
    }

    printf("%d \n", i);
  }

  return 0;
}

```

**Output**
```
1
2
```
## break with while loop

```c
#include <stdio.h>

int main() {

  while (1) {
    int number;
    printf("Enter a number: ");
    scanf("%d", &number);
    
    if (number < 0) {
      break;
    }
    
    printf("%d \n", number);
  }

  return 0;
}

```
**Output**
```
Enter a number: 5
5
Enter a number: 9
9
Enter a number: -4

```

## continue Statement
```c
#include <stdio.h>

int main() {

  for (int i = 1; i <= 5; i++) {

    if (i == 3) {
      continue;
    }

    printf("%d \n", i);
  }

  return 0;
}

```
**Output**
```
1
2
4
5

```
## Example: break and continue
```c
#include <stdio.h>

int main() { 

  while (1) { 
    int number;
    printf("Enter a number: ");
    scanf("%d", &number);
    
    if (number <= 0) {
      break;
    }
    
    if ((number % 2) != 0) {
      continue;
    }

    printf("%d \n", number);
  }

  return 0;
}
```
**Output**
```
Enter a number: 4
4
Enter a number: 7
Enter a number: 32
32
Enter a number: -3

```


---
