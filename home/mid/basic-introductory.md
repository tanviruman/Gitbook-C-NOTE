# Basic Introductory

_**Basic Introductory Practice problems and solutions**_

#### Problem-1

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704815437531/3f9e7f10-482e-4298-bbc5-764064c425dc.png)

```c
#include<stdio.h>

int main ()
{
    printf("Hello World\n");

    return 0 ;
}
```

***

#### Problem-2

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704815597810/d99d386c-219e-4d6b-8ef2-8003f5cb2fc2.png)

```c
#include<stdio.h>

int main ()
{
    printf("Hello World.\nThis is my first program.\tC is fun.\n");

    return 0 ;
}
```

***

#### Problem-3

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704817753585/130c180f-2fea-4b13-ba04-f2fec81f39e3.png)

```c
#include<stdio.h>
int main()
{
    printf("The question is-\"How to write a \n\\comment\/ in C progrannig language?\"\n");
    return 0 ;
}
```

***

#### Problem-4

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704817921583/aa43c130-1d3f-4899-9fd6-2891ea778d13.png)

```c
#include<stdio.h>
int main()
{
    int integerVar;
    float floatVar;
    char charVar;

    integerVar=5 ;
    floatVar=3.141593;
    charVar='a';

    printf("The inetger value:%d\n",integerVar);
    printf("The floating point value:%f\n",floatVar);
    printf("The Character value:%c\n",charVar);
    return 0 ;
}
```

***

#### Problem-5

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704818103924/a4a9bb64-2b06-4eac-84e5-898053ceb8a0.png)

```c
#include<stdio.h>
int main()
{
//Declare a variable uninitialized
 int uninitializedVar;

 //Declare and  initialize a variable in one statement
 int initializedVar=65;

 //Declare and initialize multiple variables with different values in one statement
 int Var1=65,Var2=75,Var3=85,Var4=95;

//Declare and initialize multiple variables with the same value in one statement
int sameVar1=20,sameVar2=20,sameVar3=20,sameVar4=20;

printf("a)Uninitialized variable:%d\n",uninitializedVar);

printf("b)Initialize  variable:%d\n",initializedVar);

printf("c)multiple variables with different values:%d, %d, %d, %d\n",Var1,Var2,Var3,Var4);

printf("d)multiple variables with same value:%d, %d, %d, %d\n",sameVar1,sameVar2,sameVar3,sameVar4);

return 0 ;

}
```

***

#### Problem-6

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704818235342/b45ba287-9b33-4919-8437-178cc71d9c29.png)

```c
#include<stdio.h>
int main()
{
  int age;

  printf("Enter age:");

  scanf("%d",&age);

  printf("My age is :%d\n",age);

  return 0;



}
```

***

#### Problem-7

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704818407539/31418607-7186-4185-85a3-4f9ff9b1a692.png)

```c
#include<stdio.h>
int main()
{
    int integerVar;
    float floatVar;
    char charVar;

    printf("Enter an Integer:");
    scanf("%d",&integerVar);

    printf("Enter a floating point value :");
    scanf("%f",&floatVar);

//Clear the newline character left in the input buffer
while(getchar()!='\n');

    printf("Enter a Character :");
    scanf("%c",&charVar);

    printf("The integer value:%d\n",integerVar);
    printf("The floating point value:%f\n",floatVar);
    printf("The character value:%c\n",charVar);

    return 0;
}
```

***

#### Problem-8

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704818993664/684fd5a7-229b-44eb-9167-735c32d11f1c.png)

```c
#include<stdio.h>
int main()
{

    int firstValue,lastValue;
    int middleValue;

    printf("Enter three integer value:");

    scanf("%d %*d %d",&firstValue,&lastValue);

    printf("First Value = %d ,Last Value = %d\n",firstValue,lastValue);

    return 0;

}
```

***

#### Problem-9

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704819227974/b7090f01-bbbd-46c0-9b24-69e922ec4e03.png)

```c
#include<stdio.h>
int main()
{
    double doubleVar=3.14159;
    int booleanVar= 1;

    printf("The double value:%lf\n",doubleVar);
    printf("The boolean value:%s\n",booleanVar? "true":"false");

    return 0;


}
```

