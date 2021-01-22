  **1). Mirror Problem**
   

    #include <stdio.h>
    int main()
    {
        int num,tNum,cnt;
        scanf("%d",&num);
        cnt=0;
        tNum=num;
        while(tNum>0){
            cnt++;
            tNum/=10;
        }
        printf("%d",cnt);
        return 0;
    }

**2). Series of Series**

    #include <stdio.h>
    int main() {
        int i, n, t1 = 0, t2 = 1, nextTerm;
        scanf("%d", &n);
        for (i = 1; i <= n; ++i) {
            printf("%d ", t1);
            nextTerm = t1 + t2;
            t1 = t2;
            t2 = nextTerm;
        }
        return 0;
    }
**3). Value Insertion**

    #include <stdio.h>
    int main()
    {
      int array[100],position,c,n,value;
      scanf("%d",&n);
      for(c=0;c<n;c++)
      scanf("%d",&array[c]);
      scanf("%d",&value);
      scanf("%d",&position);
      for(c=n-1;c>=position;c--)
       array[c+1]=array[c];
       array[position]=value;
      for(c=0;c<=n;c++)
         printf("%d\n",array[c]);
      return 0;
    }
**4). Armstrong Digits**

    #include <stdio.h>
    int main() {
    	int i,n,num,t,d,r;
      scanf("%d",&n);
      for(i=0;i<n;i++)
      {
      scanf("%d\n",&num);
       t=num;
        r=0;
      while (t!=0)
        {
          d=t%10;
          r=r+(d*d*d);
          t=t/10;
        } 
      if (r==num)
        printf("Armstrong\n");
      else 
        printf("Not Armstrong\n");
      }
    	return 0;
    }

**5). State Election**

    #include <stdio.h>
    int main() 
    {
    	
      int a;
      scanf("%d", &a);
      if(a >=18 && a <=60 )
        {
        printf("Eligible");
       } 
      else
        {
        printf("Not Eligible");
       } 
    	return 0;
    }
**6). Power of 2**

    #include<stdio.h>
    #include<math.h>
    int main() {
    
        int num;   
          scanf("%d", &num);
        if(num && ((num & (num-1)) == 0)){
    
            printf("WOW");
    
        } else {
    
            printf("OOPS");
    
        }
        return 0;
    
    }
**7). Switch Integer**

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
**8). Occurrences of Characters**

    #include<stdio.h>
    #include<string.h>
    int main()
    {
      char s[200];
      int t,len,arr[26],i,f;
      scanf("%d",&t);
      while(t--)
      {
        for(i=0;i<26;i++) arr[i] = 0;
        scanf("%s",s);
        len = strlen(s);
        for(i=0;i<len;i++)
        {
          arr[s[i]- 'a']++;
        }
        f=0;
        for(i=0;i<26;i++)
        {
          if(arr[i] == len - arr[i]) { f = 1; break;}
        }
        if(f == 1) printf("YES\n");
        else printf("NO\n");
      }
      return 0;
    }

**9). Grading System**

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
**10). Star Formation**

    #include <stdio.h>
    int main() {
       int i, j, rows;
       scanf("%d", &rows);
       for (i = 1; i <= rows; ++i) {
          for (j = 1; j <= i; ++j) {
             printf("*");
          }
          printf("\n");
       }
       return 0;
    }
 TO BE CONTINUED....
