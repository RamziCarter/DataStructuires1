## Chapter 2

> UML- Unitfied Modeling Language
* a way to pictorally describe a class



**Part 1**
* name


**Part 2**
* attributes



**Part 3**
* methods

> Common practice to use (+) for public items and (-) for private items

![UML Visual](https://raw.githubusercontent.com/RamziCarter/DataStructures1/main/Screen%20Shot%202023-05-07%20at%202.32.01%20PM.png)
---

```java
Problem: Find a data structure to represent a shopping bag ADT
* Requirements of the ADT (Bag)
  * needs methods to operate the bag
  * need to decide what will be done to the items in the bag

**Attempt 1**


* use arrays to implement the bag

4 parallel array to display the attributes like name of item, store product code, number of items in stock and price

String [] name = new String [100];
String [] productCode = new String [100];
int [] stock = new int [100];
double [] price = new double[100];

The issue with this is that the items are not connected within the program only in the designers mind. And updating the arrays is tedious and it is not dynamic. To solve this we can create a class


**Attempt 2**

Public Class Grocery
{
    private String name;
    private int stock;
    private String productCode;
    private int price;
    
    
    
    public Grocery(String ItemName, String ItemProductCode, int ItemStock, int ItemPrice)
    {
     name = ItemName;
     productCode = ItemProductCode;
     stock = ItemStock;
     price = ItemPrice;
     
     
    }
}


// with this class we can create an array of type Grocery to represent a bag

Grocery [] bag = new Grocery[10]; // 1 items per bag; so this is 10 bags



```





Array List
> you can add / remove items onto the data structure
> It is dynamic 
> you can also insert at specific locations

* you need an import statement: java.util.ArrayList
* uses a wrapper class for the TYPE of thing you want to input into the list
* ArrayList <String> myList = new ArrayList <String>();
  * myList.add("California");
  * myList.add(2, "Florida");
    * add at specific location (Insert)

 
 
