# 1-D array

_1-D array -Related Problems and Solutions_

#### **Problem-1**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955093784/6fd23dd5-1df1-43a9-83da-82b58102ff5b.png)

```c
#include <stdio.h>

int main() {
    int n, i;
    printf("Enter array size: ");
    scanf("%d", &n);
    int array[n];
    printf("Enter %d elements of the array:\n", n);

    for (int i = 0; i < n; i++) {
        scanf("%d", &array[i]);
    }

    printf("Array elements in reverse order:\n");

    for (i = n - 1; i >= 0; i--) {
        printf("%d ", array[i]);
    }

    return 0;
}
```

***

#### **Problem-2**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955104948/c3faa00d-3aad-4e2b-a7bb-814a6968255d.png)

```c
#include <stdio.h>

int main() {
    int n, sum = 0;

    // Input the number of integers
    printf("Enter the number of integers: ");
    scanf("%d", &n);

    // Declare an array of size n
    int array[n];

    // Input the integers into the array
    printf("Enter %d integers:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &array[i]);
        sum += array[i]; // Add the current integer to the sum
    }

    // Display the sum
    printf("Sum of the integers: %d\n", sum);

    return 0;
}
```

***

#### **Problem-3**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955124530/c605853a-2bcd-4eed-8025-e0374bddf4c0.png)

```c
#include <stdio.h>

int main() {
    int n, i;
    printf("Enter the size of the array: ");
    scanf("%d", &n);
    int array[n];
    printf("Enter %d integers:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &array[i]);
    }
    int sum = 0;
    for (i = 0; i < n; i++) {
        if (array[i] % 2 == 0) {
            sum += array[i];
        }
    }
    printf("Sum of even integers in the array: %d\n", sum);
    return 0;
}
```

***

#### **Problem-4**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955134759/d51e394d-8f94-44b4-9e8a-efab417fee58.png)

```c
#include <stdio.h>

int main() {
    int n, i;
    printf("Enter the size of the array: ");
    scanf("%d", &n);
    float arr[n];
    printf("Enter %d numbers: ", n);
    for (i = 0; i < n; i++) {
        scanf("%f", &arr[i]);
    }
    float sum = 0;
    for (i = 0; i < n; i++) {
        sum += arr[i];
    }
    float average = sum / n;
    printf("Average is: %.2f\n", average);
    return 0;
}
```

***

#### **Problem-5**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955147469/d76ca6d6-3e83-4992-a1d6-81d9f31f637b.png)

```c
#include <stdio.h>

int main() {
    int n, i;
    printf("Enter the size of the array: ");
    scanf("%d", &n);
    int array[n];
    printf("Enter %d integers:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &array[i]);
    }
    int sum = 0;
    for (i = 0; i < n; i++) {
        if (i % 2 == 0) {
            sum += array[i];
        }
    }
    printf("Sum of even integers of array: %d\n", sum);
    return 0;
}
```

***

#### **Problem-6**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955172840/cde30066-1b28-4dc3-aef2-a4e5055f738f.png)

```c
#include <stdio.h>

int main() {
    int n;
    printf("Enter the size of the array: ");
    scanf("%d", &n);
    int firstArray[n];
    int secondArray[n];
    int sumArray[n];

    printf("Enter %d elements for the first array:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &firstArray[i]);
    }

    printf("Enter %d elements for the second array:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &secondArray[i]);
    }

    for (int i = 0; i < n; i++) {
        sumArray[i] = firstArray[i] + secondArray[i];
    }

    printf("Sum of corresponding numbers:\n");
    for (int i = 0; i < n; i++) {
        printf("%d ", sumArray[i]);
    }

    return 0;
}
```

***

#### **Problem-7**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955182772/6bd0e2eb-58df-4a62-8c0f-17fed7340dbc.png)

```c
#include <stdio.h>

int main() {
    int n, i, temp;
    printf("Enter the size of the array: ");
    scanf("%d", &n);
    int arr[n];

    printf("Enter %d elements of the array: ", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Reversing the array
    for (i = 0; i < n / 2; i++) {
        temp = arr[i];
        arr[i] = arr[n - 1 - i];
        arr[n - 1 - i] = temp;
    }

    printf("Reversed array: ");
    for (i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");

    return 0;
}
```

***

#### **Problem-8**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955195766/8a72fa59-ac76-49a0-8294-2f5bb1e88021.png)

