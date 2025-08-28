// 1:Sum of two numbers
#include <stdio.h>
int main() {
    int a, b;
    printf("Enter a: ");
    scanf("%d", &a);
    printf("Enter b: ");
    scanf("%d", &b);

    printf("Sum is %d\n", a + b);
    return 0;
}
// 2:Sum, difference, product, and quotient of two numbers
#include <stdio.h>
int main() {
    int a, b;
    printf("Enter a: ");
    scanf("%d", &a);
    printf("Enter b: ");
    scanf("%d", &b);

    printf("Sum is %d\n", a + b);
    printf("Difference is %d\n", a - b);
    printf("Product is %d\n", a * b);

    if (b != 0) {
        printf("Quotient is %d\n", a / b);
    } else {
        printf("Cannot divide by zero.\n");
    }

    return 0;
}
// 3:Area and perimeter of a rectangle
#include <stdio.h>
int main() {
    int l, b;
    printf("Enter length: ");
    scanf("%d", &l);
    printf("Enter breadth: ");
    scanf("%d", &b);

    printf("Perimeter is %d\n", 2 * (l + b));
    printf("Area is %d\n", l * b);

    return 0;
}
 // 4:Area and circumference of a circle
#include <stdio.h>
#define PI 3.14159

int main() {
    float r;
    printf("Enter radius: ");
    scanf("%f", &r);

    printf("Circumference is %.2f\n", 2 * PI * r);
    printf("Area is %.2f\n", PI * r * r);

    return 0;
}
// 5:Celsius to Fahrenheit conversion
#include <stdio.h>
int main() {
    float c;
    printf("Enter temperature in Celsius: ");
    scanf("%f", &c);

    printf("Temperature in Fahrenheit is %.2f\n", (c * 9 / 5) + 32);

    return 0;
}
// 6:Swap two numbers using a third variable
#include <stdio.h>
int main() {
    int a, b, temp;
    printf("Enter a: ");
    scanf("%d", &a);
    printf("Enter b: ");
    scanf("%d", &b);

    temp = a;
    a = b;
    b = temp;

    printf("After swapping: a = %d, b = %d\n", a, b);

    return 0;
}
// 7:Swap two numbers without using a third variable
#include <stdio.h>
int main() {
    int a, b;
    printf("Enter a: ");
    scanf("%d", &a);
    printf("Enter b: ");
    scanf("%d", &b);

    a = a + b;
    b = a - b;
    a = a - b;

    printf("After swapping: a = %d, b = %d\n", a, b);

    return 0;
}
// 8:Sum of first n natural numbers
#include <stdio.h>
int main() {
    int n, sum = 0;
    printf("Enter n: ");
    scanf("%d", &n);

    for (int i = 1; i <= n; i++) {
        sum += i;
    }

    printf("Sum of first %d natural numbers is: %d\n", n, sum);

    return 0;
}
// 9:Simple and compound interest
#include <stdio.h>
#include <math.h>

int main() {
    float p, r, t;
    printf("Enter principal (p): ");
    scanf("%f", &p);
    printf("Enter rate of interest (r): ");
    scanf("%f", &r);
    printf("Enter time (t in years): ");
    scanf("%f", &t);

    float simple_interest = (p * r * t) / 100;
    float compound_amount = p * pow((1 + r / 100), t);
    float compound_interest = compound_amount - p;

    printf("Simple Interest: %.2f\n", simple_interest);
    printf("Compound Interest: %.2f\n", compound_interest);

    return 0;
}
// 10:Online C compiler to run C program online
#include <stdio.h>

int main() {
    int total_seconds, h, m, s;  // total_seconds = input seconds
    printf("Enter total seconds: ");
    scanf("%d", &total_seconds);

    h = total_seconds / 3600;
    m = (total_seconds % 3600) / 60;
    s = total_seconds % 60;

    printf("Time = %02d:%02d:%02d\n", h, m, s);

    return 0;
}
