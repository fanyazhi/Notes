# How to loop through an array
```
for (int i = 0; i < sizeof(arr)/sizeof(arr[0]); i++) 
	cout <<arr[i]<<endl;

```
# How to loop through multidimensional array
```
// example array
int A[][3] = {
        {1, 2, 3},
        {4, 5, 6}
};

//display array
for (unsigned int i=0; i<sizeof(A)/sizeof(A[0]); i++) {
    for (unsigned int j=0; j<sizeof(A[0])/sizeof(A[0][0]); j++) {
        cout << A[i][j] << " " << flush;
    }
    cout << endl;
}; 

```
# How to loop through a list 
This method requires C++11

```
#include <list>

list<int> myList = {0, 1, 2, 3, 4};
for (auto v : myList)
	cout << v << "\n";
```

Using iterator: 
 
```
#include <list>

list<int> myList = {0, 1, 2, 3, 4};
list<int>::const_iterator iterator;
for (iterator = myList.begin(); iterator != myList.end(); ++iterator) {
    cout << *iterator << "\n";
}
```

---
**[Go back >>](/CPP)**