***

#### Problem-10

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704819432459/87f3e50c-baa7-41d2-94fe-c5f3e483ec30.png)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704820430807/b6c15106-7385-42fb-ac60-72bd72f9986c.png)

```c
#include <stdio.h>

int main() {
    long int longIntVariable = 1234567890L;         // A long int variable
    long long int longLongIntVariable = 1234567890123456789LL; // A long long int variable
    long double longDoubleVariable = 3.141592653589793238L;  // A long double variable
    short int shortIntVariable = 32767;              // A short int variable

    // Printing the values
    printf("The Long Int Value: %ld\n", longIntVariable);
    printf("The Long Long Int Value: %lld\n", longLongIntVariable);
    printf("The Long Double Value: %Lf\n", longDoubleVariable);
    printf("The Short Int Value: %d\n", shortIntVariable);

    return 0;
}
```

***

#### Problem-11

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704820522056/7f20e7a6-5258-4ba1-b980-c9f6aae7daa2.png)

```c
#include <stdio.h>

int main() {
    unsigned int unsignedIntVariable = 4294967295U;                     // An unsigned int variable
    unsigned long int unsignedLongIntVariable = 18446744073709551615UL; // An unsigned long int variable
    unsigned long long int unsignedLongLongIntVariable = 18446744073709551615ULL; // An unsigned long long int variable
    unsigned short int unsignedShortIntVariable = 65535U;               // An unsigned short int variable

    // Printing the values
    printf("Unsigned Int Value: %u\n", unsignedIntVariable);
    printf("Unsigned Long Int Value: %lu\n", unsignedLongIntVariable);
    printf("Unsigned Long Long Int Value: %llu\n", unsignedLongLongIntVariable);
    printf("Unsigned Short Int Value: %u\n", unsignedShortIntVariable);

    return 0;
}
```

***

#### Problem-12

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704820787489/a1bd4cdc-f75d-427c-967a-040602c1586e.png)

```c
#include<stdio.h>
int main()
{
    const float pi=3.1416;

    printf("The value of pi:%.4f\n",pi);

    return 0;

}
```

***

#### Problem-13

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704821120472/d9e474f6-7c1b-4ce6-91d4-9bea9b32b29c.png)

```c
#include<stdio.h>
int main()
#define HEIGHT 100
{


    printf("The value of HEIGHT:%d\n",HEIGHT);

    return 0;

}
```

***

#### Problem-14

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704821350403/ee04ad06-8d6b-442e-b649-fd7d81bea720.png)

```c
#include <stdio.h>

int globalVariable = 10; // Define a global variable

int main() {
    printf("A. Value of globalVariable before defining the local variable: %d\n", globalVariable);

    int globalVariable = 20; // Define a local variable with the same name

    printf("B. Value of globalVariable after defining the local variable: %d\n", globalVariable);

    {
        extern int globalVariable;
        printf("C. Value of globalVariable as global: %d\n", globalVariable);
    }

    return 0;
}
```

***

#### Problem-15

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1704821535652/176bb277-abbc-4247-9030-463a277b40ac.png)

```c
#include <stdio.h>

int main() {
    float floatValue;

    // Prompt the user for input
    printf("Please enter a floating-point number: ");

    // Read the floating-point number from the user
    scanf("%f", &floatValue);

    // (a) Print the number right-justified within 10 columns
    printf("(a) Right-justified within 10 columns: %10.6f\n", floatValue);

    // (b) Print the number right-justified to 2 columns
    printf("(b) Right-justified to 2 columns: %2.6f\n", floatValue);

    // (c) Print the number rounded to two decimal places
    printf("(c) Rounded to two decimal places: %.2f\n", floatValue);

    // (d) Print the number rounded to an integer (without conversion or type casting)
    printf("(d) Rounded to integer: %.0f\n", floatValue);

    // (e) Print the number in exponential notation (scientific notation)
    printf("(e) Exponential notation: %e\n", floatValue);

    return 0;
}
```

***
