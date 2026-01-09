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

    5.Boolean

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

```
#include<iostream>
using namespace std;

int main(){
    int a=14, b=15;
    float pi=3.14;
    char poo='c'
    cout<<"Here the value of a is "<<a<<". \nThe value of b is "<< b;
    cout<<"\nThe value of pi is"<<pi;
    cout<<"\nHere the value of poo is"<< poo;
    return 0;
}