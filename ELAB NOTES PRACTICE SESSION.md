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





https://onlinegdb.com/rJnztlYsw

//to find the cube of number 
#include <stdio.h>

int main()
{
    int a,b;
    scanf("%d",&a);
    b=a*a*a;
    printf("CUBE is: %d",b);
   return 0;
}


https://onlinegdb.com/ryQr1-Kow
//power elab

printf("Difference between %dand %dis = %d",a,b,c);


#include <math.h>
#include <stdio.h>
int main()
{
    int a,b,c;
    scanf("%d%d",&a,&b);
    c=pow(a,b);
    printf("%d",a);
    printf(" to the power of ");
    printf("%d",b);
    printf(" is= %d",c);
    return 0;
}



theater square

#include <stdio.h>
#include <math.h>
 
int main() {
    float m, n, o;
    int p, q, r;
    scanf("%f %f %f", &m, &n, &o);
    p = ceil(m / o);
    q = ceil(n / o);
    r = p*q;
    printf("%d", r);
    return (0);
}

2.56 =70.240616
3.1=124.724983

//volume of sphere 1
int main()
{
	float v,r;
	scanf("%f",&r);
        v=(4*22*r*r*r)/(7*3); 
	printf("%f",v);
	return 0;
}
70.304527 

//2.
#include<stdio.h>
int main()
{
	float v,r;
	scanf("%f",&r);
        v=(4*3.14*r*r*r)/(3); 
	printf("%f",v);
	return 0;
}
 70.240608

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

70.304527 

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

33.493332 

//7.
#include<stdio.h>
int main()
{
	float v,r,pi=3.14;
	scanf("%f",&r);
   v= 4*pi*r*r ;
	printf("%f",v);
	return 0;
}82.313210


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
33

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

33

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

33

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


70.304524      

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

33

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




armstrong number
https://onlinegdb.com/Sy5tvy0jP

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
 


ADDITION OF TWO NUMBERS
Harinis home work for the second day is to subtract two numbers, help Harini to solve the proble

CODING ARENA
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


INDIA VS ENGLAND
Problem Description

Virat Kohli has won the toss against England in a 50 Over World Cup Final 2019. During the Toss time the commentator have him a funny task to test his mathematical skills. 

Shastri was the umpire to judge his mathematical skills. When the number is 23 he needs tell "INDIA" and when the number is 50 he needs to tell "ENGLAND".

When the number is less than "0" he needs to tells as "Sorry". Help our cricket captain by writing a sample program.

Refer sample Input and Output:
Input 1: 204 Output: ENGLAND
Input 2: 219 Output: INDIA 
Input 3: 2228 Output: ENGLAND
Input 4: -1 Output: Sorry
CODING ARENA
#include <stdio.h>
int main()
{
  int a;
  scanf("%d",&a);
  if(a>0)
  {
    if(a%2==0)
       printf("ENGLAND");
    else if(a%2!=0)
       printf("INDIA");
  }
  else 
    printf("Sorry");
 return 0;
}
Test Case 1

Input (stdin)
2056

Expected Output
ENGLAND




REMOVE LAST OCCURRENCE
Problem Description

Write a C program to read any string from user and remove the last occurrence of a given character from the string.
CODING ARENA
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

Test Case 1

Input (stdin)
a

madam

Expected Output
madm




ARRAY INVERSION
Problem Description

Number of an inversion in array is the number of pair(a[i],a[j]) of elements such that i < j and a[i] > a[j]. For an example if we have a list of element 2 3 6 9 1 then number of inversion is 4 and the pairs are (2,1), (3,1), (6,1) and (9,1).
Input:
The first line is N, N is the size of array.
The second line contains N input C[i].
CODING ARENA::
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
Test Case 1

Input (stdin)
5

2 3 6 9 1

Expected Output
4



APPLE VENDOR
Problem Description

Helen wants to find the sum of apples in 2 baskets that she is carrying to the market. You need to write a C program to help her find the total number of apples. Use functions in C to write this program.
CODING ARENA::
#include <stdio.h>
int main()
{
  int a,b;
  scanf("%d%d",&a,&b);
  printf("%d",a+b);

 return 0;
}
Test Case 1

