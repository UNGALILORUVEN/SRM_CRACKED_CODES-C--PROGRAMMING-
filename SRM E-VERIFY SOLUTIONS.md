**1).billing id**

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

**2).types of triangle**
        
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
**3). Divide and eat

	#include <stdio.h>
	int main() {
	int x, y;
	int div_result; 
    	scanf("%d", &x);
    	scanf("%d", &y);
   
   	if(y != 0)
     	{
   		div_result = (int)x/(int)y;
		printf("%.1d\n", div_result);
	 } 
	else 
	 {
	 		printf("Division not possible.\n");
	  }
  	return 0;
	}
**4). Sorting employees**
	
	#include<stdio.h>
	#include<string.h>

	typedef struct
	{
  	char name[110];
  	int salary;
	}
	employee;

	int main(){
  	int t;
  	scanf("%d",&t);
  	while(t--)
    {
      int n,i,j,z;
      employee e[1001], temp;
      scanf("%d",&n);
      for(i=0; i<n; i++)
      {
        scanf("%s",e[i].name);
        scanf("%d",&e[i].salary);
      }
      for(i=0;i<n-1;i++)
      {
        for(j=i+1;j<n;j++)
        {
          if(e[i].salary>e[j].salary)
          {
            temp=e[i];
            e[i]=e[j];
            e[j]=temp;
          }
          
          if(e[i].salary == e[j].salary)
          {
            int l1= strlen(e[i].name);
            int l2=strlen(e[j].name);
            int small=l1;
            if(l2<l1)
              small=l2;
           	for(z=0;z<small;z++)
            {
              if(e[i].name[z]<e[j].name[z])
                break;
              else
              {
                temp=e[i];
                e[i]=e[j];
                e[j]=temp;
              }
            }
          }
        }
      }
      
      for(i=0;i<n;i++)
      {
        printf("%s %d",e[i].name,e[i].salary);
        if(i!=n-1)
          printf(" ");
      }
      printf("\n");
    }
	return 0;
    }
**5). Lion club**

	#include<stdio.h>
	long long int data[41][2];
	long long int Answer(int k,int num);
	int main()
	{
  	int t,n,m,c,p,i;
  	long long int answer;
  	scanf("%d",&t);
  	while(t--)
  	{
    	scanf("%d%d",&n,&m);
    	answer=0;
  	for(i=0;i<41;i++)
   	 data[i][0]=data[i][1]=0;
  	for(i=0;i<n;i++)
   	 {
      	scanf("%d%d",&c,&p);
      	data[c][0]+=p;
      	data[c][1]++;
    	}
  	for(i=1;i<=40;i++)
  	if(data[i]>0)
      	answer+=data[i][0]*(1<<(data[i][1]-1))*Answer(m-1,i);
      	printf("%.9lf\n",(double)answer/Answer(m,0));
  	}
   	return 0;
	}
  	long long int Answer(int k,int num)
  	{
  	long long int answer=0,e[41][41],v[41];
  	int i,j=1,tot=0;
  	for(i=0;i<41;i++)
    	if(data[i][0]>0&&i!=num)
    	{
  		v[j++]=(1<<data[i][1])-1;
  		tot++;
    	}
       for(i=0;i<tot+1;i++)
        e[i][0]=1;
        for(i=0;i<tot+1;i++)
        for(j=1;j<=tot;j++)
        if(j>i)
        e[i][j]=0;
        else
        e[i][j]=e[i-1][j]+e[i-1][j-1]*v[i];
        for(i=k;i<=tot;i++)
        answer+=e[tot][i];
        return answer;
       }
 **6). Reverse string**

	#include <stdio.h>
	int main()
	{
  	int a,b,c;
  	long d;
  	scanf("%d",&a);
 	 while(a--)
 	 {
    	long rev=0;
    	scanf("%ld",&d);
    	while(d!=0)
    	{
      		c=d%10;
     	        rev=rev*10+c;
      		d=d/10;
    	}
    	printf("%ld\n",rev);
  	}
    	return 0;
	)
**7). Harry and his mixtures** 

	#include <stdio.h>
	int main()
	{
  	int num_mixtures,i,j,k;
  	while(scanf("%d",&num_mixtures)!=EOF)
 	{
    		int mix[num_mixtures];
    		for(i=0;i<num_mixtures;i++)
    	{
      	scanf("%d",&mix[i]);
    	}
    int smoke[num_mixtures][num_mixtures];
    int color[num_mixtures][num_mixtures];
    int sum=0;
    for(i=0;i<num_mixtures;i++)
    {
      sum=color[i][i]=mix[i];
      for(j=i+1;j<num_mixtures;j++)
      {
        sum+=mix[j];
        color[i][j]=sum%100;
      }
    }
    for(i=0;i<num_mixtures;i++)
      smoke[i][i]=0;
    int l,curr_val;
    for(l=2;l<=num_mixtures;l++)
    {
      for(i=0;i<=num_mixtures-l+1;i++)
      {
        j=i+l-1;
        smoke[i][j]=0x7fffffff;
        for(k=i;k<j;k++)
        {
          curr_val=smoke[i][k]+smoke[k+1][j]+color[i][k]*color[k+1][j];
          if(curr_val<smoke[i][j])
            smoke[i][j]=curr_val;
        }
      }
    }
    printf("%d\n",smoke[0][num_mixtures-1]);
    }
    return 0;
    }
