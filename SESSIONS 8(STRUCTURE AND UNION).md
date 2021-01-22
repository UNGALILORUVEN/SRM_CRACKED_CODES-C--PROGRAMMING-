**Q. 71: Student Data Repository**

    #include<stdio.h>
    struct student
    {
     char name[100];
    struct dateOfBirth
    {
      int rollno,date,month,year;
    }DOB;
    }std;
    int main()
    {
      scanf("%s%d%d%d%d",std.name,&std.DOB.rollno,&std.DOB.date,&std.DOB.month,&std.DOB.year);
      printf("Name=%s\nRollNo=%d\nDate of birth=%d/%d/%d",std.name,std.DOB.rollno,std.DOB.date,std.DOB.month,std.DOB.year);
      return 0;
    }
**Q. 75: Phd Fees**

    #include <stdio.h>
    #include<string.h>
    struct student
    {
      int roll;
      char name[100];
      char course[100];
      int fees;
    }s1;  
    int main()
    {
    printf("Details of student");
      scanf("%d",&s1.roll);
      scanf("%s",s1.name);
      scanf("%s",s1.course);
      scanf("%d",&s1.fees);
      printf("\nRoll Number=%d",s1.roll);
      printf("\nName=%s",s1.name);
      printf("\nCourse=%s",s1.course);
      printf("\nFees=%d",s1.fees);
      return 0;
    }
***Q. 76: Sonata***

    #include <stdio.h>
    union Time
    {
      int seconds,minutes,hours;
    };
    int main(){
        union Time startTime,stopTime,diff;
        printf("The time difference is\n");
        scanf("%d %d\n",&startTime.hours,&stopTime.hours);
        diff.hours=startTime.hours-stopTime.hours;
        printf("Hours:%d\n",diff.hours);
        scanf("%d %d\n ",&startTime.minutes,&stopTime.minutes);
        diff.hours=startTime.minutes-stopTime.minutes;
        printf("Minutes:%d\n",diff.minutes);
        scanf("%d %d",&startTime.seconds,&stopTime.seconds);
        diff.hours=startTime.seconds-stopTime.seconds;
        printf("Seconds:%d\n",diff.seconds);
        return 0; 
    }
***Q. 77: Student Marksheet***

    #include <stdio.h>
    #include<string.h>
    union Student{
      char name[60];
      int tamil,english,maths,science,ss;
    };
    int main() {
      union Student s1;
      printf("Details of student\n");
      scanf("%s",s1.name);
       printf("Name of the student=%s\n",s1.name);
      scanf("%d",&s1.tamil);
      printf("Tamil=%d\n",s1.tamil);
      scanf("%d",&s1.english);
      printf("English=%d\n",s1.english);
      scanf("%d",&s1.maths);
      printf("Maths=%d\n",s1.maths);
      scanf("%d",&s1.science);
      printf("Science=%d\n",s1.science);
      scanf("%d",&s1.ss);
      printf("Social Science=%d",s1.ss);
    	return 0;
    }


***Q. 78: Add Up the Distance***

    #include <stdio.h>
    union Distance
    {
      int feet_of_type;
      float inch_of_type;
    };
    int main()
    {
      union Distance d1,d2,sumOfDistances;
      scanf("%d %d\n",&d1.feet_of_type,&d2.feet_of_type );
      sumOfDistances.feet_of_type=d1.feet_of_type+d2.feet_of_type;
      printf("Sum of distances=%d feet\n",sumOfDistances.feet_of_type);
      scanf("%f %f\n",&d1.inch_of_type,&d2.inch_of_type);
      sumOfDistances.inch_of_type=d1.inch_of_type+d2.inch_of_type;    
      printf("Sum of distances=%.2f inches",sumOfDistances.inch_of_type);
      return 0;
    }