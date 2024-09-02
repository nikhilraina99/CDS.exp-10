# Experiment-10

##Aim
To understand and implement pointer operations in C++.

## Software Used
VS Code

## Problem Statements
1. Develop a C++ program to swap two numbers using call by value.
2. Develop a C++ program to swap two numbers using call by reference.

## Theory

### Call by Value
In the call by value approach, when a function is invoked, new elements are created on the stack to store function-related information, including memory allocation for parameters and return values. Modifications to the parameters within the function do not impact the original arguments.

### Call by Reference
In the call by reference approach, the function receives a reference to the argument rather than a copy. This allows the function to operate directly on the original argument. As a result, any changes made to the parameter within the function are reflected in the actual argument.

## Program Codes

```javascript
// Nikhil
// 23070123093
// experiment 10a
#include <iostream>
using namespace std;
void swap(int *a,int* b)
{
    int temp;
    temp=*a;
    *a=*b;
    *b=temp;
  cout<<"Inside swapByValue- "<<"a = "<< *a<<" , "<<"b = "<< *b<<endl;
}
 int main()
{ int a=5,b=10;
cout<<"Before swapByValue- "<<"a = "<<a<<" , "<<"b = "<<b<<endl;
swap(&a,&b); 
cout<<"After swapByValue- "<<"a = "<<a<<" , "<<"b = "<<b<<endl;
}
```
```javascript
// Nikhil
// 23070123093
// experiment 10b
#include <iostream>
using namespace std;
void swap(int a,int b) 
{
    int temp;
    temp=a;
    a=b;
    b=temp;
   cout<<"Inside swapByValue- "<<"a = "<<a<<" , "<<"b = "<<b<<endl;
}
int main()
 
{ int a=5,b=10;
cout<<"Before swapByValue- "<<"a = "<<a<<" , "<<"b = "<<b<<endl;
swap(a,b);
cout<<"After swapByValue- "<<"a = "<<a<<" , "<<"b = "<<b<<endl;
}
```
## Outputs:

1.Call By Reference-

![Screenshot 2024-09-02 094701](https://github.com/user-attachments/assets/50dad748-785d-48c8-a42b-d031be56508d)

2.Call By Value-

![Screenshot 2024-09-02 094723](https://github.com/user-attachments/assets/3095961d-f08c-4127-884e-830bf2388cc4)

## Conclusion
- We explored how to swap numbers using call by value.
- We also explored how to swap numbers using call by reference.









