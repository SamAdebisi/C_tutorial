# C Booleans and Comparison Operator

## if Statement in C Programming

```c
Syntax :

if (test_condition) {
  // body of if statement
}
```

### Example 1: if Statement
```c
#include <stdio.h>

int main() {
  int age;

  printf("Enter your age: ");
  scanf("%d", &age);

  if (age >= 18) {
    printf("You are eligible to vote");
  }

  return 0;
}
```

**Output**
```
Enter your age: 31
You are eligible to vote
```
### Example 2: if Statement
```c
#include <stdio.h>

int main() {
  int age;

  printf("Enter your age: ");
  scanf("%d", &age);

  if (age >= 18) {
    printf("You are eligible to vote");
  }

  if (age < 18) {
    printf("Sorry, you are not eligible to vote");
  }

  return 0;
}
```

**Output**
```
Enter your age: 15
Sorry, you are not eligible to vote
```
## if...else Statement

```c
Syntax: 

if (test_condition) {
  // statements inside if body
}
else {
  // statements inside else body
}
```

### Example : if .. else Statement

```c
#include <stdio.h>

int main() {

  int age = 15;

  if (age >= 18) {
    printf("You are eligible to vote");
  }

  else {
    printf("Sorry, you are not eligible to vote");
  }

  return 0;
}
```

**Output**
```
Sorry, you are not eligible to vote
```

## else if Statement

```c
Syntax: 

if (test_condition1) {
    // statements1
}
else if (test_condition2){
    // statements2
}
else {
    // statements3
}

```
### Example 1: else if statement

```c
#include <stdio.h>

int main() {

  int age = 130;

  if (age > 120) {
    printf("Invalid Age");
  }

  else if (age < 0) {
    printf("Invalid age");
  }

  else if (age >= 18) {
    printf("You are eligible to vote");
  }

  else {
    printf("Sorry, you are not eligible to vote");
  }

  return 0;
}
```

**Output**
```
Invalid Age
```

### Example 2: else if statement

```c
#include <stdio.h>

int main() {

  int age = -4;

  if (age > 120) {
    printf("Invalid Age");
  }

  else if (age < 0) {
    printf("Invalid age");
  }

  else if (age >= 18) {
    printf("You are eligible to vote");
  }

  else {
    printf("Sorry, you are not eligible to vote");
  }

  return 0;
}
```
**Output**

```
Invalid age
```
### Example 3: Using logical operator to combine the conditions

```c
#include <stdio.h>

int main() {

  int age = -1;

  if (age > 120 || age < 0) {
    printf("Invalid Age");
  }

  else if (age >= 18) {
    printf("You are eligible to vote");
  }

  else {
    printf("Sorry, you are not eligible to vote");
  }

  return 0;
}

```
**Output**
```
Invalid Age
```
---
