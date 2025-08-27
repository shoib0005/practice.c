// 1:  Write a program to input two numbers and display their sum

#include<stdio.h>
int main () {
    int a, b;
    printf("enter a : ");
    scanf("%d", &a);
    printf("enter b : ");
    scanf("%d", &b);
    
    printf("sum is %d\n", a+b);

}
// 2: Write a program to input two numbers and display their sum, difference, product, and quotient
#include<stdio.h>
int main () {
    int a, b;
    printf("enter a : ");
    scanf("%d", &a);
    printf("enter b : ");
    scanf("%d", &b);
    
    printf("sum is %d\n", a+b);
    printf("difference is %d\n", a-b);
    printf("product is %d\n", a*b);
    printf("quotient is %d\n", a/b);
    
       return 0;
}
