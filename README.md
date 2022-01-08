/*100到200之间的素数*/
#include<stdio.h>
int main()
{
	int prime(int);
	int n;
	for(n=100;n<200;n++)
	{
	  if(prime(n))
	    printf("%d   \n",n);
	}
	return 0; 
 } 
 
 int prime(int n)
 {
 	int flag=1,i;
 	for(i=2;i<n/2&&flag==1;i++)
 	  if(n%i==0)
 	    flag=0;
 	return (flag);
 }
