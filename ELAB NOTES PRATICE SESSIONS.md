#include<stdio.h>
int main()
	{
  		int a, b, c;
  		printf("\n Please Enter two angles of a triangle \n");
  		scanf("%d%d",&a,&b);
   		c= 180 - (a + b);
   		printf("\n Third Angle of a Triangle = %.2d\n", c);
  		return 0;
	}	

//volume of sphere 1
int main()
{
	float v,r;
	scanf("%f",&r);
        v=(4*22*r*r*r)/(7*3); 
	printf("%f",v);
	return 0;
}

#include<stdio.h>
int main()
{
	float v,r;
	scanf("%f",&r);
        v=(4*3.14*r*r*r)/(3); 
	printf("%f",v);
	return 0;
}
//3.
#include<stdio.h>
int main()
{
	float v,r;
	scanf("%f",&r);
        v=(r*r*r)*(4/3)*(22/7); 
	printf("%f",v);
	return 0;
}

//4.
#include <stdio.h>
int main()
{
	float v,r,b,g,k,i;
	scanf("%f",&r);
    b=7*3;
    g=r*r*r;
    k=4*22;
    i=k*g;
    v=i/b;
	printf("%f",v);
	return 0;
}
//5.

V = 4/3 * pi * r^3

//6.
#include<stdio.h>
int main()
{
     int r;
     float volume_sphere;
     printf("Enter Radius : ");
     scanf("%d",&r);
     volume_sphere = (4/3.0)*3.14*r*r*r;
     printf("\nVolume of Sphere = %f",volume_sphere);
     return 0;
}
//7.
#include<stdio.h>
int main()
{
	float v,r,pi=3.14;
	scanf("%f",&r);
   v= 4*pi*r*r ;
	printf("%f",v);
	return 0;
}
//8.

#include<stdio.h>
int main()
{
	double v,r;
	scanf("%lf",&r);
        v=(4*22*r*r*r)/(7*3); 
	printf("%lf",v);
	return 0;
}
//9.


#include<stdio.h>
int main()
{
	unsigned int  v,r;
	scanf("%u",&r);
        v=(4*22*r*r*r)/(7*3); 
	printf("%u",v);
	return 0;
}
//10.
#include<stdio.h>
int main()
{
	long int  v,r;
	scanf("%ld",&r);
        v=(4*22*r*r*r)/(7*3); 
	printf("%ld",v);
	return 0;
}
//11.

#include<stdio.h>
int main()
{
   	unsigned long int  v,r;
	scanf("%lu",&r);
        v=(4*22*r*r*r)/(7*3); 
	printf("%lu",v);
	return 0;
}
//12.


#include<stdio.h>
int main()
{
   	long double v,r;
	scanf("%Lf",&r);
        v=(4*22*r*r*r)/(7*3); 
	printf("%Lf",v);
	return 0;
}
//13.
#include<stdio.h>
int main()
{
   	unsigned short int  v,r;
	scanf("%hu",&r);
        v=(4*22*r*r*r)/(7*3); 
	printf("%hu",v);
	return 0;
}
//14.
#include<stdio.h>
int main()
{
   	long long int  v,r;
	scanf("%lld",&r);
        v=(4*22*r*r*r)/(7*3); 
	printf("%lld",v);
	return 0;
}
#include<stdio.h>  
 int main()    
{    
int n,d,f,sum=0,sum2=0,sum3=0,a,temp,temp2,temp3,r,j,p;        
scanf("%d",&a);    
temp=n; 
temp2=d;
temp3=f; 
switch (a)
{
case 1:
scanf ("%d",&n);
temp=n; 
while(n>0)    
{    
r=n%10;    
sum=sum+(r*r*r);    
n=n/10;    
}    
if(temp==sum)    
printf("\nArmstrong");    
else    
printf("\nNot Armstrong");
break ;
case 2:
scanf ("%d%d",&n,&d);
temp=n;
temp2=d;
while(n>0)    
{    
r=n%10;    
sum=sum+(r*r*r);    
n=n/10;    
}    
if(temp==sum)    
printf("\nArmstrong");    
else    
printf("\nNot Armstrong"); 
while(d>0)    
{    
j=d%10;    
sum2=sum2+(j*j*j);    
d=d/10;    
}    
if(temp2==sum2)    
printf("\nArmstrong");    
else    
printf("\nNot Armstrong");  
break ;
case 3:
scanf ("%d%d%d",&n,&d,&f);
temp=n; 
temp2=d;
temp3=f; 
while(n>0)    
{    
r=n%10;    
sum=sum+(r*r*r);    
n=n/10;    
}    
if(temp==sum)    
printf("\nArmstrong");    
else    
printf("\nNot Armstrong"); 
while(d>0)    
{    
j=d%10;    
sum2=sum2+(j*j*j);    
d=d/10;    
}    
if(temp2==sum2)    
printf("\nArmstrong");    
else    
printf("\nNot Armstrong");  
while(f>0)    
{    
p=f%10;    
sum3=sum3+(p*p*p);    
f=f/10;    
}    
if(temp3==sum3)    
printf("\nArmstrong");    
else    
printf("\nNot Armstrong");  
break ;}
return 0;  
} 

half pyramid

