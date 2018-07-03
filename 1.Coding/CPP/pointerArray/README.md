# Pointers and Arrays
Arrays work very much like pointers to their first elements.  
For example, consider these two declarations:  

```
int myarray [20];
int * mypointer;

```
The following assignment operation would be valid:  
```
mypointer = myarray;
```

The only difference is that myarray knowns how many blocks of ints it is pointing to, mypointer doesn’t.  
An example that mixes arrays and pointers:  

```
#include <iostream>
using namespace std;

int main ()
{
  int numbers[5];
  int * p;
  p = numbers;  *p = 10;
  p++;  *p = 20;
  p = &numbers[2];  *p = 30;
  p = numbers + 3;  *p = 40;
  p = numbers;  *(p+4) = 50;
  for (int n=0; n<5; n++)
    cout << numbers[n] << ", ";
  return 0;
}
```
output: 10, 20, 30, 40, 50

---
Brackets are a dereferencing operator known as offset operator. They dereference the variable they follow just as * does, but they also add the number between brackets to the address being dereferenced. For example:  

```
a[5] = 0;       // a [offset of 5] = 0
*(a+5) = 0;     // pointed to by (a+5) = 0 
```

---
**[Reference: cplusplus.com](http://www.cplusplus.com/doc/tutorial/pointers/)**