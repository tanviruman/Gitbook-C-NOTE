# Nested for loop

_Nested For Loop-Related Problems and Solutions_

#### **Problem-1**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073636617/10e4fd89-3660-472d-a4f4-5d5da3646c10.png)

```c
#include <stdio.h>
int main() {
int n;
printf("Enter N: ");
scanf("%d", &n);
for (int row = 1; row <= n; row++) {
for (int col = 1; col <= n; col++) {
printf("%d", col);
}
printf("\n");
}

return 0;
}
```

***

#### Problem-2

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073652999/c7cf9ba1-00a7-4209-9c1d-d6762ae220e0.png)

```c
#include <stdio.h>
int main() {
int n;
printf("Enter N: ");
scanf("%d", &n);

for (int row = 1; row <= n; row++) {
for (int col = row; col < row + n; col++) {
printf("%d", col);
}
printf("\n");
}

return 0;
}
```

***

#### **Problem-3**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073663740/cb4d8bd0-3314-4fd3-a084-9bf59da1a46b.png)

```c
#include<stdio.h>
int main(){
int n,row,col,number;
printf("Enter N: ");
scanf("%d",&n);

for(row=1;row<=n;row++){
number=row;

for(col=0;col<row;col++){
printf("%d", number++);
}
printf("\n");
}
return 0;
}
```

***

#### **Problem-4**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073673458/242de6d2-46de-4f5e-a81f-f04688e672ab.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row = 1; row <= n; row++) {

        for (int bspace = 1; bspace <= n - row; bspace++) {
            printf("_");
        }


        for (int col = 1; col <= row; col++) {
            printf("%d", row);
        }

        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-5**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073686643/57eb4017-f10a-4425-a9e6-b6250a6c90f3.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row= 1; row<= n; row++) {
        for (int col = n; col >= n - row+ 1; col--) {
            printf("%d", col);
        }
        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-6**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073697452/49fe3c9e-add0-46ea-8b58-e6586ee994e6.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row= 1;row<= n; row++) {
        for (int col = 1; col <= row; col++) {
            printf("%d", col);
        }
        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-7**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073709130/1862ec1a-a34c-4cc0-b885-bcf50f10a661.png)

```c
#include <stdio.h>

int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row= 1;row<= n; row++) {
        for (int col = 1; col <= n; col++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-8**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073717154/f1862b75-fd7d-43b5-8807-727dab7f9ca5.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row = n; row >= 1; row--) {
        for (int col = 1; col <= row; col++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-9**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073732473/a3196516-b668-4f83-9984-3d4f2008e663.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row = 1; row <= n; row++) {
        for (int col = 1; col <= n; col++) {
            if ((row + col) % 2 == 0) {
                printf("1");
            } else {
                printf("0");
            }
        }
        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-10**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073742675/226af148-381e-464d-bb74-dab4e940978f.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row = 1; row <= n; row++) {
        for (int sp = 1; sp <= n - row; sp++) {
            printf("_");
        }
        for (int st = 1; st <= row; st++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-11**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073764583/6eb1ca41-7be8-4c5d-bd65-a92dcad9d63d.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row = 1; row <= n; row++) {
        for (int sp = 1; sp <= n - row; sp++) {
            printf("_");
        }
        for (int st = 1; st <= row * 2 - 1; st++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-12**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073780155/095a75c2-6610-4551-90d1-d6e8c124e7e4.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    if (n % 2 == 0) {
        printf("Enter an odd integer");
        return 1;
    }

    int mid = n / 2;

    for (int i = 0; i < n; i++) {
        int st, sp;
        if (i <= mid) {
            st = i * 2 + 1;
            sp = mid - i;
        } else {
            st = (n - i) * 2 - 1;
            sp = i - mid;
        }
        for (int j = 0; j < sp; j++) {
            printf("_");
        }

        for (int j = 0; j < st; j++) {
            printf("*");
        }

        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-13**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073791672/783fe283-0866-4bf7-b23b-1a22df9eaca7.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row = 1; row <= n; row++) {
        for (int col = 1; col <= row; col++) {
            printf("%d", col);
        }

        for (int col = 1; col < 2*(n - row); col++) {
            printf("_");
        }

        if (row == n)
        {
            for (int col = row - 1; col >= 1; col--) {
                printf("%d", col);
            }
        }
        else
        {
            for (int col = row; col >= 1; col--) {
                printf("%d", col);
            }
        }

        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-14**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073806306/4730ecc5-86d5-4dc5-9a19-3160c4327764.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row = 1; row <= n; row++) {
        if (row % 2 == 1) {
            for (int col = 1; col <= n; col++) {
                printf("*");
            }
        } else {
            printf("*");
            for (int col = 2; col < n; col++) {
                printf("_");
            }
            printf("*");
        }

        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-15**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073820153/3a005ca3-b72f-4116-b185-449cd6353831.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row = 1; row <= n; row++) {
        for (int col = 1; col <= n; col++) {
            if (row == 1 || row == n ||  col == n - row + 1) {
                printf("Z");
            } else {
                printf(" ");
            }
        }
        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-16**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073833983/ef5ae820-b366-434b-b9df-41005d024b79.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row = 1; row <= n; row++) {
        for (int col = 1; col <= n; col++) {
            if (row == col || row + col == n + 1) {
                printf("*");
            } else {
                printf("_");
            }
        }
        printf("\n");
    }

    return 0;
}
```

***

#### **Problem-17**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073847081/3a20423d-567e-4d04-a1f2-e775721d509f.png)

```c
#include <stdio.h>
#include <stdlib.h>
#include <math.h>
int main()
{
    int n;
    printf("Enter an odd integer: ");
    scanf("%d", &n);

    int mid = n / 2;
    for (int row = 0; row < n; row++)
    {
        for (int col = 0; col < n; col++)
        {
            if ( row >= mid)
            {
                if (row == mid || col == mid)
                {
                    printf("$");
                }
                else if (abs(row - col) == mid || row + col == n - 1 + mid)
                {
                    printf("$");
                }
                else
                {
                    printf("_");
                }
            }
            else
            {
                if (row == mid || col == mid)
                {
                    printf("$");
                }
                else if (abs(row - col) == mid || row + col == mid)
                {
                    printf("$");
                }
                else
                {
                        printf("_");
                }
            }
        }
        printf("\n");
    }
    return 0;
}
```

***

#### **Problem-18**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1719073857346/fbe755c3-1fbd-41ee-a534-5092089fe179.png)

```c
#include <stdio.h>
int main() {
    int n;
    printf("Enter N: ");
    scanf("%d", &n);

    for (int row = 0; row < n; row++) {
        for (int col = 0; col < n; col++) {
            if (row == n / 2 || col == 0 || col == n-1) {
                printf("H ");
            } else {
                printf("  ");
            }
        }
        printf("\n");
    }

    return 0;
}
```

***
