**1). INCREMENT USING POINTERS**

        #include <stdio.h>
        int main() 
        {
        int a, b, c;
        scanf("%d%d%d", &a, &b, &c);
        int *ptr[3] = {&a, &b, &c};
        printf("value of a: %d, b: %d, c: %d", *ptr[0], *ptr[1], *ptr[2]);
        *ptr[0] +=10;
        *ptr[1] +=10;
        *ptr[2] +=10;
        printf("\nAfter adding 10\nvalue of a: %d, b: %d, c: %d", *ptr[0], *ptr[1], *ptr[2]);
        return 0;
        }
 **2)DHONI AND SHANE WATSON**
 
        #include <stdio.h>
        #include <string.h>
        void RevString(char *ptr, int num)
     {
         while (num > 0)
         {
                printf("%c",*ptr);
                ptr--;
                num--;
        }
        return;
        }
        int main()
        {
                int lines;
                scanf("%d", &lines);
                while (lines != 0 ){
                char str[2000];
                scanf("%s", str);
                char * token = strtok(str, ".");
                int len = strlen(token);
                char *ptr = &token[len-1];
                RevString(ptr, len);
                while (token != NULL)
                {
                        token = strtok(NULL, ".");
                        if( token != NULL)
                        {
                                printf(".");
                                len = strlen(token);
                                char *ptr = &token[len-1];
                                RevString(ptr, len); 
                        }
                }
                printf("\n");
                lines -= 1;
        }
        return 0;
      }
  **3). Change constant value using pointer**
  
             #include <stdio.h>
             int main()
             {
                const int a = 10;
                const int *p;
                p = &a;
                printf("Before changing -constant value of a:%d\n",a);
                scanf("%d",p);
                printf("After changing - value of a:%d\n",a);
                return 0;
             }
 **4). Interchange num**
 
                #include <stdio.h>
                void interchange (int *num1, int *num2)
                {
                        int temp;
                        temp = *num1;
                        *num1 = *num2;
                        *num2 = temp;
                        printf("%d %d", *num1, *num2);
                        return;
                }
  **5). Amelia's Game
  
                #include <stdio.h>
                int main()
                {
                        int lines;
                        scanf("%d", &lines);
                        if (lines < 0 || lines > 10000)
                        {
                                printf("INVALID INPUT");
                                return 0;
                        }
                        else 
                        {
                                 while (lines != 0){
                                 int num;
                                 scanf("%d", &num);
                                 if (num < 0 || num > 100)
                                 {
                                        printf("INVALID INPUT");
                                        return 0;
                                 }
                                 int i, arr[num];
                                 int *ptr = &arr[0];
                                 for (i=0; i < num; i++)
                                 {
                                        scanf("%d", ptr);
                                        if (*ptr % 3 == 0)
                                        {
                                                printf("%d\n", *ptr);
                                        }
                                 }
                                 lines--;
                         }
                       }
                        return 0;
                     }
   **6). Internet protocol addressing**
   
            #include <stdio.h>
            #include <string.h>
            #include <stdlib.h>
            #define DELIM "."
            int valid_digit(char *ip_str) 
            {
                while (*ip_str) 
                {
                        if (*ip_str >= '0' && *ip_str <= '9')
                        ++ip_str;
                         else
                        return 0;
                }
                return 1;
            }
            int is_valid_ip(char *ip_str)
             {
                int i, num, dots = 0;
                char *ptr;
                if (ip_str == NULL)
                return 0;
                ptr = strtok(ip_str,DELIM);
                if (ptr == NULL)
                return 0;
                while (ptr) 
                {
                 if (!valid_digit(ptr))
                 return 0;
                 num = atoi(ptr);
                 if (num >= 0 && num <= 255) 
                 {
                        ptr = strtok(NULL, DELIM);
                        if (ptr != NULL)
                        ++dots;
                }
                else
                return 0;
                }
                if (dots !=3)
                return 0;
                return 1;
              }
                int main()
                {int t,i;
                char ip_str[50];
                //scanf("%s",ip_str);
                scanf("%d",&t);
                LOOP :do
                {
                if ( t != 0 )
                {
                        scanf("%s",ip_str);
                        is_valid_ip(ip_str)? printf("Valid\n"): printf("Not valid\n");
                        t=t-1;
                        goto LOOP;
                 }
             }while(t>0);
             return 0;
           }
   **7). Vijay's House**
   
        #include <stdio.h>
        void rect(int a,int b,int * area,int * perim)
        {}
        int main()
        {
        int x, y, Area, Perimeter;
        int *ptrx = &x ;
        int *ptry = &y;
        scanf("%d %d", ptrx, ptry );
        Area = *ptrx * *ptry;
        Perimeter= 2*(*ptrx + *ptry);
        printf("%d" , Area);
        printf(" %d", Perimeter);
        return 0;
        }
  **8). Reality show**
  
        #include <stdio.h>
        int main()
        {
        int i, j, a, n, number[30];
        scanf("%d", &n);
        for (i = 0; i < n; ++i)
        scanf("%d", &number[i]);
        for (i = 0; i < n; ++i)
        {for (j = i - 1; j > n; --j)
        {if (number[i] > number[j])
        {a = number[i];
        number[i] = number[j];
        number[j] = a; }}}
        for (i = 0; i < n; ++i)
        printf("%d ", number[i]);                                
        return 0;
        }
