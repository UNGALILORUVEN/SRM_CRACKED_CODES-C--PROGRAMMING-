**1).squares in n*n board**

    #include <stdio.h> 
    int main()
    {
    int n,squarecount;
    scanf("%d",&n); 
    squarecount = ( (n * (n+1) * (2*n + 1))/6 );
    printf("%d", squarecount) ;
    return 0;
    }

**2).Kilometers to miles**

	#include <stdio.h>
	int main()
	{
	float kilometers;	
	scanf("%f", &kilometers);
	float miles = (kilometers*0.6213712);
	printf("%f miles per hour", miles);
	return 0;
	}
 **3).Largest Number**
 
 	#include <stdio.h>
 	int main() {
 	int a,b,c;
	scanf("%d %d %d", &a, &b, &c);
	if(a >= b && a>=c)
	printf("%d",a);
	if(b >=c && b >=a)
		printf("%d",b);
	if(c >=a && c >= b)
	    printf("%d",c);
	    return 0;
	}
 **4).Hours and Minutes**
 
 	#include <stdio.h>
 	int main(){
   	int min,hrs,mins;
       	scanf("%d",&min);
    		hrs=min/60;
    		mins=min%60;
    	printf("%d Hours, %d Minutes.",hrs,mins);
    	return 0;
	}
**5).Vote**

	#include <stdio.h>
	int main() {
	int age;
	scanf("%d",&age);
	if(age<18)
	   {    
	      printf("Not eligible");
	   }
	else
	  {
	  printf("Eligible");
	  }
	return 0;
	}
**6).CUBE**

	#include <stdio.h>
	int main()
	{
	int cube,number;
  	scanf("%d", &number);
  	cube = number * number * number;
  	printf("CUBE is: %d",cube);
  	return 0;
	}
**7).Minutes**

	#include <stdio.h>
	int main() {
	int hrs,mins,minutes;
	scanf("%d %d", &hrs,&mins);
	minutes = (mins  *  60) + (hrs [enter link description here](www.gogle.com)*60 * 60) ;
	printf("%d minutes",minutes);
	return 0;
	}
**8).Sphere**

	#include <stdio.h>
	int main() {
	float pi = 3.14, radius,volume;
	scanf("%f",&radius);
	volume = (4.0/3.0) * pi * (radius * radius * radius);
	printf("%f",volume);
	return 0;
	}
**9).Name and Birth**

	#include <stdio.h>
	int main() {
	char fn[30],ln[30];
	int y;  
	scanf("%s",fn);
	scanf("%s",ln);
	scanf("%d",&y);
	printf("%s %s %d\n",fn,ln,y);
	return 0;
	}
**10).Triangle**

	#include <stdio.h>
	int main()
	{
      	int ang1, ang2, ang3;
      	scanf("%d, %d", &ang1, &ang2);
      	ang3 = 180 - (ang1 + ang2);
      	printf("%d\n", ang3);
      	return 0;
 	}
**11).Theatre Square**

	#include<math.h>
	#include <stdio.h>
	int main()
	{
  	float m,n,o;
  	int p,q,r;
  	scanf("%f %f %f",&m,&n,&o);
  	p= ceil(m/o);
  	q= ceil(n/o);
  	r=p*q;
  	printf("%d",r);
	return 0;
	}
 **12).Pow**
 
 	#include <stdio.h>
	#include <math.h>
	int main() {
	int a,b,c;
	scanf("%d%d",&a,&b);
  	c=pow(a,b);
  	printf("%d",a);
  	printf(" to the power of ");
  	printf("%d",b);
  	printf(" is= %d",c);
	return 0;
	}
**13).Addition, Subtraction, multiplication, Division**
	
	#include <stdio.h>
	int main() {
  	int add,sub,mul,p,q,mod=0;
  	float div;
  	scanf("%d,%d",&p,&q);
  	add=p+q;
  	sub=p-q;
  	mul=p * q;
  	div=p/q;
  	mod=p%q;
  	printf("\nAddition : %d",add);
  	printf("\nSubtraction : %d",sub);
  	printf("\nMultiplication : %d",mul);
  	printf("\nDivision : %f",div);
  	printf("\nMODULUS = %d",mod);
  	return 0;
	}
**14).Float and Double**

	#include <stdio.h>
	int main() {
    	float b;
  	double a;
	scanf("%lf%f",&a,&b);
    		printf("%lf\n%f",a,b);
	return 0;
	}
**15).Sum of Three numbers**
	
	#include <stdio.h>
	int main() {int a,b,c,t;
	scanf("%d,%d,%d",&a,&b,&c);
     	t=a+b+c;
         printf("%d",t);
	return 0;
	}
