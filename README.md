Practical No.4

#include<stdio.h>
#include<stdlib.h>
#include<p18f4550.h>
void main(void)
{
int MUL,DIV;
MUL=0;
DIV=0;
MUL= 0X04*0X01;
DIV=0X06/0X02;
TRISD=0;
PORTD=MUL;
TRISC=0;
PORTC=DIV;
}

Practical No.1

#include<stdio.h>
#include<stdlib.h>
#include<p18f4550.h>
void main(void)
{
int sum;
sum =0;
sum= 0x05+0X02;
TRISD=0;
PORTD=sum;
}


Practical No.2

Program: addition of array of numbers

#include <stdio.h>
#include <stdlib.h>
#include <pic18f4550.h>
void main(void)
{
int i,sum,n;
int number[] = {1,2,3,4,5,6,7,8,9,10); 
sum = 0;
for(i=0; i<=9;i++)
{
sum = sum+number[i];
}
TRISB =0;
PORTB = sum;
//n = 0xFF + OXFF;
}