```c
#include <stdio.h>

int main() {
    int n, i;
    printf("Enter the size of the array: ");
    scanf("%d", &n);
    int array[n];

    printf("Enter the elements of the array: ");
    for (i = 0; i < n; i++) {
        scanf("%d", &array[i]);
    }

    int max = array[0], min = array[0], maxIndex = 0, minIndex = 0;

    for (i = 1; i < n; i++) {
        if (array[i] > max) {
            max = array[i];
            maxIndex = i;
        }
        if (array[i] < min) {
            min = array[i];
            minIndex = i;
        }
    }

    printf("Max: %d, Index: %d\n", max, maxIndex);
    printf("Min: %d, Index: %d\n", min, minIndex);

    return 0;
}
```

***

#### **Problem-9**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955206440/a7dab54e-23ce-463a-a6e0-cb71e1f0347e.png)

```c
#include <stdio.h>

int main() {
    int n, vowelCount = 0;
    printf("Enter the number of alphabets: ");
    scanf("%d", &n);
    char alphabets[n];

    printf("Enter %d alphabets:\n", n);
    for (int i = 0; i < n; i++) {
        scanf(" %c", &alphabets[i]);
    }

    for (int i = 0; i < n; i++) {
        char currentChar = alphabets[i];
        if (currentChar == 'A' || currentChar == 'E' || currentChar == 'I' ||
            currentChar == 'O' || currentChar == 'U' || currentChar == 'a' ||
            currentChar == 'e' || currentChar == 'i' || currentChar == 'o' || currentChar == 'U')
        {
            vowelCount++;
        }
    }

    printf("Number of vowels: %d\n", vowelCount);
    return 0;
}
```

***

#### **Problem-10**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955217513/ddb614e6-4b2b-4476-8466-bda46fa648e0.png)

```c
#include <stdio.h>

int main() {
    int n, i, searchKey, found = 0;
    printf("Enter the size of array: ");
    scanf("%d", &n);
    int array[n];

    printf("Enter the integers: ");
    for (i = 0; i < n; i++) {
        scanf("%d", &array[i]);
    }

    printf("Enter the number to search: ");
    scanf("%d", &searchKey);

    for (i = 0; i < n; i++) {
        if (array[i] == searchKey) {
            found = 1;
            break;  // Break the loop if the key is found
        }
    }

    if (found == 1) {
        printf("FOUND\n");
    } else {
        printf("NOT FOUND\n");
    }

    return 0;
}
```

***

#### **Problem-11**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955234096/54a3bdf1-0e87-4cd4-aa31-a69ce45e990d.png)

```c
#include <stdio.h>

int main() {
    int n, i;
    printf("Enter the size of array: ");
    scanf("%d", &n);
    int A[n], B[n];

    printf("Enter the elements for array A: ");
    for (i = 0; i < n; i++) {
        scanf("%d", &A[i]);
    }

    printf("Array A:");
    for (i = 0; i < n; i++) {
        printf(" %d", A[i]);
        B[n - i - 1] = A[i];
    }

    printf("\n");
    printf("Array B:");
    for (i = 0; i < n; i++) {
        printf(" %d", B[i]);
    }

    printf("\n");
    return 0;
}
```

***

#### **Problem-12**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955247615/9b1d1d93-9216-4bbc-ad45-adb34ed552f1.png)

```c
#include <stdio.h>

int main() {
    int n, position, number;
    printf("Enter the size of array: ");
    scanf("%d", &n);
    int array[n];

    printf("Enter %d integers:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &array[i]);
    }

    printf("Enter the number to insert: ");
    scanf("%d", &number);
    printf("Enter the position to insert: ");
    scanf("%d", &position);

    // Shifting the elements to the right
    for (int i = n - 1; i >= position; i--) {
        array[i + 1] = array[i];
    }

    // Inserting the number at the specified position
    array[position] = number;

    printf("Array after insertion:\n");
    for (int i = 0; i < n + 1; i++) {
        printf("%d ", array[i]);
    }

    return 0;
}
```

***

#### **Problem-13**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955261652/f4801965-e060-4a62-9dc1-c7e6a7b28991.png)

```c
#include <stdio.h>

int main() {
    int n, position, i;
    printf("Enter the size of array: ");
    scanf("%d", &n);
    int array[n];

    printf("Enter %d elements for the array:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &array[i]);
    }

    printf("Enter the position: ");
    scanf("%d", &position);

    if (position >= 0 && position < n) {
        for (i = position; i < n - 1; i++) {
            array[i] = array[i + 1];
        }
        n--;

        printf("Array after deletion:");
        for (i = 0; i < n; i++) {
            printf(" %d", array[i]);
        }
        printf("\n");
    } else {
        printf("Invalid position!\n");
    }

    return 0;
}
```

