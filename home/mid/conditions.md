# Conditions

_**Conditions-Related Problems and Solutions**_

#### **Problem-1**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705348302947/bcb58b80-4bef-4c7c-8b2d-191f3fe3f192.png)

```c
#include<stdio.h>
int main()
{
   double number ;
   printf("Enter a number:");
   scanf("%lf",&number);
   if(number>=0)
    printf("Positive");
   else
    printf("Negative");
   return 0;
}
```

***

#### **Problem-2**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705348729544/1db9e2fb-8ad1-436f-9ec8-acd2ad2f39d0.png)

```c
#include<stdio.h>
int main()
{
   int number ;
   printf("Enter a number:");
   scanf("%d",&number);
   if(number%2==0)
    printf("Even");
   else
    printf("Odd");
   return 0;
}
```

***

#### **Problem-3**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705348799666/4bf19858-def2-4217-a8db-b29ef108fc42.png)

```c
#include <stdio.h>

int main() {
int digit;

printf("Enter a single digit (0-9): ");
scanf("%d", &digit);

switch (digit) {
case 0:
printf("Zero\n");
break;
case 1:
printf("One\n");
break;
case 2:
printf("Two\n");
break;
case 3:
printf("Three\n");
break;
case 4:
printf("Four\n");
break;
case 5:
printf("Five\n");
break;
case 6:
printf("Six\n");
break;
case 7:
printf("Seven\n");
break;
case 8:
printf("Eight\n");
break;
case 9:
printf("Nine\n");
break;
default:
printf("Invalid input.\n");
}
return 0;
}
```

***

#### **Problem-4**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705348912790/27545ea7-115c-4305-bf5b-be664a56d623.png)

```c
#include<stdio.h>
int main()
{
 int a,b,c;
 printf("Enter Three angles:");
 scanf("%d%d%d",&a,&b,&c);
 if(a>0 && b>0 && c>0 && a+b+c==180)
    printf("Yes");
 else
    printf("No");
 return 0;
}
```

***

#### **Problem-5**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705348988033/fef7dc10-7c68-488e-9433-a6f7f856def3.png)

```c
#include <stdio.h>
int main() {
unsigned int a;
printf("Enter a positive nonzero number: ");
scanf("%u", &a);
if (a > 0 && (a & (a - 1)) == 0)
printf("YES");
else
printf("NO");
return 0;
}
```

***

#### **Problem-6**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705349050139/63a7706b-253c-4532-bf05-f470b6221f82.png)

```c
#include <stdio.h>

int main() {
int number;

printf("Enter a number: ");
scanf("%d", &number);

if (number > 0) {
if ((number & (number - 1)) == 0) {
printf("The number is a positive power of 2.\n");
} else {
printf("The number is positive but not a power of 2.\n");
}
} else if (number == 0) {
printf("Zero is not a valid input.\n");
} else {
printf("Negative input is not valid.\n");
}

return 0;
}
```

***

#### **Problem-7**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705349154708/d23b822c-e5ec-4bc3-b1b5-11e40e8aa1bb.png)

```c
#include<stdio.h>
int main()
{
    int X,Y;
    printf("Enter Two Number:");
    scanf("%d%d",&X,&Y);
    if(X>Y)
    printf("%d is greater than %d",X,Y);
    else if(X<Y)
    printf("%d is less than %d",X,Y);
    else
    printf("%d is equal to %d",X,Y);
    return 0;
}
```

***

#### **Problem-8**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705349203486/c1396f5f-612d-4b8d-841a-6ac7ef707196.png)

```c
#include <stdio.h>

int main() {
int year;
printf("Enter a year: ");
scanf("%d", &year);
if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) 
printf("YES");
else 
printf("NO");
return 0;
}
```

***

#### **Problem-9**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705349263242/3320a41b-5e10-4d41-a228-ba5526168ee8.png)

```c
#include<stdio.h>
int main()
{
    char ch;
    printf("Enter Character:");
    scanf("%c",&ch);
    if(ch>='A'&& ch<='Z'||ch>='a'&& ch<='z')
        printf("Alpabet\n");
    else if (ch>='0'&& ch<='9')
        printf("Digit\n");
    else
        printf("Special");
    return 0 ;
}
```

***

#### **Problem-10**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705349407087/e31b564c-f1a3-4fb4-8534-949e07b83cad.png)

```c
#include <stdio.h>
int main() {
double num1, num2;
char operator;

printf("Enter an expression ( 7 + 3): ");
scanf("%lf %c %lf", &num1, &operator, &num2);

switch (operator) {
case '+':
printf("ADD: %lf\n", num1 + num2);
break;
case '-':
printf("SUB: %lf\n", num1 - num2);
break;
case '*':
printf("MULTI: %lf\n", num1 * num2);
break;
case '/':
if (num2 != 0) {
printf("DIVI: %lf\n", num1 / num2);
} else {
printf("Zero as divisor is not valid!.\n");
}
break;
default:
printf("Invalid operator.\n");
}

return 0;
}
```

***

#### **Problem-11**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705349478664/a92630ee-31f1-4a8a-8fe9-532f5a1bf677.png)

