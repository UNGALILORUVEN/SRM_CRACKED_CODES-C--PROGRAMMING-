**1). Simple Function**

      #include <stdio.h>
      #include <ctype.h>
      #include <string.h>
      int main() 
     {
      char str[30];
      char str2[]="zach";
      scanf("%s", str);
      int result;
      str[0]=tolower(str[0]);
      result=strcmp(str,str2);
      if (result==0) 
      {
          printf("%d", 18);
      }
      else
      {
          printf("%d", 0);
      }
      return 0;
    }
**2). SWAP**

      #include <stdio.h>
      int main()
      {
      int arr[3],i;
      for (i = 0; i < 3; i++) 
      {
        scanf("%d", &arr[i]);
      }
      printf("%d\n", arr[2]);
      printf("%d\n", arr[0]);
      printf("%d\n", arr[1]);
      return 0;
      }
 **3). Operators**
 
        #include <stdio.h>
        int main()
        {
        int n,a,b,i=0;
        scanf("%d",&n);
        for(i=0;i<n;i++)
        {
            scanf("%d%d",&a,&b);
            if(a<b)
                printf("<\n");
            else if (a>b)
                printf(">\n");
            else
                printf("=\n");
        }
        return 0;
        }
 **4). Remainder**
 
            #include <stdio.h>
            int main() 
            {
            int a,b, quotient, remainder;
            scanf("%d",&a);
            scanf("%d",&b);
            quotient=(int) (a/b);
            remainder=a%b;
            printf("%d\n", quotient);
            printf("%d\n", remainder);
            return 0;
            }
  **5). Display**
  
            #include<stdio.h>
            #include<math.h>
            int main()
            {
                   int n,i;
                  scanf("%d",&n);
                  for (i=(int)sqrt(n);i>=1;-1)
                   if(n%i==0)
                   {
                         printf("%d %d", i,n/i);
                         break;
                   }
             return 0;
             }
   **6). SERIES**
   
            #include<stdio.h>
            #include<math.h>
            int main()
            {
                  int i,N;
                  float sum;
                  int count;
                  scanf("%d",&N);
                  sum=0.0f;
                  count=1;
                  for(i=1;i<=N; i++)
                  {
                sum= sum + ( (float) (pow (count, 2))       /(float(pow(count,3)));
                        
           count+=2;
                  }
                  printf("Sum of the series is: %f", sum);
                  return 0;
            }
   
**7).IPL**

          #include<stdio.h>
          int main()
         {int arr[3],i;
          for (i=0;i<3;i++)
          {scanf("%d",&arr[i]);}
         printf("%d %o %x",arr[0],arr[1],arr[2]);
        return 0;
         }

**8).INTEGER**
    
       #include <stdio.h>

      unsigned int count1Bits(unsigned int n)
       {
           unsigned int count = 0;
         while (n) {
     count += n & 1;
    n>>= 1;
        }
       return count;
      }
      int main() 
      {
    unsigned int n;
     scanf("%d", &n);
    	printf("%d", count1Bits(n));
	return 0;
      }  
**9).TOURNAMENT**
       
     #include <stdio.h>
    int main()
    {
    int num,count = 0;
    scanf("%d",&num);
     while (num > 1) {
    num =(int) (num / 2 + num % 2);
    count += 1;
     }
	printf("%d", count);
	return 0;
     }
 **10). Nth FIBO**
 
 	#include<stdio.h>
 	int Fibonacci_Series(int);
 	int main()
	{
   		int Number, Fibonacci;
   		scanf("%d", &Number);
   		Fibonacci = Fibonacci_Series(Number);
		printf("%d", Fibonacci);
   		 return 0;
	}
 	int Fibonacci_Series(int Number)
	{
   		if ( Number == 0 )
    			return 0;
   		else if ( Number == 1 )
    			return 1;
   		else
    			return ( Fibonacci_Series(Number - 1) + Fibonacci_Series(Number - 2) );
	}
**19). Greddy Puppy

	#include <stdio.h>
	int main() 
	{
  	int t,n,k;
  	scanf("%d", &t);
  	int i=0,j=0, max=0;
  	for (i=0;i<t;i++)
  	{
   		scanf("%d%d", &n,&k);
    		for(j=1;j<=k;j++)
   		{
    		if((n%j)>max)
  		{
    			max=n%j;
   		}
 		}
 		printf("%d\n",max);
 		max=0;
 	}
	return 0;
	}
**20). Finding Bitwase EXOR of Two Numbers

	#include <stdio.h>
	int main()
	{
 	int a,b;
 	scanf("%d", &a);
 	scanf("%d",&b);
 	printf("Bitwise EX-OR of ");
 	printf("%d", a);
 	printf(" and ");
 	printf("%d",b);
 	printf(" is= ");
 	printf("%d" ,a^b);
 	return 0;
	}
**21). Case of Zeros and Ones

	#include<stdio.h>
	#include<stdlib.h>
	int main()
	{
  		int n,i,c1=0,c0=0;
  		char c[200001];
  		scanf("%d", &n);
  		scanf("%s",c);
  		for(i=0;i<n;i++)
  		if(c[i]=='1')
    			c1++;
  		else
    			c0++;
    		printf("%d",abs(c1-c0));
 		return 0;
	}
**22). Shape Up


	#include<stdio.h>
	int main()
	{
  		int a;
  		scanf("%d", &a);
  		switch(a)
  		{
    		case 7:
     			printf("Heptagon");
     			break;
    		case 8:
    			printf("Octagon");
     			break;
    		case 9:
     			printf("Nanogon");
     			break;
    		case 10:
     			printf("Decagon");
     			break;
   		default:
    			printf("Not identified");
  		}
		return 0;
	}
	
	
	
**TO BE CONTINUED..........**