***

#### **Problem-14**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955274843/ecd4c641-b060-46b5-a040-c3d5a336b768.png)

```c
#include <stdio.h>

int main() {
    int n, m;

    // Input the size of arrays A and B
    printf("Enter the size of array A: ");
    scanf("%d", &n);
    printf("Enter the size of array B: ");
    scanf("%d", &m);

    // Check if the sizes are compatible for swapping
    if (n != m) {
        printf("Array sizes are not compatible for swapping.\n");
        return 1;
    }

    // Declare arrays A and B with the same size
    int A[n], B[n];

    // Input elements for array A
    printf("Enter %d integers for array A:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &A[i]);
    }

    // Input elements for array B
    printf("Enter %d integers for array B:\n", m);
    for (int i = 0; i < m; i++) {
        scanf("%d", &B[i]);
    }

    // Swap elements between arrays A and B
    for (int i = 0; i < n; i++) {
        int temp = A[i];
        A[i] = B[i];
        B[i] = temp;
    }

    // Display elements of both arrays
    printf("Array A after swapping:\n");
    for (int i = 0; i < n; i++) {
        printf("%d ", A[i]);
    }
    printf("\n");

    printf("Array B after swapping:\n");
    for (int i = 0; i < m; i++) {
        printf("%d ", B[i]);
    }
    printf("\n");

    return 0;
}
```

***

#### **Problem-15**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955292926/f975c057-acbb-402c-a120-87d57a5a261a.png)

```c
#include <stdio.h>

int main() {
    int n, i;

    // Input the size of the array
    printf("Enter the size of the array: ");
    scanf("%d", &n);

    // Declare an array with the given size
    int A[n];

    // Input elements for the array
    printf("Enter %d elements: ", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &A[i]);
    }

    // Replace elements that are divisible by 3 with -1
    for (i = 0; i < n; i++) {
        if (A[i] % 3 == 0) {
            A[i] = -1;
        }
    }

    // Display the array after replacement
    printf("Array A after replacing: ");
    for (i = 0; i < n; i++) {
        printf("%d ", A[i]);
    }
    printf("\n");

    return 0;
}
```

***

#### **Problem-16**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955310213/08e852fe-6e11-4a7d-be3d-8e43dd7802b3.png)

```c
#include <stdio.h>

int main() {
    int n, i;

    // Input the size of the array
    printf("Enter the size of the array: ");
    scanf("%d", &n);

    // Declare an array with the given size
    int A[n];

    // Input elements for the array
    printf("Enter %d elements: ", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &A[i]);
    }

    // Replace elements at odd indexes with 0
    for (i = 1; i < n; i += 2) {
        A[i] = 0;
    }

    // Display the array after replacement
    printf("Array A after replacing: ");
    for (i = 0; i < n; i++) {
        printf("%d ", A[i]);
    }
    printf("\n");

    return 0;
}
```

***

#### **Problem-17**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955330143/01a9af7f-673c-414c-bacd-ad2f060ac307.png)

```c
#include <stdio.h>

int main() {
    int n, i, j;

    // Input the size of the array
    printf("Enter the size of the array: ");
    scanf("%d", &n);

    // Declare an array with the given size
    int A[n];

    // Input elements for the array
    printf("Enter %d elements: ", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &A[i]);
    }

    // Bubble Sort
    for (i = 0; i < n - 1; i++) {
        for (j = 0; j < n - i - 1; j++) {
            if (A[j] > A[j + 1]) {
                // Swap elements if they are in the wrong order
                int temp = A[j];
                A[j] = A[j + 1];
                A[j + 1] = temp;
            }
        }
    }

    // Display the sorted array
    printf("Array A after sorting: ");
    for (i = 0; i < n; i++) {
        printf("%d ", A[i]);
    }
    printf("\n");

    return 0;
}
```

***

#### **Problem-18**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955372288/6dd541c1-2e9a-436d-ac67-19109d5c356e.png)

