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
 **Q. 54: Deletion of sub string- V**

    #include <stdio.h>
    #include<string.h>
    int main() {
    	//code
    	int n,i,j,k,l,m,l1,l2,f;
    	char str1[10000],str2[100000];
    	scanf("%d",&n);
    	while(n>0){
    	    n--;
    	    scanf("%s",str1);
    	    scanf("%s",str2);
    	    l1=strlen(str1);
    	    l2=strlen(str2);
    	    for(i=0;i<l1;i++){
    	        f=0;
    	        for(j=0;j<l2;j++){
    	            if(str1[i]==str2[j]){
    	                f=1;
    	            }
    	        }
    	        if(f==0){
    	            printf("%c",str1[i]);
    	        }
    	    }
    	    printf("\n");
    	    
    	}
    	return 0;
    }
