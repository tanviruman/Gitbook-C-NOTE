# Loop

_Loop-Related Problems and Solutions_

#### **Problem-1**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717866119221/b6af24ca-51f5-46f7-ae3c-bbd3870d9261.png)

```c
#include<stdio.h>
int main(){
int number;
printf("Enter :");
scanf("%d",&number);

for(int i=1;i<=number;i++)
{
    printf("%d",i);

    if(i!=number){

        printf(",");

}
}
return 0;

}
```

***

#### **Problem-2**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717866189458/f60ab56e-a3ba-486a-9017-5341d73421c3.png)

```c
#include<stdio.h>
int main(){
int number,odd=1;
printf("Enter :");
scanf("%d",&number);

for(int i=1;i<=number;i++)
{

    printf("%d",odd);

    odd+=2;
    if(i!=number){

        printf(",");

}
}
return 0;
}
```

***

#### **Problem-3**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717867485764/8e591e13-f996-4d72-bca4-af0a9c14857f.png)

```c

#include<stdio.h>
int main(){
int number;
printf("Enter :");
scanf("%d",&number);

for(int i=1;i<=number;i++)
{
    if(i%2==1)

        printf("1");

    else

        printf("0");

    if(i!=number)

        printf(",");

}
return 0;
}
```

***

#### **Problem-4**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717867503413/753224e9-3361-45b3-a2c8-d5c4a7445007.png)

```c
#include <stdio.h>
int main()
{
int n, i;
float input, sum = 0, average;
printf("How many numbers you wish to average : ");
scanf("%d", &n);
printf("Enter %d numbers:\n", n);
for (i = 1; i <= n; i++)
{
scanf("%f", &input);
sum += input;
}
average = sum / n;
printf("AVG of %d inputs: %f\n",n, average);
return 0;
}
```

***

#### **Problem-5**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717867519121/644f74fc-423c-4564-b990-2afd346fff34.png)

```c
#include<stdio.h>
int main()
{
int X, Y;
printf("Enter the value of X: ");
scanf("%d", &X);
printf("Enter the value of Y: ");
scanf("%d", &Y);

while (X != Y) {
printf("%d", X * X);

if (X < Y) {
X++;
printf(", ");
}

else {
X--;
printf(", ");
}
}

printf("Reached!\n");
return 0;

}
```

***

#### **Problem-6**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717867542304/4f453109-a648-48eb-994a-600de0c11d89.png)

```c
#include <stdio.h>

int main() {
int X, N, Guess, Tries_left;
printf("Enter the number given by Player-1: ");
scanf("%d", &X);
printf("Enter the number of tries given for Player-2: ");
scanf("%d", &N);
Tries_left = N;

while (Tries_left > 0) {
printf("Enter your Guess: ");
scanf("%d", &Guess);

if (Guess == X) {
printf("Right, Player-2 wins!\n");
break;
} else {
Tries_left--;
printf("Wrong, %d Choice(s) Left!\n", Tries_left);
}
}

if (Tries_left == 0) {
printf("Player-1 wins!\n");
}

return 0;
}
```

***

#### **Problem-7**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717867557203/e3733871-0870-4488-a4f9-5bf89168bbd3.png)

```c
#include <stdio.h>
int main() {
char input;
int i = 1;
printf("Enter  inputs:");

while (1) {
scanf(" %c", &input);

if (input == 'A') {
break;
}

printf("Input %d: %c\n", i, input);
i++;
}

return 0;
}
```

***

#### **Problem-8**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717867568429/55b2a358-78a0-4672-9135-2ac145158e56.png)

```c
#include <stdio.h>
int main() {
int number, reverse = 0;
printf("Enter the Number: ");
scanf("%d", &number);

while (number != 0) {
int digit = number % 10;
reverse = reverse * 10 + digit;
number = number /10;
}

printf("Reverse: %d\n", reverse);
return 0;
}
```

***

#### **Problem-9**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717867579334/8cd84d94-df31-48d1-bc8c-20557dacc483.png)

