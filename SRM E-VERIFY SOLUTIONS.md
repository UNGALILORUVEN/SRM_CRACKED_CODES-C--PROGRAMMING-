**billing id**
2
#include <stdio.h>
          int main()
       {
       int bid,pid,q;
    float pr,out;
      scanf("%d%d",&bid,&pid);
     scanf("%f",&pr);
    if((bid>=1000)&&(bid<=9999))
    {
    if ((pid>=1000)&&(pid>=9999)) 
    {
      if((pr>=10)&&(pr<=500))

       {  
    }}}
     scanf("%d",&q);
     out=pr*q;
     printf("%.2f",out);
    return 0;
     }

**types of triangle**
        #include<stdio.h> 
        #include<math.h> 
        int main(void)
{   
    float a, b, c, s, area;
    scanf("%f", &a);
    scanf("%f", &b);
    scanf("%f", &c);
    if( (a + b > c) && (b + c > a) && (c + a > b) )
    {
        if( (a == b) && (b == c) )

       {
            printf("Triangle is equilateral.\n");

        }
        else if( (a == b) || (b == c) || (a == c) )
        {
            printf("Triangle is isosceles ");
        }
        else
        {
	printf("Triangle is scalene");
        }
}
    return 0; 
}