#include<stdio.h> 
int main() {
   int i, j, n;
   scanf("%d", &n);
   for (i = 1; i <= n; ++i) {
      for (j = 1; j <= i; ++j) {
         printf("*");
      }
      printf("\n");
   }
   return 0;
}


asccending string

#include <stdio.h>
#include<string.h>
int main()
{
  char str[100],temp;
  int i,j;
  scanf("%s",str);
  for(i=0;str[i];i++)
  {
    for(j=i+1;str[j];j++)
    {
      if(str[j]<str[i])
      {
        temp=str[j];
        str[j]=str[i];
        str[i]=temp;
      }
    }
  }
  printf("%s",str);

 return 0;
}

number pattern

#include <stdio.h>
int main()
{
  int i,j,n;
  scanf("%d",&n);
  for(i=1;i<=n;i++)
  {
    for(j=n;j>=1;j--)
    {
      if(i==j)
        printf("*");
      else
        printf("%d",j);
    }
    printf("\n");
  }
  return 0;
}
    

reverse string


#include <stdio.h>
#include<string.h>
int main()
{
  int i,j=0,k=0,len,x;
  char str[100],str1[10][20],temp;
  scanf("%[^\n]s",str);
  
  for(i=0;str[i]!='\0';i++)
  {
    if(str[i] == ' ')
    {
      str1[k][j]='\0';
      k++;
      j=0;
    }
    else
    {
      str1[k][j]=str[i];
      j++;
    }
  }
  str1[k][j]='\0';
  
  for(i=0;i<=k;i++)
  {
    len=strlen(str1[i]);
    for(j=0,x= len - 1; j<x; j++, x--)
    {
      temp=str1[i][j];
      str1[i][j]=str1[i][x];
      str1[i][x]=temp;
    }
  }
  for(i=0;i<=k;i++)
  {
    printf("%s ",str1[i]);
  }
  return 0;
}


smallest vale in an verical orderby adding

#include <stdio.h>
#include<stdlib.h>
int compare(const void *a,const void *b);
int main()
{
  int n,j,t,ans;
  scanf("%d",&t);
  while(t!=0)
  {
    scanf("%d",&n);
    int a[n];
    for(j=0;j<n;j++)
    {
      scanf("%d",&a[j]);
    }
    qsort(a,n,sizeof(int),compare);
    ans=a[0]+a[1];
  
    printf("%d",ans);
    t--;
  }
    return 0;
}
int compare(const void *a,const void *b)
{
  return(*(int*)a-*(int*)b);
}
 


ADDITION OF TWO NUMBERS:

#include <stdio.h>
int main()
{
  int a,b;
  float c,d;
  scanf("%d%d",&a,&b);
  scanf("%f%f",&c,&d);
  printf("The Addition of two number is=%d",a+b);
  printf("\nThe Addition of two number is=%0.1f",c+d);
 return 0;
}

REMOVE LAST OCCURRENCE
#include <stdio.h>
#include<string.h>
int main()
{
  char str[20];
  char ch;
  int i,index,len;
  index=-1;
  scanf("%s%s",&ch,str);
  len=strlen(str);
  for(i=0;i<len;i++)
  {
    if(str[i]==ch)
    {
      index=i;
    }
  }
  if(index!=-1)
  {
    i=index;
    while(i<len)
    {
      str[i]=str[i+1];
      i++;
    }
  }
  printf("%s",str);
 return 0;
}

ARRAY INVERSION:

#include <stdio.h>
int arrinv(int ar[], int a)
{
  int i,j,c=0;
  for(i=0;i<a;i++)
  {
    for(j=i+1;j<a;j++)
    {
      if(ar[i]>ar[j])
        c++;
    }
  }
  return c;
}
        
int main()
{
  int a,i;
  scanf("%d",&a);
  int arr[a];
  for(i=0;i<=a;i++)
  {
    scanf("%d",&arr[i]);
  }
  printf("%d",arrinv(arr,a));

 return 0;
}

APPLE VENDOR
#include <stdio.h>
int main()
{
  int a,b;
  scanf("%d%d",&a,&b);
  printf("%d",a+b);

 return 0;
}
FIND NO OF CHARACTERS IN NAME
#include <stdio.h>
#include<string.h>
struct slen
{
  char str[100];
  int ln;
}s;
int main()
{
  scanf("%s",s.str); 
  s.ln=strlen(s.str);
  printf("%d\n",s.ln); 
  return 0;
}
PRINT THE GIVEN STRING
#include <stdio.h>
int main()
{
  char ch[20];
  char *ptr;
  scanf("%s",ch);
  ptr=ch;
  while(*ptr!='\0')
     printf("%c",*ptr++);

 return 0;
}
SUM OF EVEN AND ODD NUMBERS
#include <stdio.h>
int main()
{
  int a,b,i,even,odd;
  scanf("%d",&a);
  for(i=0;i<a;i++)
  {
    scanf("%d",&b);
    if(b%2==0)
    {
      even=even+b;
    }
    else
    {
      odd=odd+b;
    }
  }
  printf("even=%d",even);
  printf("\nodd=%d",odd);

 return 0;
 }
 
ODD TRIANGLE:

