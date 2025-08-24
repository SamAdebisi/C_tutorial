# Switch Statement in C Programming 

### Syntax :

```c
switch(variable/expression) {
    case value1:  
        // body of case 1
        break;

    case value2:  
        // body of case 2
        break;

    case valueN:
        // body of case N
        break;

    default:
        // body of default
}

```

### Example 1 : print the day of a week
```c
#include <stdio.h>

int main() {

  int number;
  printf("Enter a number between 1 to 7: ");
  scanf("%d", &number);

  switch(number) {
    case 1:
      printf("Sunday");
      break;

    case 2:
      printf("Monday");
      break;

    case 3:
      printf("Tuesday");
      break;

    case 4:
      printf("Wednesday");
      break;

    case 5:
      printf("Thursday");
      break;

    case 6:
      printf("Friday");
      break;

    case 7:
      printf("Saturday");
      break;

    default:
      printf("Invalid Number");
  }

return 0;
}

```

**Output**
```
Enter a number between 1 to 7: 5
Thursday

```
### Example 2 : Removing break statement from previous example
```c
#include <stdio.h>

int main() {

  int number;
  printf("Enter a number between 1 to 7: ");
  scanf("%d", &number);

  switch(number) {
    case 1:
      printf("Sunday ");

    case 2:
      printf("Monday ");

    case 3:
      printf("Tuesday ");

    case 4:
      printf("Wednesday ");

    case 5:
      printf("Thursday ");

    case 6:
      printf("Friday ");

    case 7:
      printf("Saturday ");

    default:
      printf("Invalid Number");
  }

return 0;
}

```

**Output**
```
Enter a number between 1 to 7: 5
Thursday Friday Saturday Invalid Number

```
## switch with multiple case

```c
#include <stdio.h>

int main() {

  int number;
  printf("Enter a number between 1 to 7: ");
  scanf("%d", &number);

  switch(number) {
    case 2:
    case 3:
    case 4:
    case 5:
    case 6:
      printf("Weekday");
      break;
      
    case 1:
    case 7:
      printf("Weekend");
      break;

    default:
      printf("Invalid Number");
  }

return 0;
}

```
**Output**
```
Enter a number between 1 to 7: 4
Weekday

```

## Simple Calculator

```c
#include <stdio.h>

int main() {

  char operator;
  printf("Choose an operator ['+', '-', '*', '/']: ");
  scanf("%c", &operator);
  
  double num1, num2;
  
  printf("Enter first number: ");
  scanf("%lf", &num1);
  
  printf("Enter second number: ");
  scanf("%lf", &num2);
  
  double result;

  switch(operator) {
    case '+':
      result = num1 + num2;
      break;
    case '-':
      result = num1 - num2;
      break;
    case '/':
      result = num1 / num2;
      break;
    case '*':
      result = num1 * num2;
      break;

    default:
      printf("Invalid Operator");
  }
  
  printf("%.2lf", result);

return 0;
}

```
**Output**
```
Choose an operator ['+', '-', '*', '/']: +
Enter first number: 8
Enter second number: 12
20.00

```
---
