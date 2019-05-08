---
title: "Blackjack Game"
date: 2019-01-09
tags: [C++]
header: 
   teaser: /images/c.jpg
excerpt: "C++"
---

#### [Blackjack](https://github.com/Angphurba/Blackjack)
***
### Program details:

*WELCOME TO BLACKJACK GAME*

*Program auto generates two number.*

*Then, user have the choice to hit or stand.*

*If user enter hit:*
+ *Program generates third number which will be added to first and second number.*
+ *Displays new number.*
1. *If the new number is below 21, user have the choice to hit or stand.*
+ *If user enter hit again, the program repeat this process again.*
2. *If the new number exceeds 21, Computer wins.*

*If user enter stand:*
+ "Program generates two number.*
1. *If the generated number is below 16, Computer chooses to hit.*
+ *This process is repeated again.*

2. *If the number exceeds 21, Player wins.*

3. *If the number is above player number, and below or equal to 21, Computer wins.*


### C++ code block:
```c++ 
#include "iostream"
#include "stdlib.h" // for rand function

using namespace std;

int main()
{
	string player;
	int total, a1, a2, a3;
	char choice;
	{


		cout << " WELCOME TO BLACKJACK" << endl;

		a1 = rand() % 11 + 2; 
		cout << "Your first number is:" << a1 << endl;

		a2 = rand() % 11 + 2;
		cout << "Your second number is:" << a2 << endl;

		total = a1 + a2;

		cout << "Your total number is:" << total << endl;

		cout << "Do you want to hit (h) or stand (s):?";
		cin >> choice;

		if (total > 21)
		{
			cout << " Sorry! You lose." << endl;

			system("pause");
			exit(0);
		}

		if (choice == 'h')
		{
			a3 = rand() % 11 + 2;
			cout << " Your third number is: " << a3 << endl;

			total = total + a3;

			cout << " Your new total is: " << total << endl;

		}
		if (total > 21)
		{
			cout << " Sorry! You lose." << endl;

			system("pause");
			exit(0);
		}
	}


	if (choice == 's')
	{
		cout << " Dealer turn." << endl;
	}


	string dealer;
	int total2, b1, b2, b3;

	b1 = rand() % 11 + 2;
	cout << " Dealer first number is:" << b1 << endl;

	b2 = rand() % 11 + 2;
	cout << " Dealer second number is:" << b2 << endl;

	total2 = b1 + b2;

	cout << " Dealer total number is:" << total2 << endl;

	if (total2 > 21)
	{
		cout << " You win." << endl;

		system("pause");
		exit(0);
	}

	while (total2 < 16)
	{
		cout << " Dealer hit. " << endl;

		b3 = rand() % 11 + 2;

		cout << " Dealer third number is:" << b3 << endl;

		total2 = total2 + b3;

		cout << " Dealer new total is:" << total2 << endl;

		if (total2 > 21)
		{
			cout << " You win." << endl;

			system("pause");
			exit(0);
		}



		if (total > total2)
		{
			cout << "Player wins";
		}
		else
		{
			cout << "Dealer wins";
		}
	}
	system("pause");
	return 0;
}



```
### Console block:
```console

WELCOME TO BLACKJACK    

Your first number is:8                                                                                                                                 
Your second number is:12                                                                                                                               
Your total number is:20    

Do you want to hit (h) or stand (s):?s        

 Dealer turn.                                                                                                                                         
 Dealer first number is:8                                                                                                                              
 Dealer second number is:4                                                                                                                             
 Dealer total number is:12                                                                                                                             
 Dealer hit.         

 Dealer third number is:3                                                                                                                              
 Dealer new total is:15   

 Player wins Dealer hit.  

 Dealer third number is:6                                                                                                                              
 Dealer new total is:21                                                                                                                                                                                                                                                            
 Dealer wins       
          
```
         