Input (stdin)
2 3

Expected Output
5



FIND NO OF CHARACTERS IN NAME
Problem Description

Manoj arranged one event to find no of characters in his friends name, your idea is to give your friends name, for that
manoj has to answer the no of characters present in it, with the help of sturcuture concept accomplish it.

Input Method

Name of different friends 

Output Method

No of characters

Use Structure Concepts

CODING ARENA
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
Test Case 1

Input (stdin)
raja

Expected Output
4



ASCII NAME
Problem Description

Write a program which reads your name from the keyboard and output a list of ANCII codes, which represent your name
CODING ARENA
#include <stdio.h>
int main(void)
{
  char n[20];
  int i=0;
  scanf("%s",n);
  while(n[i]!='\0')
  {
    printf(" %d",n[i]); i++;
  }
  return (0);
}
Test Case 1

Input (stdin)
SRMUNIVERSITY

Expected Output
83 82 77 85 78 73 86 69 82 83 73 84 89 



PRINT THE GIVEN STRING
Problem Description

Print a string using Pointer
CODING ARENA::
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
Test Case 1

Input (stdin)
Cse

Expected Output
Cse


SUM OF EVEN AND ODD NUMBERS
Problem Description

Write a program to find the sum of even and odd numbers in an array.

Input Format:

Input consists of n+1 integers. The first integer corresponds to n , the size of the array. The next n integers correspond to the elements in the array. Assume that the maximum value of n is 15.

Output Format:

Refer sample output for details.
CODING ARENA
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
Test Case 1

Input (stdin)
5

2 3 6 8 3

Expected Output
even=16

odd=6
Test Case 2



ODD TRIANGLE
Problem Description

"Given the triangle of consecutive odd numbers:

1
3 5
7 9 11
13 15 17 19
21 23 25 27 29
...
Calculate the row sums of this triangle from the nth row index (starting at row index 1)."
CODING ARENA::
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
Test Case 1

Input (stdin)
1

Expected Output
1



SUM OF FIRST AND LAST
Problem Description

If Give an integer N . Write a program to obtain the sum of the first and last digit of this number. The first line contains an integer T, total number of test cases. Then follow T lines, each line contains an integer N. Display the sum of first and last digit of N.
CODING ARENA::
#include <stdio.h>
int main()
{
  int a,n,f,l;
  scanf("%d",&a);
  scanf("%d",&n);

  
printf("%d",l+n);
 return 0;
}
Test Case 1

Input (stdin)
1

1234

Expected Output
5


SQUARE SUM
Problem Description

"Everyone knows what a square looks like. Mathematically, a square is a regular quadrilateral. This means that it has four equal sides and four equal angles (90 degree angles).

One beautiful day, Johnny eagerly examined the interesting properties of squares. He did not forget you, his best friend and a talented programmer and thus made a problem about squares to challenge your programming ability. The problem is: given a set of N points in the plane, how many squares are there such that all their corners belong to this set?

Now let's show Johnny your skill!
Input

The first line contains t, the number of test cases (about 10). Then t test cases follow.

Each test case has the following form:

The first line contains an integer N, the number of points in the given set (4 <= N <= 500).
Then N lines follow, each line contains two integers X, Y describing coordinates of a point (-50,= X, Y <= 50).

Output

For each test case, print in a single line the number of squares that have vertices belong to the given set."
CODING ARENA::
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
 


ARRAY PROCESSING
Problem Description

Return an array, where the first element is the count of positives numbers and the second element is sum of negative numbers.
If the input array is empty or null, return an empty array:
CODING ARENA::
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
Test Case 1

Input (stdin)
15

1 2 3 4 5 6 7 8 9 10 -11 -12 -13 -14 -15

Expected Output
Count of positive numbers=10

Sum of negative numbers=-65



MAGIC SQUARE
Problem Description