#include <stdio.h>
int main()
{
  int a;
  scanf("%d",&a);
  if(a==1)
    printf("1");
  else if(a==2)
    printf("8");
  else if(a==3)
    printf("27");
  else if(a==4)
    printf("64");
  else if(a==5)
    printf("125");

 return 0;
}
SUM OF FIRST AND LAST:

#include <stdio.h>
int main()
{
  int a,n,f,l;
  scanf("%d",&a);
  scanf("%d",&n);

  
printf("%d",l+n);
 return 0;
}
SQUARE SUM
   #include <stdio.h>
        #define  z  (d3>=0)&&(d3<=100)&&(a3>=0)&&(a3<=100)&&(point[d3][a3]==1)&&(d4>=0)&&(d4<=100)&&(a4>=0)&&(a4<=100)&&(point[d4][a4]==1)
         
        int main()  {
            
            int numcase,I,i,j,n,count,x[500],y[500],point[101][101];
            int d1,d2,d3,d4,a1,a2,a3,a4;
            
            scanf("%d",&numcase);
            for(I=0;I<numcase;I++)  {
                scanf("%d",&n);
                for(i=0;i<=100;i++)
                    for(j=0;j<=100;j++)  point[i][j]=0;
                for(i=0;i<n;i++)  {
                    scanf("%d%d",&x[i],&y[i]);
                    x[i]+=50;
                    y[i]+=50;
                    point[x[i]][y[i]]=1;
                }
                count=0;
                for(i=0;i<n;i++)  {
                    for(j=0;j<n;j++)  {
                        if(i!=j)  {
            
                           d1=x[i],a1=y[i];
                           d2=x[j],a2=y[j];
                           
                           d3=d1+a1-a2;
                           a3=a1+d2-d1;
                           
                           d4=d2+a1-a2;
                           a4=a2+d2-d1;
               
                           
        if(z)
           count++;
             }}}
                printf("%d\n",count/4);
           }
           return 0;
        }   
 


ARRAY PROCESSING:

#include <stdio.h>
int main()
{
  int a[50],n,i,t=0,c=0;
  scanf("%d",&n);
  for(i=0;i<n;i++)
  {
    scanf("%d",&a[i]);
    if(a[i]<0)
    {
      t=t+a[i];
    }
    else
    {
      c++;
    }
  }
  printf("Count of positive numbers=%d\n",c);
  printf("Sum of negative numbers=%d",t);
      

 return 0;
}
MAGIC SQUARE:

#include<stdio.h>
 
int main() {
   int size = 3;
   int matrix[3][3]; // = {{4,9,2},{3,5,7},{8,1,6}};
   int row, column = 0;
   int sum, sum1, sum2;
   int flag = 0;
 
   for (row = 0; row < size; row++) {
      for (column = 0; column < size; column++)
         scanf("%d", &matrix[row][column]);
   }
   sum = 0;
   for (row = 0; row < size; row++) {
      for (column = 0; column < size; column++) {
         if (row == column)
            sum = sum + matrix[row][column];
      }
   }
 
   //For Rows
   for (row = 0; row < size; row++) {
      sum1 = 0;
      for (column = 0; column < size; column++) {
         sum1 = sum1 + matrix[row][column];
      }
      if (sum == sum1)
         flag = 1;
      else {
         flag = 0;
         break;
      }
   }
 
   //For Columns
   for (row = 0; row < size; row++) {
      sum2 = 0;
      for (column = 0; column < size; column++) {
         sum2 = sum2 + matrix[column][row];
      }
      if (sum == sum2)
         flag = 1;
      else {
         flag = 0;
         break;
      }
   }
 
   if (flag == 1)
      printf("\nYes");
   else
      printf("\nNo");
 
   return 0;
}
SYMMETRIC MATRIX USING FUNCTIONS:

#include<stdio.h>
 
int main()
{
  int m, n, c, d, matrix[10][10], transpose[10][10];
 

  scanf("%d%d", &m, &n);
 
  for (c = 0; c < m; c++)
    for (d = 0; d < n; d++)
      scanf("%d", &matrix[c][d]);
 
  for (c = 0; c < m; c++)
    for (d = 0; d < n; d++)
      transpose[d][c] = matrix[c][d];
 
  if (m == n) /* check if order is same */
  {
    for (c = 0; c < m; c++)
    {
      for (d = 0; d < m; d++)
      {
        if (matrix[c][d] != transpose[c][d])
          break;
      }
      if (d != m)
        break;
    }
    if (c == m)
      printf("Symmetric\n");
    else
      printf("Not Symmetric\n");
  }
  else
    printf("Not Symmetric\n");
 
  return 0;
}
GCD AND LCM:

#include <stdio.h>
int main()
{
  int a, b, x, y,temp,GCD,LCM;
  scanf("%d",&x);
  scanf("%d",&y);
  a=x;
  b=y;
  while(b!=0)
  {
    temp=b;
    b=a%b;
    a=temp;
  }
  GCD=a;
  LCM=(x*y)/GCD;
  printf("GCD=%d\n",GCD);
  printf("LCM=%d\n",LCM);
  return 0;
}

#include <stdio.h>
#include<string.h>
int main()
{
  char name[10];
  int n;
  scanf("%s",name);
  n=strlen(name);
  printf("%d",n);
  return 0;
}
LEAP YEAR:

