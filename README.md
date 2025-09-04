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
#include <stdio.h>

int main() {
    int n;
    printf("Enter a number: ");
    scanf("%d", &n);

    if(n % 2 == 0) {
        printf("Even number\n");
    } else {
        printf("Odd number\n");
    }

    return 0;
}
// 11: Even or Odd
#include <stdio.h>

int main() {
    int n;
    printf("Enter a number: ");
    scanf("%d", &n);

    if(n >= 0) {
        if(n == 0) {
            printf("Number is 0\n");
        } else {
            printf("Positive number\n");
        }
    } else {
        printf("Negative number\n");
    }

    return 0;
}
// 12: Positive, Negative, or Zero
#include <stdio.h>

int main() {
    int year;
    printf("Enter year: ");
    scanf("%d", &year);

    if((year % 4 == 0 && year % 100 != 0) || year % 400 == 0) {
        printf("It is a leap year\n");
    } else {
        printf("It is not a leap year\n");
    }
    return 0;
}
// 13: Leap Year Check 
#include <stdio.h>

int main() {
    char ch;
    printf("Enter a character: ");
    scanf(" %c", &ch);  // Space before %c to consume any newline

    if(ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' ||
       ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') {
        printf("It is a vowel\n");
    } else {
        printf("It is a consonant\n");
    }

    return 0;
}
// 14: Vowel or Consonant
#include <stdio.h>

int main() {
    char ch;
    printf("Enter a character: ");
    scanf(" %c", &ch);  // Space before %c

    if(ch >= 'a' && ch <= 'z') {
        printf("Lowercase alphabet\n");
    } else if(ch >= 'A' && ch <= 'Z') {
        printf("Uppercase alphabet\n");
    } else if(ch >= '0' && ch <= '9') {
        printf("It is a digit\n");
    } else {
        printf("It is a special character\n");
    }

    return 0;
}
// 15: Character Type
#include <stdio.h>

int main() {
    int a, b, c;
    printf("Enter a: ");
    scanf("%d", &a);
    printf("Enter b: ");
    scanf("%d", &b);
    printf("Enter c: ");
    scanf("%d", &c);

    if(a > b && a > c) {
        printf("a is greatest\n");
    } else if(b > a && b > c) {
        printf("b is greatest\n");
    } else {
        printf("c is greatest\n");
    }

    return 0;
}
// 16: Largest of Three Numbers
#include <stdio.h>
#include <math.h>

int main() {
    float a, b, c, d, root1, root2;
    printf("Enter coefficient of x^2: ");
    scanf("%f", &a);
    printf("Enter coefficient of x: ");
    scanf("%f", &b);
    printf("Enter constant: ");
    scanf("%f", &c);

    d = b * b - 4 * a * c;

    if(d > 0) {
        root1 = (-b + sqrt(d)) / (2 * a);
        root2 = (-b - sqrt(d)) / (2 * a);
        printf("Roots are real and distinct: %.2f and %.2f\n", root1, root2);
    } else if(d == 0) {
        root1 = -b / (2 * a);
        printf("Roots are real and equal: %.2f\n", root1);
    } else {
        float realPart = -b / (2 * a);
        float imagPart = sqrt(-d) / (2 * a);
        printf("Roots are complex: %.2f + %.2fi and %.2f - %.2fi\n",
               realPart, imagPart, realPart, imagPart);
    }

    return 0;
}
// 17:Roots of quadratic eqautions
#include <stdio.h>
#include <math.h>

int main() {
    float a, b, c, d, root1, root2;
    printf("Enter coefficient of x^2: ");
    scanf("%f", &a);
    printf("Enter coefficient of x: ");
    scanf("%f", &b);
    printf("Enter constant: ");
    scanf("%f", &c);

    d = b * b - 4 * a * c;

    if(d > 0) {
        root1 = (-b + sqrt(d)) / (2 * a);
        root2 = (-b - sqrt(d)) / (2 * a);
        printf("Roots are real and distinct: %.2f and %.2f\n", root1, root2);
    } else if(d == 0) {
        root1 = -b / (2 * a);
        printf("Roots are real and equal: %.2f\n", root1);
    } else {
        float realPart = -b / (2 * a);
        float imagPart = sqrt(-d) / (2 * a);
        printf("Roots are complex: %.2f + %.2fi and %.2f - %.2fi\n",
               realPart, imagPart, realPart, imagPart);
    }

    return 0;
}
// 18: Grade Based on Marks
#include <stdio.h>
#include <math.h>

int main() {
    float a, b, c, d, root1, root2;
    printf("Enter coefficient of x^2: ");
    scanf("%f", &a);
    printf("Enter coefficient of x: ");
    scanf("%f", &b);
    printf("Enter constant: ");
    scanf("%f", &c);

    d = b * b - 4 * a * c;

    if(d > 0) {
        root1 = (-b + sqrt(d)) / (2 * a);
        root2 = (-b - sqrt(d)) / (2 * a);
        printf("Roots are real and distinct: %.2f and %.2f\n", root1, root2);
    } else if(d == 0) {
        root1 = -b / (2 * a);
        printf("Roots are real and equal: %.2f\n", root1);
    } else {
        float realPart = -b / (2 * a);
        float imagPart = sqrt(-d) / (2 * a);
        printf("Roots are complex: %.2f + %.2fi and %.2f - %.2fi\n",
               realPart, imagPart, realPart, imagPart);
    }

    return 0;
}
// 19: Triangle Classification
#include <stdio.h>

int main() {
    int marks;
    printf("Enter marks (0–100): ");
    scanf("%d", &marks);

    if(marks >= 90 && marks <= 100) {
        printf("A grade\n");
    } else if(marks >= 70 && marks < 90) {
        printf("B grade\n");
    } else if(marks >= 40 && marks < 70) {
        printf("C grade\n");
    } else if(marks >= 0 && marks < 40) {
        printf("Fail\n");
    } else {
        printf("Invalid marks\n");
    }

    return 0;
}
#include <stdio.h>

int main() {
    int a, b, c;
    printf("Enter side a: ");
    scanf("%d", &a);
    printf("Enter side b: ");
    scanf("%d", &b);
    printf("Enter side c: ");
    scanf("%d", &c);

    if(a == b && b == c) {
        printf("Equilateral triangle\n");
    } else if(a == b || b == c || c == a) {
        printf("Isosceles triangle\n");
    } else {
        printf("Scalene triangle\n");
    }

    return 0;
}
// 20: Day of the Week (Switch-Case)
#include <stdio.h>

int main() {
    int day;
    printf("Enter day number (1-7): ");
    scanf("%d", &day);

    switch(day) {
        case 1: printf("Monday\n"); break;
        case 2: printf("Tuesday\n"); break;
        case 3: printf("Wednesday\n"); break;
        case 4: printf("Thursday\n"); break;
        case 5: printf("Friday\n"); break;
        case 6: printf("Saturday\n"); break;
        case 7: printf("Sunday\n"); break;
        default: printf("Invalid day number\n");
    }

    return 0;
}

