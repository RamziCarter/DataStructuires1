## Lab 1




![Prompt pt 1](https://raw.githubusercontent.com/RamziCarter/DataStructures1/main/Screenshot%202023-02-01%20001318.png)

![Prompt pt 2](https://raw.githubusercontent.com/RamziCarter/DataStructures1/main/Screenshot%202023-02-01%20001332.png)




```java
public interface attributes {
	
	
	
				
				 /**
				  * gets color of the car
				  * @return string of color if car has one assigned
				  */
				public String getColor();
				
				
				 /**
				  * gets Vehicle identification number of the car
				  * @return string of color if car has one assigned
				  */
				public String getVin();
				
				
				 /**
				  * gets make of the car
				  * @return make of car if car has one assigned
				  */
				public String getMake();
				
				
				 /**
				  * gets year of the car
				  * @return year car was made if car has one assigned
				  */
				public int getYear();
				
				
				
				
}

```

```java

public class Car implements attributes{
	
	
	String vin;
	String color;
	String make;
	int year;
	
	public Car (String vin, String color, String make, int year)
	{
		this.vin = vin;
		this.color = color;
		this.make = make;
		this.year = year;
	}
	
	public String getVin()
	{
		return vin;
	}
	
	public String getColor()
	{
		return color;
	}
	
	public String getMake()
	{
		return make;
	}
	
	public int getYear()
	{
		return year;
	}
	
	public String toString()
	{
		return "  vin: " + vin + "color: " + color + "make: " + make + "year: " + year + "\n";
	}
	
}

```


```java
import java.util.*;


public class carList extends Car   {

	
	public carList(String vin, String color, String make, int year) {
		super(vin, color, make, year);
		// TODO Auto-generated constructor stub
	}


	public static ArrayList<Car> randomizer(ArrayList<Car> cars, int x){
		
		for(int i = 0; i< cars.size(); i++)
		{
			if (cars.indexOf(i) % x ==0) 
				{
					cars.remove(cars.indexOf(i));
				}
			
		}
		return cars;
	}
	
	
	public static void main(String [] args) {
		
		// random objext
		Random rand = new Random ();
		// generate random number 0-9 
		int x = rand.nextInt(10);
				
		ArrayList <Car> cars = new ArrayList <Car>();
		
		// create 10 new car objects
		
		Car Car1 = new Car("JN1BF0AA0PM403335", "Black", "Nissan", 2023);
		
		Car Car2 = new Car("1G6KB5RS8KU130109", "Tan", "Cadillac", 2019);
		
		Car Car3 = new Car("1G1FX6S0XP4117585", "Gray Ghost Metallic", "Chevrolet", 2023);
		
		Car Car4 = new Car("1B3ER69E41V701370", "Viper Red Clearcoat", "Dodge", 2001);
		
		Car Car5 = new Car("1FA6P8R09N5554287", "Fighter Jet Gray", "Ford", 2022);
		
		Car Car6 = new Car("5FNYF6H80NB095165", "Crystal Black Pearl", "Honda", 2022);
		
		Car Car7 = new Car("1C4HJXFN1PW601579", "Bright White Clearcoat", "Jeep", 2023);
		
		Car Car8 = new Car("VF9SP3V34KM795215", "Black", "Bugatti", 2019);
		
		Car Car9 = new Car("242679B136769", "Orange", "Pontiac", 1969);
		
		Car Car10 = new Car("WMEFJ5DA0GK077457", "White", "Smart", 2016);
		
		cars.add(Car1);
		cars.add(Car2);
		cars.add(Car3);
		cars.add(Car4);
		cars.add(Car5);
		cars.add(Car6);
		cars.add(Car7);
		cars.add(Car8);
		cars.add(Car9);
		cars.add(Car10);
		
		randomizer(cars, x);
		System.out.print(cars.toString());

	}
}

```