#include <stdio.h>
int main()
{
  int year;
  scanf("%d",&year);
  if(year%4==0)
  {
    printf("Leap Year");
  }
  else
    printf("Not a Leap year");
  return 0;
}

#include <stdio.h>
int main()
{
  int num,r,c;
  scanf("%d",&num);
  for(r=1;num>=r;r++)
  {
    for(c=1;c<=num;c++)
      printf("%d",c);
    
    printf("\n");
  }
  return 0;
}

ARRAY TRANSFORMATION:
#include <stdio.h>
int main()
{
  int t,n,k,a[100],hash[1000],i,ans,x;
  scanf("%d",&t);
  while(t--)
  {
    scanf("%d %d",&n,&k);
    for(i=0;i<1000;i++)hash[i]=0;
    ans=0;
    for(i=0;i<n;i++)
    {
      scanf("%d",&a[i]);
      x=(a[i]%(k+1));
      hash[x]++;
      if(hash[x]>n-2)ans=1;
    }
    if(ans)
      printf("YES\n");
    else
      printf("NO\n");
  }
  return 0;
}
ASCCENDING STRING:

#include <stdio.h>
#include<string.h>
int main()
{
  char str[100],temp;
  int i,j;
  scanf("%s",str);
  for(i=0;str[i];i++)
  {
    for(j=i+1;str[j];j++)
    {
      if(str[j]<str[i])
      {
        temp=str[j];
        str[j]=str[i];
        str[i]=temp;
      }
    }
  }
  printf("%s",str);

 return 0;
}

SQUARE MATRIX:

#include <stdio.h>
#include<math.h>
#include<stdlib.h>
int main()
{
  int n,sum=0,i,j,sum1=0,difference=0;
  scanf("%d",&n);
  int a[100][100];
  for(i=0;i<n;i++)
  {
    for(j=0;j<n;j++)
    {
      scanf("%d",&a[i][j]);
    }
  }
  for(i=0;i<n;i++)
  {
    for(j=0;j<n;j++)
    {
      if(i==j)
        sum=sum+a[i][j];
    }
  }
  for(i=0;i<n;i++)
  {
    for(j=0;j<n;j++)
    {
      if(i==n-j-1)
        sum1=sum1+a[i][j];
    }
  }
  difference=abs(sum-sum1);
  printf("%d",difference);
  return 0;
}

CALCULATING PERCENTAGE:

#include <stdio.h>
int main()
{
  int a,b,c;
  scanf("%d%d%d",&a,&b,&c);
  printf("The gain percentage is=%.2f",((c-a-b)*1.0/(a+b))*100);

 return 0;
}

COMPUTING X
#include<stdio.h>
int main()
{
  float cp,sp,x;
  scanf("%f%f",&cp,&sp);
  x=(cp*100)/(sp+100);
  printf("%.2f",x);
    
 return 0;
}
GROSS SALARY:
#include<stdio.h>
 
int main(){
    int t,n;
    scanf("%d",&t);
    while(t){
        scanf("%d",&n);
        if(n<1500)
            printf("%.0f\n",(float)n*2);
        else
            printf("%.0f\n",(float)n*1.98+500.00);
 
        t--;
    }
 
return 0;
}
TRIANGULAR NUMBERS:

#include <stdio.h>
int triangle(int num)
{
  if (num<0)
    return 0;
  int n,sum;
  for(n=1;sum<num;n++)
  {
    sum=sum+n;
    if(sum==num)
    return 1;
  }
  return 0;
}
int main()
{
  int n;
  scanf("%d",&n);
  if(triangle(n))
    printf("YES");
  else
    printf("NO");
  return 0;
}

GCD AND LCM:

#include <stdio.h>
int main()
{
  int m,a,b,n,d,r,gcd,lcm;
  scanf("%d",&m);
  while(m--)
  {
    scanf("%d %d",&a,&b);
    if(a>b)
    {
      n=a;
      d=b;
    }
    else
    {
      d=a;
      n=b;
    }
    r=n%d;
    while(r!=0)
    {
      n=d;
      d=r;
      r=n%d;
    }
    gcd=d;
    lcm=(a*b)/gcd;
    printf("%d %d\n",gcd,lcm);
  }
  return 0;
}

GREAT CALCULATOR:
#include <stdio.h>
int main()
{
  char a;
  int b,c;
  scanf("%c",&a);
  switch (a)
  {
    case '1':
    scanf("%d %d",&b,&c);
    printf("%d",b+c);
    break;
    case '2':
    scanf("%d %d",&b,&c);
    printf("%d",b-c);
    break;
    case '3':
    scanf("%d %d",&b,&c);
    printf("%d",b*c);
    break;
    case '4':
    scanf("%d %d",&b,&c);
    printf("%d",b/c);
    break;
    default:
      printf("Invalid Input");
  }
    
    

 return 0;
}
MODULE OF NUMBERS
#include <stdio.h>
int main()
{
  int a, b,c; 
  scanf("%d\n%d",&a,&b); 
  c=a%b;
  printf("The modulo of two number is:%d",c);
  

 return 0;
}

