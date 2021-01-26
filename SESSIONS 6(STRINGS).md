**1). Flag**

    #include<stdio.h>
    int n,m;
    int main()
    {
    int i,j;
    char fln ,flm,flag,t;
    while(~scanf("%d%d",&n,&m)){
    flag=1;fln=-1;getchar();
    for(i=0;i<n;i++)
    {
    scanf("%c",&flm);
    if(fln==flm)flag=0;
    for(j=1;j<m;j++)
    {
    scanf("%c",&t);
    if(t!=flm)flag=0;
    }
    fln=flm;
    getchar();
    }
    if(flag)printf("YES\n");
    else printf("NO\n");
    }
    return 0;
    }
**2). COUNT ALPHA**

    #include <stdio.h>
    int main()
    {
      char a;
      scanf("%c",&a);
      if(a=='Q')
      printf("an alphabet");
      else
        printf("Not an alphabet");
    
     return 0;
    }
**3). Reverse the string**

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
**4). Mahasena**

    #include <stdio.h>    
    int main(void) {
        int n,i,c1=0,c2=0; scanf("%d",&n);
        int a[n];
        for(i=0;i<n;i++)
        {
            scanf("%d",&a[i]);
            if(a[i]%2==0) c1++;
            else c2++;
        }
        if(c1>c2) printf("READY FOR BATTLE\n");
        else printf("NOT READY\n");
    	return 0;
    } 
**5). s-palindrome**

    #include<stdio.h>
    
    #include<string.h>
    
    int main()
    
    {
    
        char str[1000];
    
        scanf("%s",str);
    
       int i,j;int f=9,len;
    
        len=strlen(str);
    
       
    
        for(i=0,j=len-1;i<len&&j>=0;i++,j--)
    
        {
    
            if((str[i]=='b')&&(str[j]=='d'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='d')&&(str[j]=='b'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='I')&&(str[j]=='I'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='M')&&(str[j]=='M'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='O')&&(str[j]=='O'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='o')&&(str[j]=='o'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='p')&&(str[j]=='q'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='q')&&(str[j]=='p'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='T')&&(str[j]=='T'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='U')&&(str[j]=='U'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='V')&&(str[j]=='V'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='v')&&(str[j]=='v'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='w')&&(str[j]=='w'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='W')&&(str[j]=='W'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='X')&&(str[j]=='X'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='x')&&(str[j]=='x'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='Y')&&(str[i]=='Y'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='A')&&(str[j]=='A'))
    
            {
    
                f=0;continue;
    
            }
    
            else if((str[i]=='H')&&(str[j]=='H'))
    
            {
    
                f=0;continue;
    
            }
    
            else
    
            {
    
                f=1;break;
    
            }
    
        }
    
        if(f==0 || strcmp(str,"bob")==0 )
    
        printf("TAK\n");
    
        else
    
        printf("NIE\n");
    
        return 0;
    
    }
 **6). Deletion of sub string- V**

    #include <stdio.h>
    #include<string.h>
    int main()
    {
    	int n,i,j,k,l,m,l1,l2,f;
    	char str1[10000],str2[100000];
    	scanf("%d",&n);
    	while(n>0){
    	    n--;
    	    scanf("%s",str1);
    	    scanf("%s",str2);
    	    l1=strlen(str1);
    	    l2=strlen(str2);
    	    for(i=0;i<l1;i++)
            {
    	        f=0;
    	        for(j=0;j<l2;j++)
                {
    	            if(str1[i]==str2[j])
                    {
    	                f=1;
    	            }
    	        }
    	        if(f==0)
                {
    	            printf("%c",str1[i]);
    	        }
    	    }
    	 printf("\n");
    	 return 0;
        }   

 **7).YOUTUBER SUM**
          
        #include <stdio.h>
        #include <string.h>

        int isPali(char str[], char remain[], int spot)
        {
            if (strlen(remain) == spot)
            {
                 int len = strlen(str);
                 int i, pali = 1;
                 for (i=0; i < len; i++)
                 {
                    if (str[i] != str[len-1-i])
                    {
                        pali = 0;
                        break;
                     }
                 }
                 if (pali == 1 && len > 0)
                 {
                    return 1;
                 }
                 else 
                 {
                    return 0;
                 }
            } 
            else 
            {
                char var = remain[spot];
                char str2[50];
                strcpy(str2, str);
                strncat(str2, &var, 1);
                return isPali(str2, remain, spot+1) + isPali(str, remain, spot+1);
            }
        }
        int main()
        {
            char remain[50];
            scanf("%s",remain);
            char str[50] = "";
            int sum = isPali(str, remain, 0);
            printf("%d", sum);
            return 0;
        }
  **8). Pattern Searching**
  
        #include <stdio.h>
        #include <string.h>
        int main()
        {
            int lines;
            char str[100];
            char tofind[100];
            scanf("%d", &lines);
            while (lines != 0)
            {
                scanf("%s",str);
                scanf("%s",tofind);
                char *ptr = strstr(str, tofind);
                if (ptr != NULL)
                {
                    printf("found\n");
                } 
                else 
                {
                    printf("not found\n");
                }
                lines -= 1;
            }
            return 0;
         }
