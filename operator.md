# Operator

_**Operator Related Practice Problems and solutions**_

#### **Problem-1**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705064892821/9597eb86-35d2-48d5-aa46-2b36bcc97a9a.png)

```c
#include<stdio.h>
int main()
{
    double A,B;

    printf("Enter two numbers:");
    scanf("%lf %lf",&A,&B);

    double addition= A+B;

    double subtraction = A-B;

    double multiplication=A*B;

    printf("Addition=%lf\nSubtraction=%lf\nMultiplication=%lf ",addition,subtraction,multiplication);
    
    /*printf("Addition: %lf\n", A + B);
    printf("Subtraction: %lf\n", A - B);
    printf("Multiplication: %lf\n", A * B);*/

    if (B != 0) {
        printf("Division - Quotient: %lf, Reminder: %lf\n", A / B, fmod(A, B));
    } else {
        printf("Division by zero is undefined.\n");
    }

    
    return 0;
    
}
```

***

#### **Problem-2**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705065006064/b688b9ed-24ca-44b5-b7a2-4b2a8c6a24dd.png)

```c
#include<stdio.h>
#define Pi 3.1416
int main()
{
    double A;
    double r;

    printf("Enter the radius of the circle:");
    scanf("%lf",&r);

    A=2*Pi*r;

    printf("Area:%lf",A);

    return 0;
}
```

***

#### **Problem-3**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705065083482/42074cf9-7654-4ba4-9f77-ecdcd9df1972.png)

```c
#include<stdio.h>
int main()
{
    double a,b;
    printf("Enter two numbers:");
    scanf("%lf %lf",&a,&b);

  double X=(3.31*a*a+2.01*b*b*b)/(7.16*b*b+2.01*a*a*a);
  printf("X=%lf",X);

   return 0 ;
}
```

***

#### **Problem-4**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705065173898/6552bb3d-6c2f-4922-93a5-13a28deaf8f2.png)

```c
#include<stdio.h>
int main()
{
    int X=5;

    printf("X++:%d\n",X++);
    X=5;
    printf("++X:%d\n",++X);
    X=5;
    printf("X--:%d\n",X--);
    X=5;
    printf("--X:%d\n",--X);
    return 0;
}
```

***

#### **Problem-5**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705065243005/30b38707-741f-411d-aeb1-b0b490fb50dd.png)

```c
#include<stdio.h>
int main()
{
    int X=5;
    int Y=10;

    X+=Y;
    printf("Incremented by Y=%d\n",X);

    X-=Y;
    printf("Decremented by Y=%d\n",X);
    return 0;
}
```

***

#### **Problem-6**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705065939044/a356e1a9-ad6a-46d3-b1d8-86099520b6dc.png)

```c
#include<stdio.h>
int main()
{
    int X=56;
    int Y=10;

    X*=Y;
    printf("Multiplication =%d\n",X);

    X=56;
    X/=Y;
    printf("Division =%d\n",X);
    return 0;
}
```

***

#### **Problem-7**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705066051615/83a99012-826f-40d7-b141-b2bcea238317.png)

```c
#include <stdio.h>

int main() {
   int numInt = -150;
   float numFloat = 123.125;

   // Floating to integer conversion using:

   // a) Assignment operation:
   int intFromFloatAssign = numFloat;  // Fractional part is discarded
   printf("Integer from float (assignment): %d\n", intFromFloatAssign);

   // b) Type casting:
   int intFromFloatCast = (int)numFloat;  // Explicit type conversion
   printf("Integer from float (type casting): %d\n", intFromFloatCast);

   // Integer to floating conversion using:

   // a) Assignment operation:
   float floatFromIntAssign = numInt;  // Integer is automatically converted to float
   printf("Float from integer (assignment): %f\n", floatFromIntAssign);

   // b) Type casting:
   float floatFromIntCast = (float)numInt;  // Explicit type conversion
   printf("Float from integer (type casting): %f\n", floatFromIntCast);

   return 0;
}
```

***

#### **Problem-8**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705066140006/bf78cf7b-5010-4727-8f1e-18630dcd4950.png)