TRIANGULAR NUMBERS:
#include <stdio.h>
int triangle(int num)
{
  if (num<0)
    return 0;
  int n,sum;
  for(n=1;sum<num;n++)
  {
    sum=sum+n;
    if(sum==num)
    return 1;
  }
  return 0;
}
int main()
{
  int n;
  scanf("%d",&n);
  if(triangle(n))
    printf("YES");
  else
    printf("NO");
  return 0;
}


GROSS SALARY:
#include <stdio.h>
int main()
{
  float n,i,bs,hra,da;
  float gs;
  scanf("%f",&n);
  for(i=0;i<n;i++)
  {
    scanf("%f",&bs);
    if(bs<1500)
    {
      hra=0.1*bs;
      da=0.9*bs;
      gs=hra+da+bs;
    }
    else if(bs>=1500)
    {
      da=0.98*bs;
      gs=bs+500+da;
    }
    printf("\n%.2f",gs);
  }
  

 return 0;
}
#include <stdio.h>
 

struct employee{
    char    name[30];
    int     empId;
    float   salary;
};
 
int main()
{
 
    struct employee emp;
     

           scanf("%s",emp.name);
             scanf("%d",&emp.empId);
         scanf("%f",&emp.salary);
     
    printf("%s\n"   ,emp.name);
    printf("%d\n"     ,emp.empId);
    printf("%.f\n",emp.salary);
    return 0;
}
#include <stdio.h>
 

struct employee{
    char    name[30];
    int     empId;
    float   salary;
};
 
int main()
{
 
    struct employee emp;
     

           scanf("%s",emp.name);
             scanf("%d",&emp.empId);
         scanf("%f",&emp.salary);
     
    printf("%s\n"   ,emp.name);
    printf("%d\n"     ,emp.empId);
    printf("%.f\n",emp.salary);
    return 0;
}
Array Mode:

#include <stdio.h>
int main()
{
  int a[100],i,j,n,flag=0;
  scanf("%d",&n);
  for(i=0;i<n;i++)
  {
    scanf("%d",&a[i]);
  }
  for(i=0;i<n;i++)
  {
    for(j=i+1;j<n;j++)
    {
      if(a[j]==a[i])
      {
        flag=1;
      printf("Mode=%d ",a[i]);
    }
  }
  }
  if(flag==0)
    printf("none");
 return 0;
}
# include <stdio.h> 
# include <conio.h> 
void main() 
{ 
 int month[12] = {31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31}; 
 char week[7][10] ;
 int date, mon, year, i, r, s = 0 ; 
 clrscr(); 
 strcpy(week[0], "Sunday") ; 
 strcpy(week[1], "Monday") ; 
 strcpy(week[2], "Tuesday") ; 
 strcpy(week[3], "Wednesday") ; 
 strcpy(week[4], "Thursday") ; 
 strcpy(week[5], "Friday") ; 
 strcpy(week[6], "Saturday") ; 
 printf("Enter a valid date (dd/mm/yyyy) : ") ; 
 scanf("%d / %d / %d", &date, &mon, &year) ; 
 if( (year % 400 == 0) || ((year % 4 == 0) && (year % 100 != 0)) ) 
  month[1] = 29 ; 
 for(i = 0 ; i < mon - 1 ; i++) 
  s = s + month[i] ; 
 s = s + (date + year + (year / 4) - 2) ; 
 s = s % 7 ; 
 printf("\nThe day is : %s", week[s]) ; 
 getch() ; 
}



#include <stdio.h>
#include <stdlib.h>

int main()
{
    //1
    int upperLimit;
    int lowerLimit;
    int i,n;

    //2
    printf("Enter the lower limit : \n");
    scanf("%d", &lowerLimit);

    printf("Enter the upper limit : \n");
    scanf("%d", &upperLimit);

    //3
    printf("Five random numbers within %d and %d are :\n", lowerLimit, upperLimit);

    for (i = 1; i < 6; i++)
    {
        n = (rand() % (upperLimit - lowerLimit + 1)) + lowerLimit;
        printf("Number %d : %d\n",i,n);
    }
    return 0;
}



range to print the series


#include<stdio.h>
void main() {
 int num,m,n;
 scanf ("%d %d", &m, &n);
 for (num = m; num <= n; num++) {
   printf("%d ", num);
 }
 getch();
}




arrat mean value
  #include<stdio.h>
int main(){
  int n, a[20], i;
  float min=0;
  scanf("%d",&n);
  for(i=0;i<n;i++)
  {
    scanf("%d",&a[i]);  
    min+=a[i];
  }

  printf("The mean of the array is %.2f",min/n);
  return 0;
}
Array Insertion and sorting:

#include <stdio.h>
 
int main()
{
   int array[100], position,i,temp, c, n, value;
 
   scanf("%d", &n);


   for (c = 0; c < n; c++)
   {
      scanf("%d", &array[c]);
   }
 
  
   scanf("%d", &position);
 

   scanf("%d", &value);
 
   for (c = n - 1; c >= position - 1; c--)
      array[c+1] = array[c];
 
   array[position] = value;
 printf("Before sorting\n");
   for (c = 0; c <= n; c++)
      printf("%d\n", array[c]);
  printf("After sorting\n"); 
  for(c=0;c<n+1;c++)
  {
    for(i=c;i<n+1;i++)
    {
      if(array[c]>array[i])
      {
        temp=array[c];
        array[c]=array[i];
        array[i]=temp;
      }
    }
  }
    for (c = 0; c <= n; c++)
      printf("%d\n", array[c]);
   return 0;
}
Count a String

