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
     
**HELLO EVERYONE THERE IS LESS QUESTIONS IN SESSION 9 PLZZ DONATE SOME CODE**
