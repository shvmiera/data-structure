# Tutorial 1 
### Question 1
1. Each Java file/program must have one public class ( T / F )\
   True.
2. Each Java file/program can have as many non-public classes as you wish ( T / F )\
   True.
3. A class is a template for creating objects ( T / F )\
   True.
4. A class can only have data that describes the attributes of the objects ( T / F )\
   False.
5. A class can only have methods that describe the actions of the objects ( T / F )\
   False.
6. Name, address, birthdate, mood and weight can be object’s data ( T / F )\
   True.
7. We can use objects to access data and methods from a class ( T / F )\
   True.
8. Void methods must return a value ( T / F )\
    False.
9. Methods can receive parameters ( T / F )\
    True.
10. You can use System.out.println() only in the main() method ( T / F )\
    False.
### Question 2
The following codes are taken from a Java file/program called Tutorial1.java.  Only the codes inside the main() method and the output are given. Without changing the codes inside the main() method, write a suitable class so you may build the program and generate the intended output correctly and in order.

public class Tutorial1 {\
	public static void main(String[] args){

	// Create an object for class Person 
	Person person1 = new Person();
	person1.name = "Jack Sparrow";
	person1.age = 38;

	// Create a second object for class Person 
	Person person2 = new Person();
	person2.name = "Katy Perry";
	person2.age = 45;
	
	// Display
	System.out.println(person1.name);
	System.out.println(person2.age);
	}
}

Output:
Jack Sparrow\
45