```c
#include<stdio.h>
int main()
{
    int num1,num2,maxnum;

    printf("Enter two numbers:");
    scanf("%d %d",&num1,&num2);

    maxnum=(num1>num2)?num1:num2;

    printf("Maximum=%d\n",maxnum);

    return 0;
}
```

***

#### **Problem-9**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705066211711/2e2f25f8-a78c-4f20-a2d2-dba77055e7ee.png)

```c
#include <stdio.h>

int main()
 {
double a, b, c;

printf("Enter values for a, b, and c: ");
scanf("%lf %lf %lf", &a, &b, &c);

double X = a - b / 3.0 + c * 2 - 1;
double Y = a - (b / (3 + c) * 2) - 1;
double Z = a - ((b / 3) + c * 2) - 1;

printf("X: %lf\nY: %lf\nZ: %lf\n", X, Y, Z);

return 0;
}
```

***

#### **Problem-10**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705066267190/b621fc23-d7c0-45b8-a3c5-f72d78eadf84.png)

```c
#include <stdio.h>
int main()
{
double a, b, c;

printf("Enter values for a, b, and c: ");
scanf("%lf %lf %lf", &a, &b, &c);

int resultA=(a+b)<=80;
int resultB=!(a+c);
int resultC=a!=0;

printf("a)Result: %d\nb)Result: %d\nc)Result:%d\n", resultA,resultB, resultC);

return 0;
}
```

***

#### **Problem-11**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705066330186/851fa92a-071b-4d86-87a7-72162e609f2c.png)

```c
#include <stdio.h>

int main() {
int a, b, c;

printf("Enter values for a, b, and c: ");
scanf("%d %d %d", &a, &b, &c);

int resultA = ((a + b) <= 80) && (b >= 0);
int resultB = ((a - b) == 0) || (c != 0);
int resultC = (a != b) || ((b < a) && (c > 0));

printf("(a) Result: %d\n(b) Result: %d\n(c) Result: %d\n", resultA, resultB, resultC);

return 0;
}
```

***

#### **Problem-12**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705073446412/a7d64abd-4467-4cc7-974d-2d22b520a459.png)

```c
#include <stdio.h>
#include <math.h>

int main() {
double a, b, c;

printf("Enter values for a, b, and c: ");
scanf("%lf %lf %lf", &a, &b, &c);

double discriminant = b * b - 4 * a * c;

if (discriminant > 0) {
double root1 = (-b + sqrt(discriminant)) / (2 * a);
double root2 = (-b - sqrt(discriminant)) / (2 * a);
printf("Root 1: %lf\nRoot 2: %lf\n", root1, root2);
} else if (discriminant == 0) {
double root = -b / (2 * a);
printf("Root: %lf\n", root);
} else {
printf("Imaginary.\n");
}

return 0;
}
```

***

#### **Problem-13**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705073505721/f33e2aa8-17fc-42a9-b772-d5a4fcaf3012.png)

```c
#include <stdio.h>
#include <math.h>

int main() {
double x;

printf("Enter a value for x: ");
scanf("%lf", &x);
x = x * 3.1416 / 180;

double result = 2 * cos(x)*cos(x) - sqrt(3) * sin(x) + sin(x / 2);

printf("Result: %lf\n", result);

return 0;
}
```

***

#### **Problem-14**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705073572607/887b01e1-e32e-4636-b60f-e2a74a3f8c64.png)

```c
#include <stdio.h>

int main() {
double X;

printf("Enter a floating-point number X: ");
scanf("%lf", &X);

double A = ceil(X);
double B = floor(X);
double C = fabs(X);

printf("A (Rounded Up): %lf\nB (Rounded Down): %lf\nC (Absolute Value): %lf\n", A, B, C);

return 0;
}
```

***

#### **Problem-15**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1705073692603/b3e1c4cd-c66d-4523-8509-c08bce5805c9.png)

```c
#include <stdio.h>

int main() {
printf("Size of int: %lu bytes\n", sizeof(int));
printf("Size of float: %lu bytes\n", sizeof(float));
printf("Size of double: %lu bytes\n", sizeof(double));
printf("Size of char: %lu byte\n", sizeof(char));

return 0;
}
```

***