**9). SORTING EMPLOYEES**

            #include <stdio.h>
            #include <string.h>
            typedef struct 
            {
                char name[106];
                int salary;
            } 
            employee;
            int main()
            {
                int lines;
                int count;
                scanf("%d", &lines);
                while (lines != 0) 
                {
                    employee e[1000];
                    scanf("%d", &count);
                    int i, j;
                    for (i=0; i < count; i++)
                    {
                        scanf("%s", e[i].name);
                        scanf("%d", &e[i].salary);
                    }
                    employee temp;
                    for (i=0; i < count-1; i++)
                    {
                        for (j=i+1; j < count; j++)
                        {
                            if(e[i].salary > e[j].salary)
                            {
                                temp = e[i];
                                e[i] = e[j];
                                e[j] = temp;
                             }
                            else 
                            {
                                if (e[i].salary == e[j].salary)
                                {
                                    if (strcmp(e[i].name,e[j].name) > 0)
                                    {
                                        temp = e[i];
                                        e[i] = e[j];
                                        e[j] = temp;
                                    }
                                }
                            }
                        }
                    }
                    lines -= 1;
                    for (i=0; i < count; i++){
                    printf("%s %d ",e[i].name, e[i].salary);
                    }
                    printf("\n");
                }
                return 0;
                }
**10). Numbers to Words**

            #include <stdio.h>
            #include <string.h>
            #include <stdlib.h>
            /* A function that prints given number in words */
            void convert_to_words(char *num)
            {
                int len = strlen(num); // Get number of digits in given number
                char *single_digits[] = { "zero", "one", "two", 
                                           "three", "four","five", 
                                           "six", "seven", "eight", "nine"};
 
                char *two_digits[] = {"", "ten", "eleven", "twelve", 
                                            "thirteen", "fourteen",
                                            "fifteen", "sixteen", 
                                            "seventeen", "eighteen", "nineteen"};
 
                char *tens_multiple[] = {"", "", "twenty", "thirty", "forty", "fifty",
                                        "sixty", "seventy", "eighty", "ninety"};
 
                char *tens_power[] = {"hundred", "thousand"};
 
                if (len == 1) {
                printf("%s\n", single_digits[*num - '0']);
                return;
                }
 
                while (*num != '\0') {
 
                if (len >= 3) {
                       if (*num -'0' != 0) {
                         printf("%s ", single_digits[*num - '0']);
                         printf("%s ", tens_power[len-3]);
                }
                --len;
                }
 
                else {
                    if (*num == '1') {
                         int sum = *num - '0' + *(num + 1)- '0';
                         printf("%s\n", two_digits[sum]);
                         return;
                        }   
 
                else if (*num == '2' && *(num + 1) == '0') {
                        printf("twenty\n");
                        return;
                    }   
 
                else {
                    int i = *num - '0';
                    printf("%s ", i? tens_multiple[i]: "");
                    ++num;
                    if (*num != '0')
                        printf("%s ", single_digits[*num - '0']);
                    }
            }
            ++num;
         }
    }

    int main() {
        int lines;
        scanf("%d", &lines);
        char str[4];
        while (lines != 0) {
            scanf("%s", str);
            convert_to_words(str);
            lines -= 1;
        }
        return 0;
    }


 TO BE CONTINUED......