A magic square is an arrangement of numbers (usually integers) in a square grid, where the numbers in each row, and in each column, and the numbers in the forward and backward main diagonals, all add up to the same number


Input Format:

The input consists of (n*n+1) integers. The first integer corresponds to the number of rows/columns in the matrix. The remaining integers correspond to the elements in the matrix. The elements are read in rowwise order, first row first, then second row and so on. Assume that the maximum value of m and n is 5.


Output Format:
Print yes if it is a magic square. Print no if it is not a magic square
CODING ARENA::
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
 
 
   //For diagonal elements
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
Test Case 1

Input (stdin)
4 9 2

3 5 7

8 1 6

Expected Output
Yes




SYMMETRIC MATRIX USING FUNCTIONS
Problem Description

Create a function called symmetric() and perform the following

A symmetric matrix is a square matrix that is equal to its transpose.

Write a C program to find whether a given matrix is a square matrix or not.
Input Format:

The input consists of (m*n+2) integers. The first integer corresponds to m, the number of rows in the matrix and the second integer corresponds to n, the number of columns in the matrix. The remaining integers correspond to the elements in the matrix. The elements are read in rowwise order, first row first, then second row and so on. Assume that the maximum value of m and n is 10

CODING ARENA::
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




GCD AND LCM
Problem Description

Two integers A and B are the inputs. Write a program to find GCD and LCM of A and B.

Input: each line contains an integer A and B.

Output: Display the GCD and LCM of A and B separated by space respectively
CODING ARENA
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
  
Test Case 1

Input (stdin)
30 40

Expected Output
GCD=10

LCM=120



TWOS MOD
Problem Description

Bheem has two numbers, he wants to know the modulous value of those two numbers.
Your task is to write a c Program to calculate the modulus of two given numbers.Input the negative numbers and view the output for different test cases
CODING ARENA
#include <stdio.h>
int main()
{
  int a,b,c;
  scanf("%d%d",&a,&b);
  c=a%b;
  printf("%d",c);
  return 0;
}
Test Case 1

Input (stdin)
100 93

Expected Output
7


LENGTH OF THE STRING
Problem Description

Program which will accept string from the user and find the length of the string
CODING ARENA
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
Test Case 1

Input (stdin)
welcome

Expected Output
7





LEAP YEAR

Problem Description

Raghuraman is the worrisome as well as caring father of his only daughter bharani ,together they live a calm and content life. Over the years as Bharani grows up , Raghuramam got more and more attached to his daughter bharani. As bijarani is very intelligent and bright in her studies. She got a good placement offer in canada. Raghuraman was shocked.Although the thought of being separated from his dead daughter is heartbreaking. Raghuraman wearily accepts. Bharani promises her that she will come home once every leap year. Raghuraman was waiting for his daughter arrival. He doesnt know which is leap year. So write a C program to help Raghumaran to find a whether the year is a leap year.

Input format:

Input consists of single integer which corresponds to a year

Output format :

Displays whether the given year is a leap year or not.

Refer sample input and output for further formatting specifications.
CODING ARENA
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
Test Case 1

Input (stdin)
2004

Expected Output
Leap Year




PATTERN 6
Problem Description

Write a program to generate a following numbers structure
CODING ARENA
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
Test Case 1

Input (stdin)
5

Expected Output
12345

12345

12345

12345

12345







ARRAY TRANSFORMATION

Problem Description

"Given n numbers, you can perform the following operation any number of times : Choose any subset of the numbers (possibly empty), none of which are 0. Decrement the numbers in the subset by 1, and increment the numbers not in the subset by K.

Is it possible to perform operations such that exactly n - 1 numbers become 0 ?
CODING ARENA
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

 
Test Case 1

Input (stdin)
3

2 1

10 10

3 2

1 2 2

3 2

1 2 3

Expected Output
YES

YES

NO




ASCCENDING STRING
Problem Description

Code for Sort given string in ascending order
CODING ARENA
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
Test Case 1

Input (stdin)
sample

Expected Output
aelmps




SQUARE MATRIX

Problem Description