```c
#include <stdio.h>
int main() {
double finalScore;

printf("Enter the final score: ");
scanf("%lf", &finalScore);

if (finalScore >= 90) {
printf("Grade: A\n");
}
else if (finalScore >= 86) {
printf("Grade: A-\n");
}
else if (finalScore >= 82) {
printf("Grade: B+\n");
}
else if (finalScore >= 78) {
printf("Grade: B\n");
}
else if (finalScore >= 74) {
printf("Grade: B-\n");
}
else if (finalScore >= 70) {
printf("Grade: C+\n");
}
else if (finalScore >= 66) {
printf("Grade: C\n");
}
else if (finalScore >=62) {
printf("Grade: C-\n");
}
else if (finalScore >= 58) {
printf("Grade: D+\n");
}
else if (finalScore >= 55) {
printf("Grade: D\n");
}
else {
printf("Grade: F\n");
}

return 0;
}
```

***

#### **Problem-12**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705349555194/b8f745ec-d1b7-46bc-aaf9-ac75efcf4cdc.png)

```c
#include <stdio.h>
int main() {
double a, b, result;
int choice;

printf("Enter two real numbers a and b: ");
scanf("%lf %lf", &a, &b);

printf("Choose an operation:\n");
printf("1. Addition\n");
printf("2. Subtraction\n");
printf("3. Multiplication\n");
printf("4. Division (quotient)\n");
scanf("%d", &choice);

switch (choice) {
case 1:
result = a + b;
break;
case 2:
result = a - b;
break;
case 3:
result = a * b;
break;
case 4:
if (b != 0) {
result = a / b;
} else {
printf("Division by zero is invalid.\n");
return 1;
}
break;
default:
printf("Invalid choice.\n");
return 1;
}

printf("Result: %lf\n", result);

return 0;
}
```

***

#### **Problem-13**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705349765784/ecf5eabc-76d5-4d63-9d67-f5e460d75bd2.png)

```c
#include <stdio.h>

int main() {
double a, b, result;
int choice, caseChoice;

printf("Enter two real numbers a and b: ");
scanf("%lf %lf", &a, &b);

printf("Choose an operation:\n");
printf("1. Addition\n");
printf("2. Subtraction\n");
printf("3. Multiplication\n");
printf("4. Division (quotient and remainder)\n");
scanf("%d", &choice);

switch (choice) {
case 1:
result = a + b;
break;
case 2:
result = a - b;
break;
case 3:
result = a * b;
break;
case 4:
printf("Choose a case:\n");
printf("1. Quotient\n");
printf("2. Remainder\n");
scanf("%d", &caseChoice);
if (b != 0) {
if (caseChoice == 1) {
result = a / b;
} 
else if (caseChoice == 2) {
result = fmod(a, b);
}
 else {
printf("Invalid case choice.\n");
return 1;
}
} 
else {
printf("Error: Division by zero.\n");
return 1;
}
break;
default:
printf("Invalid choice.\n");
return 1;
}

printf("Result: %lf\n", result);

return 0;
}
```

***

#### **Problem-14**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705349841271/5c1295c0-8261-4f7a-9d5c-6f1c1caa6a20.png)

```c
#include <stdio.h>

int main() {
double a, b, result;
int choice, caseChoice;

printf("Enter two real numbers a and b: ");
scanf("%lf %lf", &a, &b);

printf("Choose an operation:\n");
printf("1. Addition\n");
printf("2. Subtraction\n");
printf("3. Multiplication\n");
printf("4. Division\n");
scanf("%d", &choice);

switch (choice) {
case 1:
result = a + b;
printf("Result: %lf\n", result);
break;
case 2:
result = a - b;
printf("Result: %lf\n", result);
break;
case 3:
result = a * b;
printf("Result: %lf\n", result);
break;
case 4:
if (b != 0) {
printf("Choose a case:\n");
printf("1. Quotient\n");
printf("2. Remainder\n");
scanf("%d", &caseChoice);
if (caseChoice == 1) {
result = a / b;
printf("Quotient: %lf\n", result);
} 
else if (caseChoice == 2) {
result = fmod(a, b);
printf("Remainder: %lf\n", result);
} 
else {
printf("Invalid case choice.\n");
}
} 
else {
printf("Error: Divisor is zero.\n");
}
break;
default:
printf("Invalid choice.\n");
}

return 0;
}
```

***

#### **Problem-15**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705349948300/4c6e5146-fb63-4f36-ab07-832650702a8a.png)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705349966808/8186155c-ebec-4a51-8c25-0a81e06119b8.png)

```c
#include <stdio.h>

int main() {
int player1Number, player2Guess, chances = 3, flag = 0;

printf("Player-1, enter a number: ");
scanf("%d", &player1Number);

printf("Player-2, you have 3 chances to guess the number.\n");

while (chances > 0) {
printf("Enter your guess: ");
scanf("%d", &player2Guess);

if (player2Guess == player1Number) {
printf("Right, Player-2 wins!\n");
flag = 1;
break;
} else {
chances--;
if (chances > 0) {
printf("Wrong, %d Chance(s) Left!\n", chances);
}
}
}

if (flag == 0) {
printf("Player-1 wins!\n");
}

return 0;
}
```
