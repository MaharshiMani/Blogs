---
title: C++ Basics 
description: This blog contains the basics of c++
date: 09 Jan 2026
author: Maharshi Mani Tripathi
---
# Basics of C++
## Variables in C++

* A variable is a container to hold data.

* Primarily we have these varible types in C++:

    1.Int

    2.Float(Low precision)

    3.Char

    4.Double(High precision)

    5.Boolean(true=1, false=0)

* Based on Scope, variable can be classified into two types:

    1.Local Variables

    2.Global Variables

### Variable Scope

* Scope of a variable is the region in code where the existence of variable is valid.

* **Local Variable**: These variables are declared inside the braces of any function and can be accessed only from there.

* **Global Variable**: These variables are declared outside any function and can be accessed from anywhere.

    **Global and Local variable can have same name in C++.**

## Data Types in C++

* Data types define the type of data a variable can hold, for example an integer variable can hold integer data, a character type variable can hold character data etc.

* Data types in C++ are cateorized in three groups:
    * **Built-in**: int, float, char, double and bool.
    * **User-defined**: struct, union and enum.
    * **Derived**: array, functions and pointers.

## Some Example Programs:

```
#include<iostream>
using namespace std;

int main(){
    int a=14, b=15;
    float pi=3.14;
    char poo='c';
    bool is_true=true;
    bool is_false=false;
    cout<<"Here the value of a is "<<a<<". \nThe value of b is "<< b;
    cout<<"\nThe value of pi is "<<pi;
    cout<<"\nHere the value of poo is "<< poo<<"\n";
    cout<<is_true<<"\n"<< is_flase;
    return 0;
}

OUTPUT:
Here the value of a is 14.
The value of b is 15
The value of pi is 3.14
Here the value of poo is c
1
0 
```

**Local variable has higher precendence over the global variable.**

```
include<iostream>
using namespace std;

int glo=4;

int main(){
int glo=34;
cout<<glo;
return 0;
}

OUTPUT:
34
```
```
include<iostream>
using namespace std;
int glo=6;

void sum(){
    cout<<glo;
}
int main(){
    int glo=26;
    glo=45;
    cout<<glo"\n";
    sum();
    return 0;
}

OUTPUT:
45  
2
```
## Rules To declare variables in C++
* Variable names in C++ can range from 1 to 255 characters.
* All variable name must begin with a letter of the alphabet or an underscore(_).
* After the first initial letter, variable names can also contain letters and numners.
* Variable names are case sensitive.
* No spaces or special characters are allowed.
* You cannot use a C++ keyword(a reserved word) as a cariable name.

## Basic Input/Output in C++
* C++ comes with libraries which helps us in performing input/output. In C++ sequence of bytes corresponding to input and output are commonly known as streams.
* **Input Stream**: Direction of flow of bytes takes place from input device(for ex Keyboard) to the main memory.
* **Output Stream**: Directin of flow of bytes takes place from main memory to the output device(for ex Display).

```
#include<iostream>
using namespace std;

int main(){
    int num1, num2;
    cout<<"Enter the value of num1:\n"; /* '<<' is called the Insertion operator */
    cin>>num1; /* '>>' is called the Extraction operator */

    cout<<"Enter the value of num2:\n"; /* '<<' is called the Insertion operator */
    cin>>num2; /* '>>' is called the Extraction operator */

    cout<<"The sum is:"<< num1+num2;
    return 0;
}

OUTPUT:
Enter the value of num1:
3
Enter the value of num2:
6
The sum is:9
```