Given a square matrix of size NN, calculate the absolute difference between the sums of its diagonals. 

Input
The first line contains a single integer N. The next N lines denote the matrix's rows, with each line containing N space-separated integers describing the columns.

Output
Print the absolute difference between the two sums of the matrix's diagonals as a single integer.

Constraints
1<=N<=10

Explanation
The primary diagonal is: 
11
5
-12
Sum across the primary diagonal: 11 + 5 - 12 = 4
The secondary diagonal is:
4
5
10

Sum across the secondary diagonal: 4 + 5 + 10 = 19 
Difference: |4 - 19| = 15
CODING ARENA
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
Test Case 1

Input (stdin)
3

11 2 4

4 5 6

10 8 -12

Expected Output
15





CALCULATING PERCENTAGE
Problem Description

SRM University buys an old scooter for Rs. A and Spends Rs. B on its repairs. if he sells the scooter for Rs.C , what is his gain %? Write C program to compute the gain %?

Input format:

The first input is an integer which corresponds to A . The second input is an integer which corresponds to B. The third input is a float which corresponds to gain $
CODING ARENA
#include <stdio.h>
int main()
{
  int a,b,c;
  scanf("%d%d%d",&a,&b,&c);
  printf("The gain percentage is=%.2f",((c-a-b)*1.0/(a+b))*100);

 return 0;
}
Test Case 1

Input (stdin)
4700

800

5800

Expected Output
The gain percentage is=5.45



COMPUTING X
Problem Description

The cost prince of n articles is the same as the selling price of X articles . If the profit is p% then what is the value of x?

Input format:

The first input is an integer which corresponds to n the second is an integer which corresponds to p

Output Formt:

Refer sample Input and output for formatting Specifications

The float values are displayed correct to 2 decimal places.
CODING ARENA
#include<stdio.h>
int main()
{
  float cp,sp,x;
  scanf("%f%f",&cp,&sp);
  x=(cp*100)/(sp+100);
  printf("%.2f",x);
    
 return 0;
}
Test Case 1

Input (stdin)
12.5

14.5

Expected Output
10.92




GROSS SALARY
Problem Description

In a company an emplopyee is paid as under: If his basic salary is less than Rs. 1500, then HRA = 10% of base salary and DA = 90% of basic salary.

If his salary is either equal to or above Rs. 1500, then HRA = Rs. 500 and DA = 98% of basic salary. 

If the Employee's salary is input, write a program to find his gross salary.

NOTE: Gross Salary = Basic Salary+HRA+DA

Input

The first line contains an integer T, total number of testcases. Then follow T lines, each line contains an integer salary.

Output

Output the gross salary of the employee.

Constraints
1 < T< 1000
1< salary < 100000
CODING ARENA
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
}TRIANGULAR NUMBERS
Problem Description

"A triangular number is the number of dots in an equilateral triangle uniformly filled with dots. For example, three dots can be arranged in a triangle; thus three is a triangular number. The n-th triangular number is the number of dots in a triangle with n dots on a side. . You can learn more about these numbers from Wikipedia (http://en.wikipedia.org/wiki/Triangular_number).
Your task is to find out if a given integer is a triangular number.
Input
The first line contains the single number n (1<n<500) the given integer.
Output
If the given integer is a triangular number output YES, otherwise output NO.
"
CODING ARENA
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
 
Test Case 1

Input (stdin)
3

1400

2500

3000

Expected Output
2800

5450

6440



GCD AND LCM
Problem Description

Two integers A and B are the inputs. Write a program to find GCD and LCM of A and B.
Input

The first line contains an integer T, total number of testcases. Then follow T lines, each line contains an integer A and B.
Output

Display the GCD and LCM of A and B separated by space respectively.
Constraints

1 <= T<= 1000
1 <= A,B <= 1000000
CODING ARENA
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
Test Case 1

Input (stdin)
5

2 3

2 4

3 5

4 6

7 8

Expected Output
1 6

2 4

1 15

2 12

1 56





GREAT CALCULATOR
Problem Description

