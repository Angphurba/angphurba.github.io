---
title: "Story Game"
date: 2019-01-01
tags: [Python]
header: 
   teaser: /images/python.jpg
excerpt: "Python"
---

#### [Story Game](https://github.com/Angphurba/storyGame) 
***
### Game details:

*Generates short funny story.*

*Player have to enter noun, city, number, and so on.*

### Python code block:
```python 
   def story_game():

    noun = input("Enter a noun:")
    city = input("Enter a city:")
    number = int(input("Enter a number:"))
    time = input("Enter day/month/year:")
    first_adjective = input("Enter a adjective:")
    second_adjective = input("Enter a second adjective:")
    name = input("Enter a persons name:")
    cloth =input("Enter a type of clothing:")
    color= input("Enter a color:")
    
    print ("_________________________________________________________________")
    print ("\nIt is a little known fact that",noun,"have been watching",city,"for",number,time,".")
    print ("\nOnly the" ,first_adjective, "people believed that it was just a matter of time before",noun,"invaded the", second_adjective, "city of", city, ".\n")
    print (name,",who was a", first_adjective, "person tried to warn the people, telling them their best defense was to hang",cloth, "from the trees and", color, "shoes on every door knob.")
    print ("\nUnfortunately no one believed", name, "and when",noun, "attacked", city, ",only the", first_adjective, "people survived.")
    print ("_________________________________________________________________")
    
    print ("\nWould you like to play the game again?")
    ans = input("Enter your decision(Y or N):")
    if ans in ("Y","y"):
        story_game();
    else:
        print ("Thank you.")
story_game();
```
### Console block:
```console
Enter a noun:Ang                                                                                                                                     
Enter a city:New York                                                                                                                                
Enter a number:7                                                                                                                                     
Enter day/month/year:year                                                                                                                            
Enter a adjective:fluffy                                                                                                                             
Enter a second adjective:skinny                                                                                                                      
Enter a persons name:Sheldon                                                                                                                         
Enter a type of clothing:tshirt and pant  
Enter a color:white and black
```
________________________________________________________________                                                                                                                                              
It is a little known fact that Ang have been watching New York for 7 year .                                                                          
                                                                                                                                                     
Only the fluffy people believed that it was just a matter of time before Ang invaded the skinny city of New York .      

Sheldon ,who was a fluffy person tried to warn the people, telling them their best defense was to hang tshirt and pant from the trees and white and b
lack shoes on every door knob.                                                                                                                       
                                                                                                                                                     
Unfortunately no one believed Sheldon and when Ang attacked New York ,only the fluffy people survived.                                               
_________________________________________________________________                                                                                    
                                                                                                                                                     
Would you like to play the game again?                                                                                                               
Enter your decision(Y or N):      
```          