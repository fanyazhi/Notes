# References

```
int value1;
int &value2;

```
value 2 is declared as reference, it is an alias for value1 (same variable).  

References are usful in functions where we do not want to return variables, but to replace them.  
<br/>

*Reference is different from pointer*  

* Once a reference is declared, it cannot be made to reference another object.  
* Reference cannot be NULL, pointer can.
* Reference don't need dereferencing operators. '&' operator is only needed at the time of declaration.


---
**[Reference Source](https://www.geeksforgeeks.org/references-in-c/)**