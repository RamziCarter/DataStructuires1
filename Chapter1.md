## Chapter 1


* Overview of Java key concepts
   * Classes
   * Methods
   * Variables
   * Calculations
   * Making decisions
   * Looping
   * Inptut (Keyboard)
   
* Program Design is Important
  * What must the program do?
  * What information do we need to know in order to print a bill?


![Sample Problem](https://raw.githubusercontent.com/RamziCarter/DataStructures1/main/Screenshot%202023-01-23%20163501.png)

```java
import java.text.DecimalFormat;
import java.util.*;


public class CoffeeSlip 
	{
	
	
	
		public static double total(double CoffeePrice, double sum, int numCups)
		{
			int x = 0;
			
			for(int i = 1; i <= numCups; i++)
			{
					x = x + 1;	
			}
			return x * CoffeePrice;
			
			
		}
		
		
		
		
		
		public static void main (String [] args)
			{
				double coffeePrice = 2.89;
				
				Scanner scan = new Scanner(System.in);
				System.out.print("How many cups of coffee would you like to purchase? ");
				int numCups = scan.nextInt();
				
				double sum =0;
				
				double result = total(coffeePrice, sum, numCups);
				
				if(result == 0)
					{
						System.out.println("The customer cancelled their order");
					}
				
				else 
					 {	
						double y = result * 0.09;
						result = result + y;
						DecimalFormat df = new DecimalFormat("#.##");
						result = Double.parseDouble(df.format(result));
						System.out.print("The total cost is: " + result);
					 }
				
			}

	}

```

* Readability
  * How easy is the program to understand?
    * Choose meaningful variable names
    * skip lines in code
    * comment on the program
    * Indenting blocks of code
    * use named constants rayther than hard coded numbers


* More Programming Ideas
  * Abstraction 
    * Focusing on more important details while ignoring unimportant details
  * Pre and post conditions
    * Used to verify that programs are correct
    * Java allows for assertions
  * Garbage collection
  * Encapsulation
    * Information hiding (public vs private)
    * Interface vs implementation
  * Overloading
    * Two methods that have the same name but DIFFERENT SIGNIATURE
    
``` java
public class MathUtils {
    public int sum(int x, int y) {
        return x + y;
    }

    public double sum(double x, double y) {
        return x + y;
    }
}

```

  * Overriding
    * Allows subclasses to customize the behavior of inherited methods
    * if a child class has a method with the same name as the parent class then the child class can override to make the method act differently

```java

public class Vehicle {
    public void drive() {
        System.out.println("Vehicle is driving");
    }
}

public class Car extends Vehicle {
    @Override
    public void drive() {
        System.out.println("Car is driving");
    }
}

```



---
Four Pillars of Object Oriented Programming


> Encapsulation
* information hiding
  * private vs public specifiers
* Interface vs Implementation


> Polymorphism
* used by method overloading an overriding
* An object knows how to act when called **In simple terms**

> Inheritance


> Abstraction
---
* Data Structurs Vs Abstract Data Types
  * Data Structure - a physical thing; you can see it inside the computer
  * ADT - just an idea 

---

#### Arrays

> an array is a gorup of data items that are all the same type

* Parallel Arrays

```java

String [] itemName = new [50]
String [] itemUPC = new [50]

```
* The danger with parallel arrays is that they are only connected in the programmers mind

---
#### Common Operations of ADT
* add / remove items
* check if full / empty
* count number of items
* check if a specific item is in the adt
* number of items
*number of one specific item

---

* Interfaces
  * a shell that contains the public methods
  * It contains only method headers, no actual code
``` 
Javadoc - a method of documentation
- all javadoc items are comments
- They start with /** and end with */
- It creates an HTML document containing 
  * a summary of the methods
```

  ![JavaDoc Example](https://raw.githubusercontent.com/RamziCarter/DataStructures1/main/Screen%20Shot%202023-05-07%20at%202.23.56%20PM.png)
 
  
  
  
  
