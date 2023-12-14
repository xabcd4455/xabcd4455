Practical No.4

MUL AND DIV 8 BIT NO.BY 8 BIT

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

void main(void) {

int i,sum,n;

int number[] = {1,2,3,4,5,6,7,8,9,10};

sum = 0;

for(i=0; i<=9;i++)

{

sum = sum+number[i]; }

TRISB =0;

PORTB = sum;

//n = 0xFF + OXFF;
}


Practical No.3


a)Internal to internal memory transfer

#include <stdio.h>

#include <stdlib.h>

#include <pic18f4550.h>

void main(void) {

int i;

int source1[] = {0x21,0x22,0x23,0x24,0x25};

int dest[] = {0x00,0x00,0x00,0x00,0x00};

for(i=0; i<=4;i++) {

// counter = 5

dest[i] = source1[i];

// source to destination

}

}


b)memory exchange program

#include <stdio.h>

#include <stdlib.h>

#include <pic18f4550.h>

void main(void) {

int temp,i;

int source1[] = {0x21,0x22,0x23,0x24,0x25};

int dest[] = {0x99,0x99,0x99,0x99,0x99};

for(i=0; i<=4;i++) {

temp = source1[i];

source1[i] = dest[i];

dest[i] = temp; }

}

Practical No.5

Progrm for sorting of no. in ase and des order

#include <stdio.h>

#include <stdlib.h>

#include <pic18f4550.h>

void main(void)

{

int i,j,temp;

int num_asc[] = {10,2,5,1,6};

for(i=0;i<=4;i++)

{

for(j=i+1;j<=4;j++)

if (num_asc[i]> num_asc[j])

{

temp = num_asc[i];

num_asc[i]= num_asc[j];

num_asc[j]= temp;

}

}
}


Practical No.6

 Program for LED interfacing:

#include<p18f4520.h>

void delay(unsigned int itime);



void main()

{

TRISD=0;

{

while(1)

{

PORTD=0X00;

delay(100);

PORTD=0xIF;

delay(100);

}

}

}

void delay(unsigned int itime)

{

int i,j;

for(i=0;i<=itime;i++)

for(j=0;j<=1275:j++);

}

