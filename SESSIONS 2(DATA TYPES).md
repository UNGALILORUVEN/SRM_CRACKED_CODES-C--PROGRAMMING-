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
 **11). State Election**

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
 **12). Four Square**
 
     #include <stdio.h>
     #include <math.h>
     int main()
     {
      int lines;
      scanf("%d\n",&lines);
      while (lines != 0) {
      int num, result;
      scanf("%d", &num);
      result = floor(sqrt(num));
      printf("%d\n",(int) result);
      lines -= 1;}
      return 0;
      }
  **13). Print NCR**
  
      #include <stdio.h>
      int fact(int z);
      int main()
      {
       int n, r, ncr;
       scanf("%d%d", &n, &r);
       ncr = fact(n) / (fact(r) * fact(n - r));
       printf("%d", ncr);
       return 0;
       }
  **14). Magical game of sum**
        
       #include<stdio.h>
       int main()
       {
        int l,t,n;
        scanf("%d",&l);
        while (l != 0)
      {
       scanf("%d %d",&t,&n);
       while (t != 0 )
       {
          n=n*(n+1)/2;
          t-=1;
       }
       printf("%d\n",n);
       l-=1;
      }
      return 0;
     }
 **15). Happy Addition**

       #include <stdio.h>
       int main() 
       {
       int j,i,k,c;
       scanf("%d",&k);
       int a[k];
       for (i=0;i<k;i++)
       {
         scanf("%d",&a[i]);
       }
       scanf("%d %d",&c,&j);
       for (i=k-1;i>=j-1;i--)
       {
         a[i+1]= a[i];
       }
       a[j-1]=c;
       for(i=0;i<=k;i++)
       {
         printf(" %d",a[i]);
        }
      return 0;
      }
 **16). Sum of Two Large Numbers**
 
        #include <stdio.h>
        int main()
        {
        int n,x,y,i,t,j;
        scanf("%d",&n);
        for(i=0;i<n;i++)
        {
        scanf("%d %d",&x,&y);
        t=x+y;
        int c1=0,c2=0,x1;
        while(t!=0)
        {
          c1++;
          t/=10;
        }
       x1=x;
       t=x+y;
       while(x1!=0)
       {
        c2++;
        x1/=10;
       }
       if(c1==c2)
       {
       printf("%d\n",t);
       } 
      else 
      {
        printf("%d\n",x);
      }
    }
 	return 0;
    }
**17). Rate of Interest**

      #include <stdio.h>
      int main()
      {
      int p,t;
      float r, si;
      scanf("%d",&p);
      scanf("%d",&t);
      scanf("%f", &r);
      si=(p*t*r)/100;
      printf("%.2f",si);
      return 0;
      }
 **18). Mersal vs Babubali**
 
       #include <stdio.h>
       int main()
    {
        int n,i,b,o;
        scanf("%d",&n);
        int a[n];
        b=0,o=0;
        for(i=0;i<n; i++)
        {
            scanf("%d",&a[1]);
            if(a[1]%2==0)
            {
                b++;
            }
            else
            {
                o++;
            }
        }
        if(b>o)
        {
                printf("READY FOR BATTLE");
        }
        else
        {
                printf("NOT READY");
        }
        return 0;
    }
**19). India vs England**

    #include <stdio.h>
    int main()
    {
       int a;
       scanf("%d",&a);
       if(a>0)
       {
          if (a%2==0)
          printf("ENGLAND");
          else if(a%2!=0)
          printf("INDIA");
       }
       else
           printf ("Sorry");
       return 0;
     }
 **20). Swap Numbers**
 
      #include <stdio.h>
      int main()
      {
      int a=0;int b=0;
      scanf("%d%d",&a,&b);
      a=a+b;
      b=a-b;
      a=a-b;
      printf("Values after Swapping\nvalue of a is:%d\nvalue of b is:%d", a,b);
      return 0;
      }
**21). Seasoners**

     #include <stdio.h>
     int main ()
     {
       char month[100],l[3];
        scanf("%s",month);
        scanf("%s",l);
        if((strcmp(l,"22")==0)&&(strcmp(month, "Sep")==0))
        {
            printf("Fall");
        }
        if((strcmp(l,"20")==0)&&(strcmp(month, "Man")==0))
        {
            printf("Summer");
        }
       if((strcmp(l,"21")==0)&&(strcmp(month,"Jun")==0))
       {
            printf("Spring");
       }
       if((strcmp(l,"21")==0)&&(strcmp(month,"Dec")==0))
       {
            printf("winter");
       }
 **22). Narcissistic Sum**
 
      #include <stdio.h>
      int main() 
     {
        int n;
        scanf("%d",&n);
        int temp, sum=0;
        temp=n;
        while(n>0)
        {
             sum=sum+((n%10)*(n%10)*(n%10));
             n=n/10;
        }
        if(sum==temp)
           printf("Narcissistic Number");
        else
           printf("NOT Narcissistic Number");
        return 0;
     }
 **23). Welcome to World**
 
        #include <stdio.h>
        int main ()
        {
          char n[20];
          char c[20];
          char p[20];
          int s;
          float sp;
          scanf("%s",n);
          scanf("%s",c);
          scanf("%s",p);
          scanf("%d",&s);
          scanf("%f",&sp);
          printf("Robot Details\n");
          printf("I am the Robot name=%s\n",n);
          printf("I was created by %s\n", c);
          printf ("I am created for the purpose of %s\n",p);
          printf("My memory space is around amb and my speed is %.1fTB",s,sp);
          return 0;
        }
 **24). Display your name**
 
    #include <stdio.h>
    int main(void)
    {
      char string[25];
      scanf("%[^\n]*c", string);
      printf("Your name is:%s", string);
      return 0;
    }
**25). Cube of a number**

    #include <stdio.h>
    int main()
    {
      int ctr;
      scanf("%d",&ctr);
      printf("%d\n", (ctr*ctr*ctr));
      return 0;
    }
**26). Square of the Number**

     #include <stdio.h>
     int main()
     {
       int ctr;
       scanf("%d",&ctr);
       printf("%d", (ctr*ctr));
       return 0;
     }
 **27). Hero's Formula/ Heroine's Formula**
 
    #include <math.h>
    #include <stdio.h>
    int main()
    {
      int a, b, c;
      scanf("%d %d %d", &a, &b, &c);
      float s = (a+b+c)/2.0;
      float area = sqrt(s*(s-a)*(s-b)*(s-c));
      printf("%.2f", area);
      return 0;
    }
    

 TO BE CONTINUED....
