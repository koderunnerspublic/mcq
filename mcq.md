# KIITSAT CS Recruitment

### Time: 30 minutes
### Questions: 10

**Q1.**
```# include <stdio.h>
void fun(int *ptr) {
    *ptr = 30;
}
int main() {
  int y = 20;
  fun(&y);
  printf("%d", y);
  return 0;
}
```
**Options**
1. 20
2. 30
3. Compiler Error
4. Runtime Error


**Q2.**
Consider a compiler where int takes 4 bytes, char takes 1 byte and pointer takes 4 bytes.
```#include <stdio.h> 
int main() {
    int arri[] = {1, 2 ,3};
    int *ptri = arri;
    char arrc[] = {1, 2 ,3};
    char *ptrc = arrc;
    printf("sizeof arri[] = %d ", sizeof(arri));
    printf("sizeof ptri = %d ", sizeof(ptri));
    printf("sizeof arrc[] = %d ", sizeof(arrc));
    printf("sizeof ptrc = %d ", sizeof(ptrc));
    return 0;
}
```

**Options**
1. sizeof arri[] = 3 sizeof ptri = 4 sizeof arrc[] = 3 sizeof ptrc = 4
2. sizeof arri[] = 12 sizeof ptri = 4 sizeof arrc[] = 3 sizeof ptrc = 1
3. sizeof arri[] = 3 sizeof ptri = 4 sizeof arrc[] = 3 sizeof ptrc = 1
4. sizeof arri[] = 12 sizeof ptri = 4 sizeof arrc[] = 3 sizeof ptrc = 4


**Q3.**
Assume that float takes 4 bytes, predict the output of following program.
```#include <stdio.h>
int main() {
    float arr[5] = {12.5, 10.0, 13.5, 90.5, 0.5};
    float *ptr1 = &arr[0];
    float *ptr2 = ptr1 + 3;
    printf("%f ", *ptr2);
    printf("%d", ptr2 - ptr1);
   return 0;
}```

**Options**
1. 90.500000 3
2. 90.500000 12
3. 10.000000 12
4. 0.500000 3


**Q4.**
```#include<stdio.h>
int main()
{
    int arr[] = {10, 20, 30, 40, 50, 60};
    int *ptr1 = arr;
    int *ptr2 = arr + 5;
    printf("Number of elements between two pointer are: %d.", 
                                (ptr2 - ptr1));
    printf("Number of bytes between two pointers are: %d",  
                              (char*)ptr2 - (char*) ptr1);
    return 0;
}```

**Options**
1. Number of elements between two pointer are: 5. Number of bytes between two pointers are: 20
2. Number of elements between two pointer are: 20. Number of bytes between two pointers are: 20
3. Number of elements between two pointer are: 5. Number of bytes between two pointers are: 5
4. Compiler Error
5. Runtime Error


**Q5.**
```#include<stdio.h> 
int main() 
{ 
   int a; 
   char *x; 
   x = (char *) &a; 
   a = 512; 
   x[0] = 1; 
   x[1] = 2; 
   printf("%dn",a);   
   return 0; 
}```

**Options**
1. Machine Dependent
2. 531
3. 258
4. Compiler Error


**Q6.**
```#include <stdio.h>
int main()
{
 char *ptr = "KIITSAT";
 printf("%c", *&*&*ptr);
 return 0;
}```

**Options**
1. Compiler Error
2. Garbage Value
3. Runtime Error
4. K


**Q7.**
The reason for using pointers in a C program is

**Options**
1. Pointers allow different functions to share and modify their local variables
2. To pass large structures so that complete copy of the structure can be avoided
3. Pointers enable complex “linked" data structures like linked lists and binary trees
4. All of the above


**Q8.**
Consider this C code to swap two integers and these five statements after it:
```void swap(int *px, int *py) 
{ 
   *px = *px - *py; 
   *py = *px + *py; 
   *px = *py - *px; 
}```
S1: will generate a compilation error
S2: may generate a segmentation fault at runtime depending on the arguments passed
S3: correctly implements the swap procedure for all input pointers referringto integers
stored in memory locations accessible to the process
S4: implements the swap procedure correctly for some but not all valid input pointers 
S5: may add or subtract integers and pointers.

**Options**
1. S1
2. S2 and S3
3. S2 and S4
4. S1 and S2
5. S5 and S3


**Q9.**
```#include <stdio.h>
int main()
{
    int arr[] = {1, 2, 3, 4, 5};
    int *p = arr;
    ++*p;
    p += 2;
    printf("%d", *p);
    return 0;
}```

**Options**
1. 2
2. 3
3. 4
4. Compiler Error


**Q10.**
What does the following C-statement declare?
```int ( * f) (int * ) ;```

**Options**
1. A function that takes an integer pointer as argument and returns an integer
2. A function that takes an integer as argument and returns an integer pointer
3. A pointer to a function that takes an integer pointer as argument and returns an integer
4. A function that takes an integer pointer as argument and returns a function pointer