**16).Rectangular**

	#include<stdio.h>
	int main()
	{
  	int height,width,perimeter,sub;
 	scanf("%d%d",&height,&width);
	 sub=height+width;
 	perimeter=sub * 2;
 	printf("%d",perimeter);
 	return 0;
	}
**17). Quotient and reminder**
	
	#include <math.h>
	#include <stdio.h>
	int main() {
  	int divider,divisor,quotient,remainder;
  	scanf("%d",&divider);
  	scanf("%d",&divisor);
  	quotient=divider/divisor;
  	remainder=divider%divisor;
  	printf("quotient: %d",quotient);
  	printf(", remainder: %d",remainder);
	return 0;
	}
**18). ASCII**

	#include <stdio.h>
	int main() {  
   	char c;
    	scanf("%c", &c);  
    	printf("%d.", c);
    	return 0;
	}
**19). Bottle Deposits**

	#include <stdio.h>
	#include <math.h>
	int main()
	{
	int a, b;
	float c;
	scanf("%d%d",&a,&b);
	c=a*0.10+5*0.25;
	printf ("Refunds for Bottles=%.2f",c);
	return 0;
	}
**20). Xavier Math**

	#include <stdio.h>
	int main()
	{
    	int n, i,sum = 0;
    	scanf("%d",&n);
    	for(i=1;i<n; i++)
    	{
       		 printf("%d+", i);
        	 sum +=i;
    	}
   	printf("%d=%d", n, sum+n);
    	return 0;
	}
**21). Twos Mod**

	#include <stdio.h>
	int main()
	{
	int a,b,c;
	scanf("%d%d",&a,&b);
	c=a%b;
	printf("%d",c);
	return 0;
	}
**22). elab Fuel Bank in India**

	

	#include <stdio.h>
	int main()
	{
	float a,b;
	scanf("%f",&a);
	b=282.48/a;
	printf("%.2f",b);
	return 0;
	}
**23). Sum of the series**

	#include <stdio.h>
	int series_sum(int n)
	{
	return((n*(n+1)*(2*n+4))/12);
	}
	int main()
	{
	int n;
	scanf("%d",&n);
	printf("%d", series_sum(n));
	return 0;
	}
**24). Welcome to world**

	#include <stdio.h>
	int main ()
	{
	char n[20];
	char c[20];
	char p[20];
	int s;
	float sp;
	scanf("%s",n);
	scanf("%s",c);
	scanf("%s",p);
	scanf("%d",&s);
	scanf("%f",&sp);
	printf("Robot Details\n");
	printf("I am the Robot named=%s\n",n);
	printf("I was created by %s\n", c);
	printf ("I am created for the purpose of %s\n",p);
	printf("My memory space is around %dmb and my speed is %.1fTB",s,sp);
	return 0;
	}
**25). Mathematics Double**

	#include <stdio.h>
	int main()
	{
	float num1, num2;
	scanf("%f", &num1);
	scanf("%f", &num2);
	double res1 = (double) num1;
	double res2 = (double) num2;
	printf("%f\n", res1);
	printf("%f\n", res2);
	return 0;
	}
	
**26).Tsunami Indonesia**

	#include <stdio.h>
	int main() {
	int Dead, Injured, Safe;
	scanf("%d%d%d", &Dead, &Injured, &Safe);
	printf("TSUNAMI REPORT\n");
	printf("The number of people\n");
	printf("Dead=%d\nInjured=%d\nSafe=%d",Dead, Injured, Safe);
	return 0;
	}

**28).GRAVITY FALL**

	#include<stdio.h>
	#include<math.h>
	int main ()
	{
	float vf, vi=0, a=9.8,h;
	scanf("%f", &h);
	vf=sqrt(vi+(2*a*h));
	printf("The object will hit the ground at %.2f m/s",vf);
	return 0;
	}
**29).FEES CALCULATOR**

	#include <stdio.h>
	int main() {
	char s[1];
	int sum=0;
	int paper, rtee, arrear,afees;
	scanf("%s", s);
	scanf("%d", &paper);
	scanf("%d", &rtee);
	scanf("%d", &arrear);
	scanf("%d", &afees);
	sum=(paper*rtee)+(arrear*afees);
	switch(s[0])
	{
	case 'A':printf("The fee to be paid is Rs=%d",sum);
	break;
	case 'B':printf("The fee to be paid is Rs=%d",sum=sum+5000);
	break;
	case 'C': printf("The fee to be paid is Rs-%d",sum=sum+1500);
	break;
	case 'D':printf("The fee to be paid is Rs=%d", sum=sum+6500);
	break;

	}
	return 0;
	}

**IO22**

TO BE CONTINUED.......
