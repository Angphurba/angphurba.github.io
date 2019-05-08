---
title: "Inventory"
date: 2019-01-03
tags: [Python]
header: 
   teaser: /images/python.jpg
excerpt: "Python"
---

#### [Home Secuirty Supply](https://github.com/Angphurba/Inventory) 
***
### Program details:

*Internal company inventory program.*

1. *Lets user add: 
+ *New product*
+ *Quantiy* 
+ *Price*

2. *Displays inventory in table form:*
+ *Product name*
+ *Quantiy*
+ *Price* 
+ *Amount (Quantity*Price)*

3. *Prints report:*
+ *Total number of item.*
+ *Total price of the product.*
+ *Total amount.*


### Python code block:
```python 
item=[] 
product=0
number=0
total_price=0
total_amount=0
total_quantity=0

while(number!=4):
  number=int(input("\nHome Security Supply\n 1. Add to Inventory\n 2. View Inventory\n 3. Product Report\n 4. Exit\n"))
  
  if(number==1):
      product=int(input("\nEnter number of different product to add:"))
      for i in range(0,product):
         name=input("\nEnter product name:")
         each=int(input("Enter quantity:"))
         price=int(input("Enter price of the product:$"))
         amount=(each*price)
         print("Total amount of the product:$",amount)
         item.append([name,each,price,amount]) 
  
  if(number==2):
      print("Product\tPiece\tPrice\tAmount\n")
      for i in range(0,product): 
         print(item[i][0],"\t",item[i][1],"\t",item[i][2],"\t",item[i][3],"\n")
  
  if(number==3):
      for i in range(0,product):
        total_quantity+=item[i][1]
        total_price+=item[i][2]
        total_amount+=item[i][3]
      print("Total item = ",total_quantity,"\nTotal price = ",total_price,"\nTotal Amount = ",total_amount)
```
### Console block:
```console
Home Security Supply                                                                                                                                   
 1. Add to Inventory                                                                                                                                   
 2. View Inventory                                                                                                                                     
 3. Product Report                                                                                                                                     
 4. Exit                                                                                                                                               
1                                                                                                                                                      
                                                                                                                                                       
Enter number of different product to add:2                                                                                                             
                                                                                                                                                       
Enter product name:CCTV                                                                                                                                
Enter quantity:2                                                                                                                                       
Enter price of the product:$150                                                                                                                        
Total amount of the product:$ 300                                                                                                                      
                                                                                                                                                       
Enter product name:Alarm                                                                                                                               
Enter quantity:1                                                                                                                                       
Enter price of the product:$45                                                                                                                         
Total amount of the product:$ 45                                                                                                                       
                                                                                                                                                       
Home Security Supply                                                                                                                                   
 1. Add to Inventory                                                                                                                                   
 2. View Inventory                                                                                                                                     
 3. Product Report  
 4. Exit                                                                                                                                               
2                                                                                                                                                      
Product Piece   Price   Amount                                                                                                                         
                                                                                                                                                       
CCTV     2       150     300                                                                                                                           
                                                                                                                                                       
Alarm    1       45      45                                                                                                                            
                                                                                                                                                       
                                                                                                                                                       
Home Security Supply                                                                                                                                   
 1. Add to Inventory                                                                                                                                   
 2. View Inventory                                                                                                                                     
 3. Product Report                                                                                                                                     
 4. Exit                                                                                                                                               
3                                                                                                                                                      
Total item =  3                                                                                                                                        
Total price =  195                                                                                                                                     
Total Amount =  345                                                                                                                                    
                                                                                                                                                       
Home Security Supply                                                                                                                                   
 1. Add to Inventory                                                                                                                                   
 2. View Inventory     
 3. Product Report                                                                                                                                     
 4. Exit                                                                                                                                               
4                                                                                                                                                      
                                                                                                                                                       
                                                                                                                                                       
...Program finished with exit code 0                                                                                                                   
```