#include <stdio.h>
 
int main()
{
   char str[100];
   int i, alphabets, digits, special;
   i = alphabets = digits = special = 0;
 
   scanf("%s",str);
   
   while (str[i] != '\0')
   {
    if( (str[i] >= 'a' && str[i] <= 'z') || (str[i] >= 'A' && str[i] <= 'Z') )
    {
     alphabets++;   
   }
    else if (str[i] >= '0' && str[i] <= '9')
    {
     digits++;   
    }    
    else
      special++;
     i++;
 }
    printf("Alphabets=%d", alphabets);  
 printf("\nDigits=%d", digits);  
 printf("\nSpecial characters=%d", special);   
  
   return 0;
}
SWAP 3 NUMBERS IN CYCLIC ORDER:

#include <stdio.h>
void cyclicswap(int *a,int *b,int *c);
int main()
{
  int a,b,c;
  scanf("%d%d%d",&a,&b,&c);
  cyclicswap(&a,&b,&c);
  printf("%d\n%d\n%d\n",a,b,c);
 return 0;
}
void cyclicswap(int *a,int *b,int *c)
{
  int t;
  t=*b;
  *b=*a;
  *a=*c;
  *c=t;
}
FOR LOOP PROCESSING:

#include <stdio.h>
int main()
{
  int n,i,sum=0;
  scanf("%d",&n);
  for(i=1;i<=n;i++)
    {
    sum=sum+i;
  }
  printf ("%d",sum);

 return 0;
}
RECURSIVE FUNCTIONS

#include <stdio.h>
int addnum(int n);
int main()
{
  int num;
  scanf("%d",&num);
  printf("%d",addnum(num));
  return 0;
}
int addnum(int n)
{
  if(n!=0)
    return n+addnum(n-1);
  else
    return n;
}

COUNT THE UPPER AND LOWER CASE

#include <stdio.h>
int main()
{
  int cu=0,cl=0;
  char str[100];
  int counter;
  scanf("%s",str);
  for(counter=0;str[counter]!='\0';counter++)
  {
    if(str[counter]>='A' && str[counter]<='Z')
      cu++;
    else if(str[counter]>='a' && str[counter]<='z')
      cl++;
  }
  printf("Uppercase Letters:%d",cu);
  printf("\nLowercase Letters:%d",cl);
  return 0;
}

COUNT THE UPPER AND LOWER CASE:

CODING ARENA
#include <stdio.h>
int main()
{
  int cu=0,cl=0;
  char str[100];
  int counter;
  scanf("%s",str);
  for(counter=0;str[counter]!='\0';counter++)
  {
    if(str[counter]>='A' && str[counter]<='Z')
      cu++;
    else if(str[counter]>='a' && str[counter]<='z')
      cl++;
  }
  printf("Uppercase Letters:%d",cu);
  printf("\nLowercase Letters:%d",cl);
  return 
}

ARRSUMAVG

#include <stdio.h>
int main()
{
  int n,a[20],i;
  float s=0,sum=0;
  float av;
  scanf("%d",&n);
  for(i=0;i<n;i++)
  {
    scanf("%d",&a[i]);
  }
  for(i=0;i<n;i++)
  {
    if(a[i]>0)
      sum=sum+a[i];
    else 
      if(a[i]<0)
        s=s+a[i];
  }
  av=(s+sum)/n;
  printf("Sum=%.0f",s);
  printf("\nSum=%.0f",sum);
  printf("\nAverage=%.2f",av);

 return 0;
}

BITWISE OPERATOR:

#include <stdio.h>
int main()
{
  int a,b;
  scanf("%d",&a);
  b=a*4;
  printf("%d*4=%d",a,b);
  

 return 0;
}
#include <stdio.h>

int main()
{
    char line[150];
    int i, vowels, consonants, digits, spaces;

    vowels =  consonants = digits = spaces = 0;
    scanf("%[^\n]", line);

    for(i=0; line[i]!='\0'; ++i)
    {
        if(line[i]=='a' || line[i]=='e' || line[i]=='i' ||
           line[i]=='o' || line[i]=='u' || line[i]=='A' ||
           line[i]=='E' || line[i]=='I' || line[i]=='O' ||
           line[i]=='U')
        {
            ++vowels;
        }
        else if((line[i]>='a'&& line[i]<='z') || (line[i]>='A'&& line[i]<='Z'))
        {
            ++consonants;
        }
        else if(line[i]>='0' && line[i]<='9')
        {
            ++digits;
        }
        else if (line[i]==' ')
        {
            ++spaces;
        }
    }

    printf("Vowels:%d",vowels);
    printf("\nConsonants:%d",consonants);
    printf("\nDigits:%d",digits);
    printf("\nWhite spaces:%d", spaces);

    return 0;
}
Test Case 1

Input (stdin)
Chennai 378

Expected Output
Vowels:3

Consonants:4

Digits:3

White spaces:1














SWAP FIRST AND LAST DIGIT
Problem Description