```c
#include <stdio.h>
int main() {
int N;
printf("Enter the number of  Students: ");
scanf("%d", &N);

for ( int i = 1; i <= N; i++) {
float attendance, assignment, classtest, midterm, Final;
float total;

printf("Enter the marks of  Student %d (Attendance, Assignment, Class Test, Midterm,  Final): ", i);
scanf("%f%f%f%f%f", &attendance, &assignment, &classtest, &midterm, &Final);

total = attendance + assignment + classtest + midterm * 0.6 + Final * 0.4;
printf("Total marks:%f\n", total);

if (total >= 90) {
printf("Grade of Student %d : A\n", i);
}
else if (total >= 86) {
printf("Grade of Student %d : A-\n", i);
}
else if (total >= 82) {
printf("Grade of Student %d : B+\n", i);
}
else if (total >= 78) {
printf("Grade of Student %d : B\n", i);
} else if (total >= 74) {
printf("Grade of Student %d : B-\n", i);
} else if (total >= 70) {
printf("Grade of Student %d : C+\n", i);
} else if (total >= 66) {
printf("Grade of Student %d : C\n", i);
} else if (total >= 62) {
printf("Grade of Student %d : C-\n", i);
} else if (total >= 58) {
printf("Grade of Student %d : D+\n", i);
} else if (total >= 55) {
printf("Grade of Student %d : D\n", i);
} else {
printf("Grade of Student %d : F\n", i);
}
}

return 0;
}
```

***

#### **Problem-10**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717867592725/6d1f4d7c-7a8d-4639-9750-1d94722683cb.png)

```c
#include <stdio.h>

int main() {
int N, i, number;
int sum = 0;
printf("Enter the value of N: ");
scanf("%d", &N);

for (i = 1; i <= N; i++) {
if (i % 2 == 0) {
number = -i;
printf("%d,",number);
}
else {
number = i;
printf("%d,",number);
}

sum += number;

/*if(i!=number){
printf(",");}*/
}

printf("\nRESULT OF FIRST %dth TERMS: %d\n", N, sum);
return 0;
}
```

***

#### **Problem-11**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717996894583/17cd15be-1e71-4dfd-bcbe-a72f811e7557.png)

```c
#include <stdio.h>
int main()
{
int N, i, result = 0, number = 0;
printf("Enter the value of N: ");
scanf("%d", &N);

for (i = 1; i <= N; i++) {
int num=(i + 1);
number = i * i * num ;
printf("%d^2.%d + ",i,num);
result += number;
}

printf("Result of first %d terms: %d\n", N, result);
return 0;
}
```

***

#### **Problem-12**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717996909020/44080dbe-3b84-4e09-9703-fc87fc5805bb.png)

```c
#include <stdio.h>
int main() {
int N, i;
printf("Enter the value of N: ");
scanf("%d", &N);
int firstnumber = 1, secondnumber = 1;
printf("Fibonacci series : %d, %d", N, firstnumber, secondnumber);
for (i = 3; i <= N; i++) {
int nextnumber = firstnumber + secondnumber;
printf(", %d", nextnumber);
firstnumber = secondnumber;
secondnumber = nextnumber;
}

return 0;
}
```

***

#### **Problem-13**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717996928233/c64db115-8e2e-45e0-8e1f-326e0ee1ed02.png)

```c
#include <stdio.h>
int main() {
int N, i, factorial = 1;
printf("Enter a number: ");
scanf("%d", &N);
printf("%d! = ", N);

for (i = N; i >= 1; i--) {
printf("%d", i);
factorial *= i;

if (i != 1) {
printf(" X ");
}
}

printf(" = %d\n", factorial);
return 0;
}
```

***

#### **Problem-14**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717996939995/24ac8f96-6a8b-44ca-9bf2-100d103ff753.png)

