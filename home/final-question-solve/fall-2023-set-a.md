# Fall-2023/ Set-A

{% embed url="https://drive.google.com/file/d/1pxm7MT0GHhI0K67dRCp-Vdxcp2iKBeLD/view" %}

### Problem 1

```c
#include <stdio.h>
#include <string.h>

const char *numbers[10] = {
    "zero ", "one ", "two ", "three ", "four ", "five ", "six ", "seven ", "eight ", "nine"
};

int rev(int n) {
    int r = 0;
    for (; n; n /= 10)
        r = r*10 + n%10;
    return r;
}

void toSpelledOut(int n, char *str) {
    if (n == 0) return;

    strcat(str, numbers[n % 10]);
    toSpelledOut(n / 10, str);
}

void upperCase(char *num) {
    for (; *num; num++)
        if (*num >= 'a' && *num <= 'z')
            *num -= ' ';
}

int main() {
    int n; scanf("%d", &n);
    puts("For uppercase press 1");
    puts("For lowercase press 2");
    int c; scanf("%d", &c);
    char s[100] = {0};
    toSpelledOut(rev(n), s);
    if (c == 1) upperCase(s);
    puts(s);
}
```

### Problem 2

```c
#include <stdio.h>

int is_even_sum_greater(int n, int evenSum, int oddSum) {
    int d = n%10;
    if (d % 2) oddSum += d;
    else       evenSum += d;
    if (n < 10)
        return evenSum > oddSum;
    return is_even_sum_greater(n/10, evenSum, oddSum);
}

int prime_checker(int n) {
    if (n <= 1) return 0;
    for (int i = 2; i <= n/2; i++)
        if (n % i == 0) return 0;
    return 1;
}

int even_powered_number(int n) {
    return is_even_sum_greater(n, 0, 0) && prime_checker(n);
}

void find_even_powered_prime_number (int start, int end) {
    for (; start <= end; start++)
        if (even_powered_number(start))
            printf("%d\n", start);
}

int main() {
    int a, b; scanf("%d %d", &a, &b);
    find_even_powered_prime_number(a, b);
}
```