SRM Students decides to create a software to extend our help to Petty shops and Shops. In this regard the "STUDENT" team has selected a few students to complete the task. The task was monitored by a group of experts and the software was tested by a expert team from corporate.

The task is as follows when there are two items and if the shop keeper says 1 then it needs to add the two items. If the shop keeper yells 2 then the two items should be subtracted. And when the shop keeper tells 3 then the product of the items needs to be outputted. When shop keeper tells as 4 then the items should fight with one another.

Only Integer numbers as input

Input 1 = addition
Input 2 = Substraction
Input 3 = Multiplication
Input 4 = Division
CODING ARENA
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
Test Case 1

Input (stdin)
1

35 36

Expected Output
71


MODULE OF NUMBERS
Problem Description

Harinis home work for fifth day is to find reminder of two numbers, help Harini to solve the problem.
CODING ARENA
#include <stdio.h>
int main()
{
  int a, b,c; 
  scanf("%d\n%d",&a,&b); 
  c=a%b;
  printf("The modulo of two number is:%d",c);
  

 return 0;
}
Test Case 1

Input (stdin)
6

2

Expected Output
The modulo of two number is:0



TRIANGULAR NUMBERS
Problem Description

"A triangular number is the number of dots in an equilateral triangle uniformly filled with dots. For example, three dots can be arranged in a triangle; thus three is a triangular number. The n-th triangular number is the number of dots in a triangle with n dots on a side. . You can learn more about these numbers from Wikipedia (http://en.wikipedia.org/wiki/Triangular_number).
Your task is to find out if a given integer is a triangular number.
Input
The first line contains the single number n (1<n<500) the given integer.
Output
If the given integer is a triangular number output YES, otherwise output NO.
"
CODING ARENA
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


GROSS SALARY
Problem Description

" In a company an emplopyee is paid as under: If his basic salary is less than Rs. 1500, then HRA = 10% of base salary and DA = 90% of basic salary.
If his salary is either equal to or above Rs. 1500, then HRA = Rs. 500 and DA = 98% of basic salary. If the Employee's salary is input, write a program to find his gross salary.

NOTE: Gross Salary = Basic Salary+HRA+DA
Input

The first line contains an integer T, total number of testcases. Then follow T lines, each line contains an integer salary.
Output

Output the gross salary of the employee.
Constraints

1 <= T <= 1000
1 <= salary <= 100000
CODING ARENA::
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
Test Case 1

Input (stdin)
3

1203

10042

1312

Expected Output
2406.00

20383.16

2624.00




Problem Description

1. Create a Structure called "employee"

2. Create three data members as name(char), empid(int), salary(float)

3. Input the value of employee's (name, empid and salary)

4. Create Structure Variable as "emp"

5. Display using structure variable.datamember

Hint:
emp.name

Note: The structure variables, data members and structure name are CASE Sensitive.

Follow the same case mentioned in the mandatory
CODING ARENA
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
Test Case 1

Input (stdin)
Bogar

1122

15000

Expected Output
Bogar

1122

15000





Static Structure - Employee
Problem Description

1. Create a Structure called "employee"

2. Create three data members as name(char), empid(int), salary(float)

3. Input the value of employee's (name, empid and salary)

4. Create Structure Variable as "emp"

5. Display using structure variable.datamember

Hint:
emp.name

Note: The structure variables, data members and structure name are CASE Sensitive.

Follow the same case mentioned in the mandatory
CODING ARENA
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
Test Case 1

Input (stdin)
Bogar

1122

15000

Expected Output
Bogar

1122

15000




Array Mode
Problem Description

Write a program to find the mode of the elements in the array.

The mode in a list of numbers refers to the list of numbers that occur most frequently. It is important to note that there can be more than one mode and if no number occurs more than once in the set, then there is no mode for that set of numbers.



Input and Output Format:

Input consists of n+1 integers where n corresponds to the number of elements in the array.

The first integer corresponds to n and the next n integers correspond to the elements in the array.

Refer sample input and output for formatting specifications.

Assume that the maximum number of elements in the array is 20.

