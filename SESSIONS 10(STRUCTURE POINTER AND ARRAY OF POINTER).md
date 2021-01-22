
**1). Increment Using Pointer**

    #include <stdio.h>
    int main() {
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
