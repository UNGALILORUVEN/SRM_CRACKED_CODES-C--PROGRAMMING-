
**1). where is hanoi**

    #include "stdio.h"
    void towerOfHanoi(int n, char srcTower, char dstTower, char bufferTower) {
      if (n <= 0) return;
      if (n == 1) {
        printf("Move disk 1 from rod %c to rod %c\n", srcTower, dstTower);
        return;
      }
      towerOfHanoi(n - 1, srcTower, bufferTower, dstTower);
      printf("Move disk %d from rod %c to rod %c\n", n, srcTower, dstTower);
      towerOfHanoi(n - 1, bufferTower, dstTower, srcTower);
    }
    int main() {
      int i = 0;
      int n = 0;
      scanf("%d", &n);
      towerOfHanoi(n, 'A', 'C', 'B');
      return 0;
    }
**2). password not strong enough**

    #include <stdio.h>
    
    
    int length = 0;
    int digit = 0;
    int lower = 0;
    int upper = 0;
    int special = 0;
      
    
    int pass(char s[],int n) {
      int i;
      
      length = n;
        
      for (i = 0; i < n; i++) {
        if (s[i] >= 48 && s[i] <= 57)
          digit = 1;
        
        if (s[i] >= 97 && s[i] <= 122)
          lower = 1;
        
        if (s[i] >= 65 && s[i] <= 90)
          upper = 1;
        
        switch(s[i]) {
          case '!':
          case '@':
          case '#':
          case '$':
          case '%':
          case '^':
          case '&':
          case '*':
          case '(':
          case ')':
          case '-':
          case '+':
            special = 1;
        }  
      }
    }
    
    int main() {
        int n; 
        scanf("%i", &n);
        char password[1024];
        scanf("%s", password);
        int answer = pass(password, n);
      	int k = 4 - (digit + lower+ upper + special);
      	if (length < 6) {
          if (k > 6 - length) {
            printf("%d", k);
            return 0;
          }
          printf("%d", 6 - length);
          return 0;
        }
    	printf("%d", k);
        return 0;
    }

**3). super digit**

    #include <stdio.h>
    #include <string.h>
    #include <math.h>
    #include <stdlib.h>
    int superd(long long int sumd)
    {
        int t=0;
        if(sumd/10==0)
            {return sumd;}
        else
            {
             
             while(sumd!=0)
                 {
                 int d;
                 d=sumd%10;
                 t=t+d;
                 sumd=sumd/10.0;
             }
            }
       sumd=t; 
       return superd(sumd);
    }    
    int main() {
        int p; long long int sumd=0;
        char ch;
        ch=getchar();
        while(ch!=' ')
        {
          int q=ch-'0';
          sumd=sumd+q;
          ch=getchar();  
        }    
        scanf("%d",&p);
        sumd=p*sumd;
        //printf("%d",sum);
        printf("%d",superd(sumd));
        return 0;
    }

**4).IPV4 ADDRESSInternet protocol addressing**
            
                       #include <stdio.h>
                     #include <string.h>
                     #include <stdlib.h>

                        #define DELIM "."
                    int valid_digit(char *ip_str)
                     { 
                     while (*ip_str) {
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

                    ptr = strtok(ip_str, DELIM);

                    if (ptr == NULL)
                        return 0;

                    while (ptr) {


                        if (!valid_digit(ptr))
                            return 0;

                        num = atoi(ptr);


                        if (num >= 0 && num <= 255) {

                            ptr = strtok(NULL, DELIM);
                            if (ptr != NULL)
                                ++dots;
                        } else
                            return 0;
                    }

                    if (dots != 3)
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
                    }}while(t>0);
                        return 0;
                    }

**5).BOOK THAT NUMBER**

                    #include <stdio.h>

                    int main()
                    {
                        char isbn[10];
                        int lines;
                        scanf("%d", &lines);
                        while (lines != 0){
                            scanf("%s", isbn);
                            if (isValidISBN(isbn) == 1){
                                printf("VALID\n");
                            } else {
                                printf("INVALID\n");
                            }
                            lines -= 1;
                        }
                        return 0;
                    }

                    int isValidISBN(char isbn[]) {
                        int i, sum=0;
                        for (i=0; i < 10; i++){
                            if (isbn[i] == 'X'){
                                sum += 10 * (10-i);
                            } else {
                                sum += (isbn[i] - '0') * (10-i);
                            }
                            printf("%d\n", sum);
                        }
                        if (sum % 11 == 0){
                            return 1;
                        }
                        return 0;
                    }

