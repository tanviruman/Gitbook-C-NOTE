# Summer-2023/ Set-B

{% embed url="https://drive.google.com/file/d/1Ln5G-MpZpbuA4CD4ATxqyyE-jQOKMRV4/view" %}

### Problem 1

```c
#include <stdio.h>

int is_palindrome(int n) {
    int rev = 0;
    for (int i = n; i; i /= 10)
        rev = rev*10 + i%10;
    return rev == n;
}

int fibonacci(int n) {
    if (n == 1) return 0;
    if (n == 2) return 1;
    return fibonacci(n-1) + fibonacci(n-2);
}

int is_fibonacci_palindrome(int n) {
    if (!is_palindrome(n)) return 0;
    for (int i = 1, f; ; i++) {
        f = fibonacci(i);
        if (n == f) return 1;
        if (f > n) return 0;
    }
}

void find_superhero_fibonacci_palindromes(int start, int end) {
    for (; start <= end; start++)
        if (is_fibonacci_palindrome(start))
            printf("%d\n", start);
}

int main() {
    int a, b; scanf("%d %d", &a, &b);
    find_superhero_fibonacci_palindromes(a, b);
}
```

### Problem 2

```c
#include <stdio.h>

struct demons {
    char name[60];
    int power;
};

int DivisibleBy_7(int n) {
    return (n % 7) ? 0 : 1;
}

int atleastOne(char *input) {
    for (; *input; input++) {
        if ((*input < 'a' || *input > 'z')
            && (*input < 'A' || *input > 'Z'))
            return 1;
    }
    return 0;
}

int main() {
    int n; scanf("%d", &n);
    struct demons ar[n];
    int count = 0;
    for (int i = 0; i < n; i++) {
        scanf(" %[^\n]", ar[i].name);
        scanf("%d", &ar[i].power);
        if (DivisibleBy_7(ar[i].power) ||
            atleastOne(ar[i].name))
            count++;
    }

    printf("%d\n", count);
}
```