**8). SUM**

	#include <stdio.h>
	int main()
	{
 	int t,i,j,d,n,p;
  	scanf("%d",&t);
  	for(i=1;i<=t;i++)
 	{
    	scanf("%d%d",&d,&n);
    	for(j=1;j<=d;j++)
   	{
      p=n*(n+1)/2;
      n=p;
    }
    printf("%d\n",p);
    }
    return 0;
    }
 **9). 0's and 1's** 
 
	#include <stdio.h>
	#include <stdlib.h>
	int main()
	{
  	int n,i,c1=0,c0=0;
  	char c[200001];
  	scanf("%d",&n);
  	scanf("%s",c);
  	for(i=0;i<n;i++)
    	if(c[i]=='1')
      	c1++;
  	else
    		c0++;
  	printf("%d",abs(c1-c0));
  	return 0;
	}
**10). SWITCH INTEGER**

	#include<stdio.h>
	int main()
	{
  	int a,b,c;
  	long d;
  	scanf("%d",&a);
  	while(a--)
  	{ 
    	long s=0;
    	scanf("%ld",&d);
    	while(d!=0)
 	 {
    	c=d%10; 
    	s=s*10+c;
    	d=d/10;
  	}
   	 printf("%ld\n",s);
  	}
  	return 0;
	}
**11). POWER OF 2**

	#include <stdio.h>
	int main()
	{
  	int num;
  	scanf("%d",&num);
  	if( (num!=0) && ( (num & (num - 1))==0))
    	printf("WOW");
	else
    	printf("OOPS");
  	return 0;
	}
**12). Sum of three**
	
	#include<stdio.h>
	int main ()
	{
	int a,b,c,d;
	scanf("%d %d %d",&a,&b,&d);
	c=a+b+d;
	printf("%d",c);
	return 0;
	}
**13). Race in secomds**

	#include <stdio.h>
	int main()
	{int a;
 	int d,m,s,h;
 	scanf("%d",&a);
 	d=a/(24*3600);
 	h=(a%(24*3600))/3600;
	 m=(a%3600)/60;
 	s=(a%3600)%60;
 	printf("The Duration is %d days %d hours %d minutes %d seconds",d,h,m,s);
 		return 0;
	}
**14). Maths assignment**

	MATH#include<stdio.h>
 
	#define MOD 1000000007
 
	int count;
 
	void calc(int chef[], int n, int sum, int index)
	{
	//printf("n=%d sum=%d index=%d count=%d\n",n,sum,index,count);
	if(index<0)
		return;
	if(sum<0)
		return;
	if((long long)chef[index]*n < sum)
		return;
	if(n==0)
	{
		if(sum==0)
			count=(count+1)%MOD;
		return;
	}
	calc(chef,n-1,sum-chef[index],index);
	calc(chef,n,sum,index-1);	
	}
 
	int main()
	{
	int i, q, x, k;
	int chef[43];
	chef[0]=1;
	chef[1]=2;
	for(i=2;i<43;i++)
		chef[i]=chef[i-1]+chef[i-2];
	scanf("%d",&q);
	while(q--)
	{
		count=0;
		scanf("%d%d",&x,&k);
		calc(chef,k,x,42);
		printf("%d\n",count);
	}
	return 0;
	} 
**15). Hours and minutes**

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
**16). Kilometres**

	#include <stdio.h>

	int main() {
	float kilometers;
	scanf("%f", &kilometers);
	float miles = (kilometers*0.6213712);
	printf("%f miles per hour", miles);
  	return 0;
	}
**17). Distance**

	#include <stdio.h>

	struct Distance

	{

  	int feet;

  	float inch;

	}d1,d2,sumOfDistances;

	int main()

	{

 	 scanf("%d %f\n",&d1.feet,&d1.inch);

  	scanf("%d %f\n",&d2.feet,&d2.inch);

  	{

    sumOfDistances.feet=d1.feet+d2.feet;

    sumOfDistances.inch=d1.inch+d2.inch;

    printf("Sum of distances=%d feet and %.2f inches",sumOfDistances.feet,sumOfDistances.inch);

  	}

  	return 0;
	}
**18). Day DREAM**

	#include <math.h>
	#include <stdio.h>
		#include <string.h>
		#include <stdlib.h>
	#include <assert.h>
	#include <limits.h>
	#include <stdbool.h>

	int main(){
    int n; 
    int m; 
    scanf("%d %d",&n,&m);
    int sup = ((n + 1) / 2) * ((m + 1) / 2);
    printf("%d\n", sup);
    return 0;
    }
  **19). Magical Game of sum**
  
  	#include <stdio.h>
	int main() 
	{
  	int t,i,j,d,n,p;
  	scanf("%d",&t);
  	for(i=1;i<=t;i++)
   	{
    	scanf("%d%d",&d,&n);
    	for(j=1;j<=d;j++)
     	{
      	p=n*(n+1)/2;
      	n=p;
  	}
    	printf("%d\n",p);
	  }
           
	return 0;
	}
**20). Grading system**

	#include <stdio.h>
	int main() {
	int t;
 	 scanf("%d",&t);
  	while (t--)
  	{
    	int a,b;
    	float c;
    	scanf("%d %f %d",&a,&c,&b);
   	 if (a>50&& c<0.7 && b>5600)
    	  printf("10\n");
    	else if (a>50&& c<0.7)
    	  printf("9\n");
  	 else  if (c<0.7 && b>5600)
     	 printf("8\n");
   	else  if (a>50 && b>5600)
      	printf("7\n");
    	else if (a>50|| c<0.7 || b>5600)
      	printf("6\n");
   	 else 
	      printf("5\n");
  	}
	return 0;
	}