John has a task to swap the first and last digit of the given number. Help him to write a C program to input any number from user and swap the first and last digit of the number
CODING ARENA
#include <stdio.h>
#include <math.h>
int main()
{
  int num,first,count,last,a,b,snum;
  scanf("%d",&num);
  count=log10(num);
  first=num/pow(10,count);
  last=num%10;
  a=first*(pow(10,count));
  b=num%a;
  num=b/10;
  snum=last*(pow(10,count))+(num*10+first);
  printf("%d",snum);

 return 0;
}
Test Case 1

Input (stdin)
12345

Expected Output
52341

















MIRROR PROBLEM
Problem Description

Puck, the trickster, has again started troubling people in your city. The people have turned on to you for getting rid of Puck. 

Puck presents to you a number consisting of numbers from 0 to 9 characters. 

He wants you to count the numbers that he uttered. 

Kindly help people to get rid of the Puck by developing a small program .The hope of people are on you so you have to solve the riddle
CODING ARENA
#include <stdio.h>
int main()
{
  int num,count=0;
  scanf("%d",&num);
  while(num!=0)
  {
    num=num/10;
    count++;
  }
  printf("%d",count);
  return 0;
}
Test Case 1

Input (stdin)
251298

Expected Output
6












CUBE SERIES
Problem Description

Your task is to write a code to find the sum of the following series
13 + 23 + 33 + + n3
Input:
Input should contain the value of the limit n
Output:
It should print the Sum of series upto n limit

CODING ARENA::
#include<stdio.h>
#include<math.h>
int main() {
 int n,i;
 int sum=0;
 scanf("%d",&n);
 sum = pow(((n * (n + 1) ) / 2),2);
 for (i =1;i<=n;i++)
    {
  if (i != n)
               printf("%d^3 + ",i); 
      else
               printf("%d^3=%d",i,sum);
 }
 return 0;
}
  
 
Test Case 1

Input (stdin)
2

Expected Output
1^3 + 2^3=9




ascending elab




  #include <stdio.h>
  int main(){
        int n, p, q;
        int exchange, aray[100];
        scanf("%d", &n);
        for (p=1; p<=n; ++p)
        scanf("%d", &aray[p]);
    
         for (p=1; p<=n-1; ++p){
                          for (q=p+1; q<=n; ++q){
                          if(aray[p] > aray[q])
                         {
                         exchange = aray[p];
                        aray[p] = aray[q];
                        aray[q] = exchange;
                    }}}
         
         for (p=1; p<=n; ++p)
         printf("  %d\n", aray[p]);
         return 0;
         }








d,f
x+3,x-2
a=x+3;
s=x-3;
for (a||a==d,g++,b||a==f)
printf("%d",g)



mark zuckerberg

#include<stdio.h>
int main()
{int n1,n2;
scanf("%d %d",&n1,&n2);
printf("%d\n",n1 & n2);
printf("%d\n",n1 | n2);
printf("%d\n", ~ n1);
printf("%d\n",n1 ^ n2);
printf("%d\n",n1 << 1);
printf("%d\n",n1 >> 1);
return 0;
}

ipll

#include<stdio.h>
int main()
{int arr{3},i;
for (i=0;i<3;i++)
{scanf("%d",&arr[i]);}
printf("%d %o%x",arr[0],arr[1],arr[2]);
return 0;
}

tournament
#include<stdio.h>
int main()
{int n,c=0;
scanf("%d",&n);
while (n>1)
{n=(int) (n/2+n%2);
c+=1;}
printf("%d",c);
return 0;
}







C Program to find sum of series : 1 + 3^2/3^3 + 5^2/5^3 + 7^2/7^3 + … till N terms


#include<stdio.h>
#include<math.h>
 
int main()
{
    int i,N;
    float sum;
    int count;
 
 
    /*read value of N*/
    printf("\nEnter total number of terms :: ");
    scanf("%d",&N);
 
    /*set sum by 0*/
    sum=0.0f;
 
    /*calculate sum of the series*/
    count=1;
    for(i=1;i<=N;i++)
    {
        sum = sum +  ( (float)(pow(count,2)) / (float)(pow(count,3)) );
        count+=2;
    }
 
    /*print the sum*/
 
    printf("\nSum of the series is :: %f\n",sum);
 
    return 0;
}


#include<stdio.h>
int main()
{
int l,t,n;
scanf("%d",%l);
while (l != 0)
{scanf("%d %d",&t,&n);
while (t != 0 )
{n=n*(n+1)/2;
t-=1;
}
printf("%d\n",num);
l-=1;
}return 0;
}









#include<stdio.h>
#include<conio.h>
int main()
{
    int num,num2,num3, fact=1,fact2=1,fact3=1, n,n2,n3,s;
    scanf("%d",&s);
    switch(s)
    {case 1:
    scanf("%d", &num);
    n = num;
    while (num!=0)
    {
        fact = fact*num;
        num = num-1;
    }

    printf("%d\n",fact);

 case 2:
    scanf("%d", &num);
    scanf("%d", &num2);
    n = num;
    while (num!=0)
    {
        fact = fact*num;
        num = num-1;
    }

    printf("%d\n",fact);
    
    n2 = num2;
    while (num2!=0)
    {
        fact2 = fact2*num2;
        num2 = num2-1;
    }

    printf("%d\n",fact2);
    case 3:
    scanf("%d", &num);
    scanf("%d", &num2);
    scanf("%d", &num3);
    n = num;
    while (num!=0)
    {
        fact = fact*num;
        num = num-1;
    }

    printf("%d\n",fact);
    
    n2 = num2;
    while (num2!=0)
    {
        fact2 = fact2*num2;
        num2 = num2-1;
    }

    printf("%d\n",fact2);

    
    n3 = num3;
    while (num3!=0)
    {
        fact3 = fact3*num3;
        num3 = num3-1;
    }

    printf("%d\n",fact3);
}
return 0;
}


