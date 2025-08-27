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
// 3: Write a program to calculate the area and perimeter of a rectangle given its length and breadth.

#include<stdio.h>
int main () {
    int l, b;
    printf("enter l : ");
    scanf("%d", &l);
    printf("enter b : ");
    scanf("%d", &b);
    
    printf("perimeter is %d\n", 2*(l+b));
    printf("area is %d\n", l*b);
   
    
       return 0;
}
// 4: Write a program to calculate the area and circumference of a circle given its radius.

#include<stdio.h>
int main () {
    float r;  // r= radius;
    printf("enter r : ");
    scanf("%f", &r);
   
    printf("circumference is %f\n", (2*3.14*r));
    printf("area is %f\n", (3.14*r*r));
   
    
       return 0;
}
// 5: Write a program to convert temperature from Celsius to Fahrenheit

#include<stdio.h>
int main () {
    float c;  // c = celsius;
    printf("enter c : ");
    scanf("%f", &c);
   
    printf("temperature in fahrenheit is  %f\n", (c*9/5+32));

   
    
       return 0;
}
// 6: Write a program to swap two numbers using a third variable

#include<stdio.h>
int main () {
    int a, b;  
    printf("enter a : ");
    scanf("%d", &a);
    printf("enter b : ");
    scanf("%d", &b);
     
     int c = a;
     a = b;
     b = c;
    printf(" a = %d\n", a);
    printf(" b = %d\n", b);
    
       return 0;
}
// 7: Write a program to swap two numbers without using a third variable

#include<stdio.h>
int main () {
    int a, b;  
    printf("enter a : ");
    scanf("%d", &a);
    printf("enter b : ");
    scanf("%d", &b);
     
     a = a + b;
     b = a - b;
     a = a - b;
    printf(" a = %d\n", a);
    printf(" b = %d\n", b);
    
       return 0;
}

