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
                        sum= sum + ( (float) (pow (count, 2)) / (float) (pow (count,3)));
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

**   **
