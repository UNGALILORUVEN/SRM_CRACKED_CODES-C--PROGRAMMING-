 squares in n*n board
 
 #include <stdio.h>
 int main() {
  int n,squarecount;
  scanf("%d",&n);
  squarecount = ( (n * (n+1) * (2*n + 1))/6 );
  printf("%d", squarecount) ;
	return 0;
}

Kilometers to miles

#include <stdio.h>

int main() {
	float kilometers;
	scanf("%f", &kilometers);
	float miles = (kilometers*0.6213712);
	printf("%f miles per hour", miles);
  return 0;
}

 Largest Number
 
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

 Hours and Minutes
 
 #include <stdio.h>
int main()
{
  int min,hrs,mins;
    scanf("%d",&min);
  hrs=min/60;
  mins=min%60;
  printf("%d Hours, %d Minutes.",hrs,mins);
  return 0;
}

Vote

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

 CUBE
 
 #include <stdio.h>
int main() {
	int cube,number;
  scanf("%d", &number);
  cube = number*number*number;
  printf("CUBE is: %d",cube);
  return 0;
}

Minutes

#include <stdio.h>
int main() 
{
  int hrs,mins,minutes;
  scanf("%d %d", &hrs,&mins);
  minutes = (mins * 60) + (hrs * 60 * 60) ;
  printf("%d minutes",minutes);
	return 0;
}

Sphere

#include <stdio.h>
int main() {
	float pi = 3.14, radius,volume;
  scanf("%f",&radius);
  volume = (4.0/3.0)*pi*(radius*radius*radius);
  printf("%f",volume);
  return 0;
}