Assume that in the input dataset there is 1 mode or no mode at all.

All text in bold corresponds to input and the rest corresponds to output.
CODING ARENA
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
Test Case 1

Input (stdin)
5

2 4 2 3 5

Expected Output
Mode=2



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



Array Mean
Problem Description

Write a program to find the mean of the elements in the array.


Input and Output Format:

Input consists of n+1 integers where n corresponds to the number of elements in the array.

The first integer corresponds to n and the next n integers correspond to the elements in the array.

Output consists of a double value which corresponds to the mean of the array. It is printed upto 2 digits of precision.

Assume that the maximum number of elements in the array is 20.

Refer sample input and output for formatting specifications.

All text in bold corresponds to input and the rest corresponds to output.
CODING ARENA
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
Case 1

Input (stdin)
5

2

4

1

3

5

Expected Output
The mean of the array is 3.00



Array Insertion and sorting
Problem Description

Write a program to insert an element in the array.


Example

For example consider an array having three elements in it initially and a[0] = 1, a[1] = 2 and a[2] = 3 and you want to insert a number 45 at location 1 i.e. a[0] = 45, so we have to move elements one step below so after insertion a[1] = 1 , and a[2] = 2 and a[3] = 3.


Input and Output Format:

Assume that the maximum number of elements in the array is 20.

Refer sample input and output for formatting specifications.

All text in bold corresponds to input and the rest corresponds to output.
CODING ARENA
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
Test Case 1

Input (stdin)
5

9 6 3 2 7

1

10

Expected Output
Before sorting

9

10

6

3

2

7

After sorting

2

3

6

7

9

10




Count a String
Problem Description

Write a C program to count total number of alphabets, digits or special characters in a string using loop. How to find total number of alphabets, digits and special characters in a string in C programming.
CODING ARENA
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
Test Case 1

Input (stdin)
SRM!University@Learning&Centre@1113

Expected Output
Alphabets=27

Digits=4

Special characters=4




SWAP 3 NUMBERS IN CYCLIC ORDER
Problem Description

Ramya, vidhya and Ramesh are always changing their places in cyclic manner. Can you write a code using methods(functions) to read 3 numbers and swap them using a temporary variable in a cyclic manner. Print the results in the specified order.
CODING ARENA
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
Test Case 1

Input (stdin)
1 2 3

Expected Output
3

1

2
Tes



FOR LOOP PROCESSING
Problem Description

Program to calculate the sum of first n natural numbers
CODING ARENA::
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
Problem Description

Write a C program for Sum of Natural Numbers Using Recursion.
CODING ARENA
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
Problem Description

Count Total number of Capital and Small Letters from Accepted Linen
Note: (No spaces between words)
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
  return 0;
}
Test Case 1

Input (stdin)
SRMUn

Expected Output
Uppercase Letters:4

Lowercase Letters:1









COUNT THE UPPER AND LOWER CASE
Problem Description

Count Total number of Capital and Small Letters from Accepted Linen
Note: (No spaces between words)
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
Test Case 1

Input (stdin)
SRMUn

Expected Output
Uppercase Letters:4

Lowercase Letters:1








ARRSUMAVG
Problem Description

Calculate Sum & Average of an Array

Assign the maximum size value is 10
CODING ARENA
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
Test Case 1

Input (stdin)
6

-8 9 -100 0 6 5

Expected Output
Sum=-108

Sum=20

Average=-14.67

















BITWISE OPERATOR
Problem Description

Kernel had an idea to use bitwise operator. He tries to do some multiplication operation. So he select a nu mber that should be multiplied by 4. His task is to write a c program to multiply given number by 4 using bitwise operators
CODING ARENA
#include <stdio.h>
int main()
{
  int a,b;
  scanf("%d",&a);
  b=a*4;
  printf("%d*4=%d",a,b);
  

 return 0;
}
Test Case 1

Input (stdin)
1

Expected Output
1*4=4








Count Vowels
Problem Description

Program to count vowels, consonants,digits and whitespaces
CODING ARENA
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
