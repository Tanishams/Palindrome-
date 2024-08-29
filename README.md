# Palindrome-
A program to find the reverse of a positive integer and to check if the value is  PALINDROME or NOT. 
#include<stdio.h>
int main()
{
   int n,m,reverse,digit;
   printf("Enter the value of n\n");
   scanf("%d",&n);
   reverse=0;
   m=n;
   while(n!=0)
   {
      digit=n%10;
      n=n/10;
      reverse=digit+10*reverse;
   }
   printf("Reverse of %d is %d\n",m, reverse);
   if(m==reverse)
      printf("It is a palindrome\n");
   else
      printf("It is not a palindrome\n");
}
