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

Output:\
Jack Sparrow\
45

**ANSWER**\
class Person {\
String name;\
int age;\
}

### Question 3
Extend Tutorial1.java with additional information to the class person.

public class Tutorial1 {\
	public static void main(String[] args){

	// Create a Person object using the Person class
	Person person1 = new Person();
	person1.name = "Jack Sparrow";
	person1.age = 38;

	// Create a second Person object using the Person class
	Person person2 = new Person();
	person2.name = "Katy Perry";
	person2.age = 45;
	
	// Display
	// System.out.println(person1.name);
	// System.out.println(person2.name);
	System.out.println(person1.sayHello);
	System.out.println(person2.sayHello);
	System.out.println(person1.speak);
	System.out.println(person1.calculateYearsToRetirement);
	System.out.println(person2.speak);
	System.out.println(person2.calculateYearsToRetirement);	
	}
}

Output:\
This is your Captain Jack Sparrow saying Oh-hoyyy!\
This is your Captain Katy Perry saying Oh-hoyyy!\
I am Jack Sparrow, 38 years old this year mate.\
I am retiring in 22 years.\
I am Katy Perry, 45 years old this year mate.\
I am retiring in 15 years.

**ANSWER**\

class Person {
    
    String name;
    int age;
    
    Person (String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String sayHello () {
        return "This is your Captain " + this.name + " saying Oh-hoyyy!";
    }
   
    public String speak () {
        return "I am " + this.name + ", " + this.age + " years old this year mate.";
    }
        
    public int retirement () {
        return 60 - this.age;
    }
     
    public String calculateYearsToRetirement () {
        int yearstoretire = retirement(); // calling the method retirement()
        return "I am retiring in " + yearstoretire + " years";
    }
    
}

public class Tutorial1 {\
    public static void main(String[] args) {
        
	// Create an object for class Person
	Person person1 = new Person("Jack Sparrow", 38);
	// Create a second object for class Person
	Person person2 = new Person("Katy Perry", 45);
	
	// Display
        System.out.println(person1.sayHello());
        System.out.println(person2.sayHello());
        System.out.println(person1.speak());
        System.out.println(person1.calculateYearsToRetirement());
        System.out.println(person2.speak());
        System.out.println(person2.calculateYearsToRetirement());
        
    }
}

### Question 4
The following is something we have not covered in the lecture. But it should be doable for you to figure it out. Similarly, you are given the main() method codes and some output. Figure out the complementary class to build the code and display the correct output. 
Tips: look into method parameters or passing of arguments as method parameters. You can ask Lecturer and Demo to explain if you don't understand.

public class Tutorial2 {

	public static void main(String[] args){

	Frog sam = new Frog();

	sam.speak("Hi, I am Sam");
	sam.jump(7);
	sam.move("West", 5.5);
	
	String greeting = "Good morning!";
	sam.speak(greeting);
	
	}
}

Output:\

Hi, I am Sam.\
Jumping 7cm 1 time!\
Jumping 7cm 2 time!\
Jumping 7cm 3 time!\
Moving 5.5 meters in the West direction.\
Good morning!

