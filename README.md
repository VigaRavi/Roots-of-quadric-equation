# Roots-of-quadric-equation
//roots of quadric equations


#include<stdio.h>
#include<math.h>


int main()
{
	double b,a,c,root1,root2,discriment;
	printf("type the value for b:");
	scanf("%lf",&b);
		printf("type the value for a:");
	scanf("%lf",&a);
		printf("type the value for c:");
	scanf("%lf",&c);
	
	discriment=b*b-(4*a*c);
	
	if(discriment>0)
	{
		root1=(-b+sqrt(discriment))/2*a;
			root2=(-b-sqrt(discriment))/2*a;
			printf("%lf,%lf",root1,root2);
			}
	
	else if(discriment==0)
	{
		root1=root2=-b/2*a;
		printf("%lf",root1);
	}
	else
	{

root1=-b/2*a+(sqrt(-discriment)/2*a);
root2=-b/2*a-(sqrt(-discriment)/2*a);
printf("%lf,%lf",root1,root2);
	}
	
}
