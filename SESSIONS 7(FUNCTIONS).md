
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