```c
#include <stdio.h>

int main() {
    int n, i, j;

    // Input the size of the array
    printf("Enter the size of the array: ");
    scanf("%d", &n);

    // Declare arrays for the input and unique elements
    int A[n], uniqueArray[n];

    // Input elements for the array
    printf("Enter the elements of the array: ");
    for (i = 0; i < n; i++) {
        scanf("%d", &A[i]);
    }

    // Remove duplicates
    int uniqueCount = 0;
    for (i = 0; i < n; i++) {
        int isDuplicate = 0;
        for (j = 0; j < uniqueCount; j++) {
            if (A[i] == uniqueArray[j]) {
                isDuplicate = 1;
                break;
            }
        }
        if (!isDuplicate) {
            uniqueArray[uniqueCount++] = A[i];
        }
    }

    // Display the array after removing duplicates
    printf("Array A after removing duplicates: ");
    for (i = 0; i < uniqueCount; i++) {
        printf("%d ", uniqueArray[i]);
    }
    printf("\n");

    return 0;
}
```

***

#### **Problem-19**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955387069/8db55a35-6a07-4801-96bb-486c93ed8153.png)

```c
#include <stdio.h>

int main() {
    int n, m, i, j;

    // Input size and elements for array A
    printf("Enter the size of array A: ");
    scanf("%d", &n);
    int A[n];
    printf("Enter the elements of array A: ");
    for (i = 0; i < n; i++) {
        scanf("%d", &A[i]);
    }

    // Input size and elements for array B
    printf("Enter the size of array B: ");
    scanf("%d", &m);
    int B[m];
    printf("Enter the elements of array B: ");
    for (i = 0; i < m; i++) {
        scanf("%d", &B[i]);
    }

    // Find and display the intersection
    int hasIntersection = 0;
    for (i = 0; i < n; i++) {
        for (j = 0; j < m; j++) {
            if (A[i] == B[j]) {
                printf("%d ", A[i]);
                hasIntersection = 1;
                break;
            }
        }
    }

    // Display "Empty set" if no intersection is found
    if (!hasIntersection) {
        printf("Empty set");
    }
    printf("\n");

    return 0;
}
```

***

#### **Problem-20**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955404479/ffeec27b-20ba-4c1d-8105-aa2d9664f000.png)

```c
#include <stdio.h>

int main() {
    int n, m, i, j;

    // Input size and elements for array A
    printf("Enter the size of array A: ");
    scanf("%d", &n);
    int A[n];
    printf("Enter %d elements for array A:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &A[i]);
    }

    // Input size and elements for array B
    printf("Enter the size of array B: ");
    scanf("%d", &m);
    int B[m];
    printf("Enter %d positive elements for array B:\n", m);
    for (i = 0; i < m; i++) {
        scanf("%d", &B[i]);
    }

    // Creating a temporary array C with size equal to the sum of sizes of A and B
    int C[n + m];

    // Copying elements of A to C
    for (i = 0; i < n; i++) {
        C[i] = A[i];
    }

    // Copying elements of B to C, excluding duplicates from A
    int unionSize = n; // Size of the union array
    for (i = 0; i < m; i++) {
        int found = 0; // Flag to check if the element is already present in A

        // Checking if the element is already present in A
        for (j = 0; j < n; j++) {
            if (B[i] == A[j]) {
                found = 1;
                break;
            }
        }

        // If the element is not found in A, add it to C
        if (!found) {
            C[unionSize] = B[i];
            unionSize++;
        }
    }

    // Display the union of arrays A and B
    printf("Union of array A and array B:\n");
    for (i = 0; i < unionSize; i++) {
        printf("%d ", C[i]);
    }

    return 0;
}
```

***

#### **Problem-21**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1718955416968/5f4fba9f-6107-4dd2-b1d3-ee8a89298628.png)

```c
#include <stdio.h>

int main() {
    int n, m, i, j;

    // Input size and elements for array A
    printf("Enter the size of array A: ");
    scanf("%d", &n);
    int A[n];
    printf("Enter %d integers for array A:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &A[i]);
    }

    // Input size and elements for array B
    printf("Enter the size of array B: ");
    scanf("%d", &m);
    int B[m];
    printf("Enter %d positive integers for array B:\n", m);
    for (i = 0; i < m; i++) {
        scanf("%d", &B[i]);
    }

    // Find the difference (A - B)
    int diffSize = 0;
    int diff[n]; // The difference array

    // Loop through elements of A
    for (i = 0; i < n; i++) {
        int found = 0; // Flag to check if the element is in B

        // Check if the element is in B
        for (j = 0; j < m; j++) {
            if (A[i] == B[j]) {
                found = 1;
                break;
            }
        }

        // If the element is not in B, add it to the difference array
        if (!found) {
            diff[diffSize] = A[i];
            diffSize++;
        }
    }

    // Display the difference array
    printf("Difference (A - B):\n");
    for (i = 0; i < diffSize; i++) {
        printf("%d ", diff[i]);
    }

    return 0;
}
```

***
