---
title: "Calculator"
date: 2019-01-04
tags: [C++]
header: 
   teaser: /images/c.jpg
excerpt: "C++"
---

#### [Simple Calculator](https://github.com/Angphurba/Calculator) 
***
### Program details:

*Basic calculation.*

*Calculates:* 
+ *addtion*
+ *subtraction*
+ *multiplication*
+ *division*
+ *remainder.*

*Enter any two number and choose what calculation to perform.*

### C++ code block:
```c++ 
#include "stdafx.h"
#include <iostream>

using namespace std;
int addition(int num1, int num2);
int subtraction(int num1, int num2);
int division(int num1, int num2);
int multiplication(int num1, int num2);
int remainder(int num1, int num2);
int num1, num2, result;
char option;

int main()
{
	while (1){
		cout << "\nSimple calculator" << endl;
		cout << "\nEnter First Number: ";
		cin >> num1;
		cout << "\nEnter Second Number: ";
		cin >> num2;
		cout << "Enter + for Addtion\nEnter - for Subtraction\n Enter / for Division\nEnter * for Multiplication\nEnter % for remainder\n Enter E to EXIT\n";
		cout << "\nEnter Option: ";
		cin >> option;
	
	
	if (option == '+')
	{
		result = (num1+num2);
		cout << "\n\t\t" << num1 << " + " << num2 << " = " << result << endl;
	}
	else if (option == '-')
	{
		result = (num1-num2);
		cout << "\n\t\t" << num1 << " - " << num2 << " = " << result << endl;
	}
	else if (option == '/')
	{   
	    if (num2 == 0)
		{
			cout << "\n\t\tError: Divide by zero is not allowed" << endl;
			return 0;
		}
		else
		result = (num1/num2);
		cout << "\n\t\t" << num1 << " / " << num2 << " = " << result << endl;
	}
	else if (option == '*')
	{
		result = (num1*num2);
		cout << "\n\t\t" << num1 << " X " << num2 << " = " << result << endl;
	}
	else if (option == '%')
	{
		result = (num1%num2);
		cout << "\n\t\t" << num1 << " % " << num2 << " = " << result << endl;
	}
	else if (option == 'e'|| option == 'E')
	{
	    cout <<"\n\t\t Thank you.";
	    return 0;
	}
	else
	{
		cout << "\n\t\tINVALID OPTION\n";
	}
	}
}
```
### Console block:
```console
Simple calculator                                                                                                                                      
                                                                                                                                                       
Enter First Number: 2                                                                                                                                  
                                                                                                                                                       
Enter Second Number: 2                                                                                                                                 
Enter + for Addtion                                                                                                                                    
Enter - for Subtraction                                                                                                                                
 Enter / for Division                                                                                                                                  
Enter * for Multiplication                                                                                                                             
Enter % for remainder                                                                                                                                  
 Enter E to EXIT                                                                                                                                       
                                                                                                                                                       
Enter Option: -                                                                                                                                        
                                                                                                                                                       
                2 - 2 = 0                                                                                                                              
                                                                                                                                                       
Simple calculator                                                                                                                                      
                                                                                                                                                       
Enter First Number: 3                                                                                                                                  
                                                                                                                                                       
Enter Second Number: 2                                                                                                                                 
Enter + for Addtion                                                                                                                                    
Enter - for Subtraction                                                                                                                                
 Enter / for Division                                                                                                                                  
Enter * for Multiplication                                                                                                                             
Enter % for remainder                                                                                                                                  
 Enter E to EXIT    
 Enter Option: *                                                                                                                                        
                                                                                                                                                       
                3 X 2 = 6                                                                                                                              
                                                                                                                                                       
Simple calculator                                                                                                                                      
                                                                                                                                                       
Enter First Number: 18                                                                                                                                 
                                                                                                                                                       
Enter Second Number: 5                                                                                                                                 
Enter + for Addtion                                                                                                                                    
Enter - for Subtraction                                                                                                                                
 Enter / for Division                                                                                                                                  
Enter * for Multiplication                                                                                                                             
Enter % for remainder                                                                                                                                  
 Enter E to EXIT                                                                                                                                       
                                                                                                                                                       
Enter Option: %                                                                                                                                        
                                                                                                                                                       
                18 % 5 = 3                                                                                                                             
                                                                                                                                                       
Simple calculator                                                                                                                                      
                                                                                                                                                       
Enter First Number: 1    
Enter Second Number: 1                                                                                                                                 
Enter + for Addtion                                                                                                                                    
Enter - for Subtraction                                                                                                                                
 Enter / for Division                                                                                                                                  
Enter * for Multiplication                                                                                                                             
Enter % for remainder                                                                                                                                  
 Enter E to EXIT                                                                                                                                       
                                                                                                                                                       
Enter Option: e                                                                                                                                        
                                                                                                                                                       
                 Thank you.                                                                                                                            
                                   
```
         