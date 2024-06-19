# Summer-2023/ Set-A

{% embed url="https://drive.google.com/file/d/12iUFLpx8fuxX_29XuMLnj_gOCcdOwin3/view" %}

### Problem 1

```c
#include <stdio.h>

int is_prime(int n) {
    if (n <= 1) return 0;
    for (int i = 2; i <= n/2; i++)
        if (n % i == 0) return 0;
    return 1;
}

int reverse_number(int n, int r) {
    if (n < 10) return r*10 + n;
    return reverse_number(n/10, r*10 + n%10);
}

int is_palindromic_prime(int n) {
    return is_prime(n) && reverse_number(n, 0) == n;
}

void find_superhero_palindromic_primes(int start, int end) {
    for (; start <= end; start++)
        if (is_palindromic_prime(start))
            printf("%d\n", start);
}

int main() {
    int a, b; scanf("%d %d", &a, &b);
    find_superhero_palindromic_primes(a, b);
}
```

### Problem 2

```c
#include <stdio.h>

struct demons {
    char name[60];
    int power;
};

int Multiple_of_5(int n) {
    return (n % 5) ? 0 : 1;
}

int onlyAlphabet(char *input) {
    for (; *input; input++) {
        if ((*input < 'a' || *input > 'z')
            && (*input < 'A' || *input > 'Z'))
            return 0;
    }
    return 1;
}

int main() {
    int n; scanf("%d", &n);
    struct demons ar[n];
    int count = 0;
    for (int i = 0; i < n; i++) {
        scanf(" %[^\n]", ar[i].name);
        scanf("%d", &ar[i].power);
        if (Multiple_of_5(ar[i].power)
            && onlyAlphabet(ar[i].name))
            count++;
    }

    printf("%d\n", count);
}
```