https://onlinegdb.com/kfG1eJ7T9


#include<stdio.h>
int main()
{
    int num,num2,num3, fact=1,fact2=1,fact3=1, n,n2,n3,s;
    scanf("%d",&s);
  if ( s == 1 )
 {   scanf("%d", &num);
    n = num;
    while (num!=0)
    {
        fact = fact*num;
        num = num-1;
    }

    printf("%d\n",fact);
}
  else if( s == 2 )
  {
    scanf("%d", &num);
    scanf("%d", &num2);
    n = num;
    while (num!=0)
    {
        fact = fact*num;
        num = num-1;
    }

    printf("%d\n",fact);
    
    n2 = num2;
    while (num2!=0)
    {
        fact2 = fact2*num2;
        num2 = num2-1;
    }

    printf("%d\n",fact2);
  }  
  else if( s == 3 )
  {
    scanf("%d", &num);
    scanf("%d", &num2);
    scanf("%d", &num3);
    n = num;
    while (num!=0)
    {
        fact = fact*num;
        num = num-1;
    }

    printf("%d\n",fact);
    
    n2 = num2;
    while (num2!=0)
    {
        fact2 = fact2*num2;
        num2 = num2-1;
    }

    printf("%d\n",fact2);

    
    n3 = num3;
    while (num3!=0)
    {
        fact3 = fact3*num3;
        num3 = num3-1;
    }

    printf("%d\n",fact3);
}
return 0;
}








#include<stdio.h>
int main()
{ int a,b,i=0,n;
scanf("%d",&n);
for (i=0;i<n;i++)
{scanf("%d %d",&a,&b);
if(a<b)
printf("<\n";
else if(a<b)
printf(">\n);
else
printf("=\n");
}return 0;
}


#include <stdio.h>
int main()
{while (1)
{int num;
scanf("%d",num);
if(num == 42)
{break;}
else
{printf("%d\n",num)
}
}
return 0;
}


#include <stdio.h>
int main()
{floata,m;
int ar;
scanf("%f %f %d",&a,&m,&ar);
if((a>90.0)&&(m>90.0)&&ar==0)
{printf("Eligible");}
else
printf("Not Eligible");
return 0;
}


#include <stdio.h>
int main()
{
int t,n,k;
scanf("%d",&t);
int i=0,j=0,max=0;
for(i=0;i<t;i++)
{scanf("%d%d",&n,&k);
for(j=1;j<=k;j++)
{
if((n%j)>max)
{max=n%j;
}}
printf("%d\n",max);
max=0;}
return 0;
}



42.

#include<stdio.h>

int main()
{const int maxn = 100007;
int a[maxn],n;
long long b[maxn];
    scanf("%d",&n);
    long long sum = 0;
    for(int i=1;i<=n;i++)
        scanf("%d",&a[i]);
    for(int i=n;i>=1;i--)
    {
        sum*=-1;
        b[i]=a[i]-sum;
        sum+=b[i];
    }
    for(int i=1;i<=n;i++)
        printf("%lld ",b[i]);
    printf("\n");
return 0;
    
}





 #include<stdio.h>
struct Student{
union  {
        char name[20];
   
         };
         int english;
         int maths;
         int science;
         int ss;
        int tamil;
    };

 
int main() {
    struct Student stud;
    
        scanf("%s",stud.name);
        scanf("%d",&stud.english);
        scanf("%d",&stud.tamil);
        scanf("%d",&stud.maths);
        scanf("%d",&stud.science);
        scanf("%d",&stud.ss);
      printf("Details of student");  
     printf("\nName of the student=%s",stud.name);   
    printf("\nTamil=%d",stud.tamil);
    printf("\nEnglish=%d",stud.english);
     printf("\nMaths=%d",stud.maths);
     printf("\nScience=%d",stud.science);
     printf("\nSocial Science=%d",stud.ss);
  return 0;
}

#include <stdio.h>

int main() {
 union Student
{char name[50];
           int tamil;
           int english;
           int maths;
           int science;
           int ss;
           };
    union Student s1;
            scanf("%s",s1.name);
            scanf("%d%d%d%d%d",&s1.tamil,&s1.english,&s1.maths,&s1.science,&s1.ss);
            
	printf("Details of student\nName of the student=%s\n",s1.name);	
            printf("Tamil=%d\nEnglish=%d\nMaths=%d\nScience=%d\nSocial Science=%d",&s1.tamil,&s1.english,&s1.maths,&s1.science,&s1.ss);
            return 0;
}

#include <stdio.h>
union Student
{char name[50];
           int tamil;
           int english;
           int maths;
           int science;
           int ss;
           int s1
           };
int main() {union Student s1;
       printf("%d",sizeof(s1));
            return 0;
}
