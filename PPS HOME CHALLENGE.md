
	#include<stdio.h>
	int main()
	{
	int a=2,b=3,c=5,sum;
	sum=a+b+c;
	printf("the num 2,3,5");
	printf("\nthe sum of these three num is:%d",sum);
	return 0;
	}

OUTPUT FOR ABOVE PROGRAM:
		
		output 1:the num 2,3,5
		the sum of these three num is:10

**program 2**

	#include<stdio.h>
	int main()
	{
	int a=3,b=2,sum,diff;
	sum=a+b;
	diff=a-b;
	printf("the sum of these 3,2  is:%d",sum);
	printf("\n\nthe diff of these 3,2 is:%d",diff);
	return 0;
	}

**output FOR ABOVE PROGRAM:**

		the sum of these 3,2  is:5
		the diff of these 3,2 is:1 
	output:
		the num 2,3,5the sum of these three num is:10
**PROGRAM 3**

	#include <stdio.h>
	int main()
	{
	printf("In Programming for problem solving,\nl know about:\n1.header\n2.initialization\n3.declaration\n4.data types\n5.function ");

  	return 0;
	}

**arithmatic operators(program 4)**

	#include <stdio.h>
	main() 
	{
  	 int a = 21;
  	 int b = 10;
  	 int c ;
   	 c = a + b;
   	 printf("Line 1 - Value of c is %d\n", c );
   	 c = a - b;
         printf("Line 2 - Value of c is %d\n", c );
	 c = a * b;
  	printf("Line 3 - Value of c is %d\n", c );
	c = a / b;
   	printf("Line 4 - Value of c is %d\n", c );
 	return 0;
 	}
**PROGRAM 4**

	#include <stdio.h>
	int main()
	{
    		int tamil,english,maths,physics,chemistry,computer_science,total;
   		float avg;
    		tamil=85,english=97,maths=70,physics=65,chemistry=78,computer_science=99,total=0,avg=0;
   		total=tamil+english+maths+physics+chemistry+computer_science;
    		avg=(float)total/5;
    		printf("the total marks subject tamil,english,maths,physics,chemistry,computer_science is: %d",total);
   		printf("\nthe total average is :%2.f",avg);
    		return 0;
		}
**OUTPUT FOR ABOVE PROGRAM**

	output  :
		
		the total marks subject tamil,english,maths,physics,chemistry,computer_science is: 494                          the total mark is :99.0  
**PROGRAM GDB LINK FOR ABOVE PROGRAM** 
   
	https://onlinegdb.com/SyD8OXZiw

**PRE INCREAMENT AND POST INCREAMENT(PROGRAM 5)**

	#include <stdio.h>
	int main()
	{
    		int inc1;
    		int inc;
    		scanf("%d",&inc1);
    		inc1=inc;
   		printf("The preincrement is =%d",--inc1);
    		printf("\nThe postincrement is =%d",inc++); 
    		return 0;
	}

**PROGRAM GDB LINK FOR ABOVE PROGRAM** 
	
	https://onlinegdb.com/hWiuNQRAh

**PRE INCREAMENT AND DECREAMENT**
	
	#include <stdio.h>
	int main()
	{
   	 int x,y;
	 x=5;
    	 y=2;
   	 printf("%d",x);  //printing without any change
   	 printf("\n%d",++x);  //pre increament change in value in first step
  	 printf("\n%d",x);  //pre increament applied but x is executed already
   	 printf("\n---------\n");// DECORATION
  	 printf("\n%d",y);  //printing the value with out changes
   	 printf("\n%d",--y);  //pre decreament change in value in first step
   	 printf("\n%d",y);  //pre decreament applied but y is executed  already
   	 return 0;
	 } 
//NOTE: (PRE) MEANS CHANGE FROM THE NEXT STEP WHEATHER INCREASE OR DECREASE NOT FROM THAT STEP

**PROGRAM GDB LINK FOR ABOVE PROGRAM** 
	
	https://onlinegdb.com/dLXB8kmEq

**POST INCREAMENT AND DECREAMENT**

	#include <stdio.h>
	int main()
	{
    		int x,y;
    		x=5;
    		y=2;
    		printf("%d",x);  //printing without any change
    		printf("\n%d",x++);  //post increament applied but x is executed first no change in value
    		printf("\n%d",x);  //post increament change in value after the next step
    		printf("\n---------\n");// DECORATION
    		printf("\n%d",y);  //printing the value with out changes
    		printf("\n%d",y--);  //post decreament applied but y is executed first no change in value
    		printf("\n%d",y);  //post decreament change in value after the next step
    		return 0;
		}
//NOTE : (POST) MEANS CHANGE FROM THE NEXT STEP WHEATHER INCREASE OR DECREASE NOT FROM THAT STEP