**6).ALL THE ARMS YOU KNOW**

                #include <stdio.h>
                #include <math.h>

                int is_armstrong(int);

                int main()
                {
                    int num;
                    scanf("%d",&num);
                    int i;
                    printf("0");
                    for (i=1; i < num; i++){
                        if (is_armstrong(i) == 1){
                            printf(" %d",i);
                        }
                    }
                    return 0;
                }

                int is_armstrong(int number){
                    int sum = 0, count = 1, temp;
                    int number2 = number;
                    while (number >= 10){
                        temp = number%10;
                        number = (number - temp)/10;
                        count += 1;
                    }
                    number = number2;
                    while (number >= 10){
                        temp = number%10;
                        number = (number - temp)/10;
                        sum += pow(temp, count);
                    }
                    sum += pow(number,count);
                    if (sum == number2){
                        return 1;
                    }
                    return 0;
                }

**7).COUNT YAMINI COUNT**

            #include <stdio.h>

            int sum(int);

            int main()
            {
                int number;
                scanf("%d",&number);
                printf("The sum of digits in %d is %d", number, sum(number));
                return 0;
            }

            int sum(int number) {
                if (number < 10) {
                    return number;
                } else {
                    int num = number % 10;
                    number = (number - num)/10;
                    return sum(number) + num;
                }
            }
 **8). Classic prime**
 
    #include <stdio.h>
    #include <math.h>


    /* Function declarations */
    int isPrime(int num);
    int isArmstrong(int num);
    int isPerfect(int num);


    int main()
    {
        int num;
    
        scanf("%d", &num);
    
        // Call isPrime() functions
        if(isPrime(num))
        {
            printf("%d is Prime number.\n", num);
        }
        else
        {
            printf("%d is not Prime number.\n", num);
        }
    
        // Call isArmstrong() function
        if(isArmstrong(num))
        {
            printf("%d is Armstrong number.\n", num);
        }
        else
        {
            printf("%d is not Armstrong number.\n", num);
        }
    
        // Call isPerfect() function
        if(isPerfect(num))
        {
            printf("%d is Perfect number.\n", num);
        }
        else
        {
            printf("%d is not Perfect number.\n", num);
        }
    
        return 0;
    }

    int isPrime(int num) 
    {
        int i;
    
        for(i=2; i<=num/2; i++)  
         {  
        
            if(num%i == 0)  
            {
                return 0;
            }  
        } 
    
        return 1; 
    }
    int isArmstrong(int num) 
    {
        int lastDigit, sum, originalNum, digits;
        sum = 0;
    
        originalNum = num;
        
        while(num > 0)
        {
            // Extract the last digit
            lastDigit = num % 10;

            // Compute sum of power of last digit
             sum = sum + round(pow(lastDigit, digits));

            // Remove the last digit
            num = num / 10;
        }
    
        return (originalNum == sum);
    }
    int isPerfect(int num) 
    {
        int i, sum, n;
        sum = 0;
        n = num;
    
        for(i=1; i<n; i++)  
        {  
            /* If i is a divisor of num */  
            if(n%i == 0)  
            {  
                sum += i;  
            }  
        }
    
        return (num == sum);
    }
**9). Light and Multiply**

    #include<stdio.h>
    int multiply(int n1, int n2);
    int main()
    {
        int num1, num2;
        scanf("%d %d", &num1, &num2);
        printf("%d",multiply(num1, num2));
        return 0;
    }
    int multiply(int n1, int n2)
    {
        int result;
        result = n1 * n2;
        return result;
    }
 **10).  Dr who's time travel**
 
        #include <stdio.h>
        int addition(int a,int b)
        {
            return a+b;
        }
        int main()
        {
        int x,y;
        scanf("%d %d",&x,&y);
        int c=addition(x,y);
        printf("%d",c);
        return 0;
        }
 **11). Words that see through**

       #include <math.h>
    #include <stdio.h>
    #include <string.h>
    #include <stdlib.h>
    #include <assert.h>
    #include <limits.h>
    #include <stdbool.h>

    int main()
    {
        char* s = (char *)malloc(10240 * sizeof(char));
        scanf("%s",s);
        int coun=0,i;
        for(i=0;i<strlen(s);i++)
        {
            if(s[i]>=65 && s[i]<=90){coun++;}
        }
        printf("%d\n",coun+1);
        return 0;
    }
    