```c
#include <stdio.h>
int main() {
int n, r, numerator = 1, denominator_r = 1, denominator_nr = 1;
float result;

printf("Enter the value of n: ");
scanf("%d", &n);
printf("Enter the value of r: ");
scanf("%d", &r);

for (int i = 1; i <= n; i++) {
numerator *= i;
}

for (int i = 1; i <= r; i++) {
denominator_r *= i;
}

for (int i = 1; i <= (n - r); i++) {
denominator_nr *= i;
}

result = numerator / (denominator_r * denominator_nr);
printf("%0.1f\n", result);

return 0;
}
```

***

#### **Problem-15**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717996953745/342d9c0c-1ed2-44db-9e44-367861e41e11.png)

```c
#include <stdio.h>
int main() {
int x, y;
printf("Enter the value of x: ");
scanf("%d", &x);
printf("Enter the value of y: ");
scanf("%d", &y);
int result = 1;
for (int i = 1; i <= y; i++) {
result=result*x;
}
printf("answer:%d\n", result);
return 0;
}
```

***

#### **Problem-16**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717996980702/cb80a91f-2097-4913-b034-e3600eaccfbd.png)

```c
#include <stdio.h>
int main() {
int num1, num2;
int newNUM1,newNUM2;
int GCD, LCM;

printf("Enter the first number: ");
scanf("%d", &num1);
printf("Enter the second number: ");
scanf("%d", &num2);

newNUM1 = num1;
newNUM2 = num2;

while (num2 != 0) {
int temp = num2;
num2 = num1 % num2;
num1 = temp;
}
GCD = num1;

LCM = (newNUM1 *newNUM2) / GCD;

printf("GCD of %d and %d is: %d\n", newNUM1,newNUM2, GCD);
printf("LCM of %d and %d is: %d\n", newNUM1,newNUM2, LCM);

return 0;
}
```

***

#### **Problem-17**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717996993873/ace50509-56f2-48a5-923f-5c71acb74e5a.png)

```c
#include <stdio.h>
int main() {
int number;
int prime = 1;

printf("Enter a number: ");
scanf("%d", &number);

if (number <= 1) {
prime = 0;
}
else {
for (int i = 2; i * i <= number; i++) {

if (number % i == 0) {
prime = 0;
break;
}
}
}

if (prime == 1) {
printf("%d is a prime number.\n", number);
}
else {
printf("%d is not a prime number.\n", number);
}

return 0;
}
```

***

#### **Problem-18**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717997008900/ac1690ed-a8d4-42f3-910f-8f01a90b5cf0.png)

```c
#include <stdio.h>

int main() {
int num, newnum, remainder, reverse = 0;

printf("Enter an integer: ");
scanf("%d", &num);
newnum = num;

while (num != 0) {
remainder = num % 10;
reverse = reverse * 10 + remainder;
num = num/10;
}

if (newnum == reverse) {
printf("Palindrome");
}
else {
printf("Not palindrome");
}

return 0;
}
```

***

#### **Problem-19**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717997023333/e90d2f2a-0155-4406-a65b-1b2bbde8610d.png)

```c
#include <stdio.h>
#include <math.h>

int main() {
double x, result = 0;
int n, sign = 1;

printf("Enter the value of x in radians: ");
scanf("%lf", &x);

printf("Enter the number of terms in the series: ");
scanf("%d", &n);

for (int i = 1; i <= n; i += 2) {
double term = pow(x, i) / tgamma(i + 1);
result += sign * term;
sign *= -1;
}

printf("sin(%lf) = %lf\n", x, result);

return 0;
}
```

***

#### **Problem-20**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1717997035593/e447d4f3-3844-4df6-8778-73d7bdc54fe0.png)

```c
#include <stdio.h>
int main() {
int n, num = 0,sum = 0;

printf("Enter the number of terms: ");
scanf("%d", &n);

for (int i = 1; i <= n; i++) {
num = num * 10 + i;
printf("%d+",num);
sum += num;
}

printf("\nSum of the series up to %d terms: %d\n", n, sum);
return 0;
}
```

***
