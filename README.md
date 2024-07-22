# Simple Calculator Program

This repository contains a C++ program that functions as a simple calculator. The program provides a menu for basic arithmetic operations: addition, subtraction, multiplication, and division.

## Code Description

The program prompts the user to choose an arithmetic operation and then enter two numbers. Based on the user's choice, the program performs the corresponding operation and displays the result.

## Code

```cpp
#include<iostream>
using namespace std;

int main()
{
    int option;
    float n1, n2, div, sub, mul, add;
    
    cout << "---Menu---";
    cout << "\nOption 1: Addition";
    cout << "\nOption 2: Subtraction";
    cout << "\nOption 3: Multiplication";
    cout << "\nOption 4: Division";
    cout << "\nChoose an option: ";
    cin >> option;
    
    cout << "\nEnter 1st number: ";
    cin >> n1;
    cout << "\nEnter 2nd number: ";
    cin >> n2;
    
    switch (option)
    {
        case 1:
            cout << "\nSum of " << n1 << " and " << n2 << " = " << n1 + n2;
            break;
        case 2:
            cout << "\nDifference of " << n1 << " and " << n2 << " = " << n1 - n2;
            break;
        case 3:
            cout << "\nProduct of " << n1 << " and " << n2 << " = " << n1 * n2;
            break;
        case 4:
            cout << "\nDivision of " << n1 << " and " << n2 << " = " << n1 / n2;
            break;
        default:
            cout << "\nInvalid function";
    }
    
    return 0;
}
