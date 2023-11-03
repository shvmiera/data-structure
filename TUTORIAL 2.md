# Tutorial 2
You are a new programmer working at the faculty. As your first job, you are given a list of registered students and asked to store each student as an object in Java. You are given a skeletal code below to get you started from the previous programmer. Of course, the code is INCOMPLETE and HAS ERRORS. You can ignore the code and start from zero if you wish to. 

| Name | Matric Id | Year |
|:----:|:---------:|:----:|
|Alexa |1007	     |  2		|		 
|Siri  |5018	     |  4		|		 
|Omega |2019	     |  1		|		 
|Beta	 |2371	     |  3		|		

## Question 1
**Task 1 : Registering students with setMethods.**

a) Create one class, 'Student', with variables matching the list's attributes. Your class should have to get and set methods for each attribute (Eg. setName, getName, setMatricId, getMatricId). Ensure suitable data types and access (public, private) are used. 

class Student{

	String name;
	setName(){
 
  }
  
	getName(){
	}	
 
}

public class Register {

    public static void main(String[] args) {
        
		student alexaObj = new alexa();
		alexaObj.setName();
		System.out.println(alexaObj.getName());
}

◤━━━━━━━━━━━━━━━━━━━━━━━━━━◥\
**ANSWER**\
class Student {
    
    String name;
    int MatricId, year;

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public long getMatricId() {
        return MatricId;
    }

    public void setMatricId(int MatricId) {
        this.MatricId = MatricId;
    }
    
    public int getYear() {
        return year;
    }

    public void setYear(int year) {
        this.year = year;
    }

}\
◣━━━━━━━━━━━━━━━━━━━━━━━━━━◢

b) Now instantiate the object student according to the list that you have been given. You should have 4 objects corresponding to 4 students on the list.

◤━━━━━━━━━━━━━━━━━━━━━━━━━━◥\
**ANSWER**\
public class Register {

    public static void main(String[] args) {
        System.out.println("Name\t\tMatric ID\t\tYear");
        
        Student alexaObj = new Student ();
        Student siriObj = new Student ();
        Student omegaObj = new Student ();
        Student betaObj = new Student ();     
    }

}\
◣━━━━━━━━━━━━━━━━━━━━━━━━━━◢

c) Using the set methods, set the attributes of each student in each object. I.e. if your object for alexa is called alexaObj then alexaObj.setName();

◤━━━━━━━━━━━━━━━━━━━━━━━━━━◥\
**ANSWER**\
public class Register {

    public static void main(String[] args) {

        System.out.println("Name\t\tMatric ID\t\tYear");
        
        Student alexaObj = new Student ();
	alexaObj.setName("Alexa");
        alexaObj.setMatricId(1007);
        alexaObj.setYear(2);
	
        Student siriObj = new Student ();
        siriObj.setName("Siri");
        siriObj.setMatricId(5018);
        siriObj.setYear(4);
        
        Student omegaObj = new Student ();
        omegaObj.setName("Omega");
        omegaObj.setMatricId(2019);
        omegaObj.setYear(1);

        Student betaObj = new Student ();
        betaObj.setName("beta");
        betaObj.setMatricId(2371);
        betaObj.setYear(3);
     
    }

}\
◣━━━━━━━━━━━━━━━━━━━━━━━━━━◢

d) In your main() method, get the info for each object and print it out. The output should look like the given list.

◤━━━━━━━━━━━━━━━━━━━━━━━━━━◥\
**ANSWER**\
class Student {
    
    String name;
    int MatricId, year;

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public long getMatricId() {
        return MatricId;
    }

    public void setMatricId(int MatricId) {
        this.MatricId = MatricId;
    }
    
    public int getYear() {
        return year;
    }

    public void setYear(int year) {
        this.year = year;
    }

}
    
public class Register {

    public static void main(String[] args) {

        System.out.println("Name\t\tMatric ID\t\tYear");
        
        Student alexaObj = new Student ();
	alexaObj.setName("Alexa");
        alexaObj.setMatricId(1007);
        alexaObj.setYear(2);
	System.out.println(alexaObj.getName() + "\t\t  " + alexaObj.getMatricId() + "\t\t\t " + alexaObj.getYear());

        Student siriObj = new Student ();
        siriObj.setName("Siri");
        siriObj.setMatricId(5018);
        siriObj.setYear(4);
        System.out.println(siriObj.getName() + "\t\t  " + siriObj.getMatricId() + "\t\t\t " + siriObj.getYear());
        
        Student omegaObj = new Student ();
        omegaObj.setName("Omega");
        omegaObj.setMatricId(2019);
        omegaObj.setYear(1);
        System.out.println(omegaObj.getName() + "\t\t  " + omegaObj.getMatricId() + "\t\t\t " + omegaObj.getYear());
        
        Student betaObj = new Student ();
        betaObj.setName("beta");
        betaObj.setMatricId(2371);
        betaObj.setYear(3);
        System.out.println(betaObj.getName() + "\t\t  " + betaObj.getMatricId() + "\t\t\t " + betaObj.getYear());
        
    }

}\
◣━━━━━━━━━━━━━━━━━━━━━━━━━━◢

## Question 2
**Task 2 : Registering students using one constructor.**

a) As you might have noticed, the code is long when using set methods to instantiate object results. As a brilliant programmer, you think, "I bet I can code shorter (more elegant) using constructors!". Your predecessor's attempt to use a constructor is given below. Your constructor should take in all parameters as in the list.

class Student{
	
	String name;
	 
	setName(){
	 }

	getName(){
	}
	
	showInfo(){
	
	System.out.println(name,matricId,..); // you are free to print in any way you prefer.
	
	}
	
	
}

public class Register {

    public static void main(String[] args) {
        
		String name;
		double matricId;
		
		public void constructor(String name, double matricId){
		  name =  name
		  matricId = matricId
		}
		
		student alexisObj = new alexis("Alexa","0007");
		student siriObj = new student("Siri","5018");
			   
	   
	}
}

◤━━━━━━━━━━━━━━━━━━━━━━━━━━◥\
**ANSWER**\
class Student{
	
    String name;
    int MatricId, year;

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getMatricId() {
        return MatricId;
    }

    public void setMatricId(int MatricId) {
        this.MatricId = MatricId;
    }

    public int getYear() {
        return year;
    }

    public void setYear(int year) {
        this.year = year;
    }

    
    public Student (String name, int MatricId, int year) {
        this.name = name;
        this.MatricId = MatricId;
        this.year = year;
    } 
            
    public void showInfo() {
	System.out.println(name + "\t\t  " + MatricId + "\t\t\t " + year);	
    }
    
    
}

public class Register {

    public static void main(String[] args) {
        
        System.out.println("Name\t\tMatric ID\t\tYear");
        
	Student alexaObj = new Student ("Alexa", 1007, 2);
	Student siriObj = new Student ("Siri", 5018, 4);
        Student omegaObj = new Student ("Omega", 2019, 1);
        Student betaObj = new Student ("Beta", 2371, 3);

        alexaObj.showInfo();
        siriObj.showInfo();
        omegaObj.showInfo();
        betaObj.showInfo();
			      
    }
}\
◣━━━━━━━━━━━━━━━━━━━━━━━━━━◢

b) What is the difference between registering students using task 1 and task 2?

◤━━━━━━━━━━━━━━━━━━━━━━━━━━◥\

**ANSWER**

The difference between registering students using task 1 and task 2 is that task 1 does not utilize a constructor, which results in longer code that can potentially lead to more errors. In task 1, we print out the details for each student using getter and setter methods. In contrast, task 2 employs a constructor, which shortens the code. This constructor accepts the student's name, MatricId, and year as parameters. We also create a method called showInfo() to print out the student's details. As the saying goes, 'the shorter the code, the better.

◣━━━━━━━━━━━━━━━━━━━━━━━━━━◢

c) What does Java do if a constructor is not specified?

◤━━━━━━━━━━━━━━━━━━━━━━━━━━◥

**ANSWER**

If a constructor is not specified, Java will automatically provide a no-args constructor. However, if you define a constructor in a class, Java will not provide a default constructor.

◣━━━━━━━━━━━━━━━━━━━━━━━━━━◢

d) Do you need set methods (e.g. setName method) if you can set using a constructor? 

◤━━━━━━━━━━━━━━━━━━━━━━━━━━◥

**ANSWER**

No, if you can set attributes using a constructor, set methods like setName are not necessary.

◣━━━━━━━━━━━━━━━━━━━━━━━━━━◢

e) The faculty staff told you that the list has errors. It should be like below. Make the necessary changes (you cannot use siriObj.name = "Sirius"..etc) and print out your answer like below.

| Name | Matric Id | Year |
|:----:|:---------:|:----:|
|Alexa |1007	     |  2		|		 
|Siri  |5018	     |  4		|		 
|Omega |2020         |  1		|		 
|Beta  |2371	     |  4		|		

◤━━━━━━━━━━━━━━━━━━━━━━━━━━◥\
**ANSWER**\
class Student{
	
    String name;
    int MatricId, year;

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getMatricId() {
        return MatricId;
    }

    public void setMatricId(int MatricId) {
        this.MatricId = MatricId;
    }

    public int getYear() {
        return year;
    }

    public void setYear(int year) {
        this.year = year;
    }

    
    public Student (String name, int MatricId, int year) {
        this.name = name;
        this.MatricId = MatricId;
        this.year = year;
    } 
            
    public void showInfo() {
	System.out.println(name + "\t\t  " + MatricId + "\t\t\t " + year);	
    }
    
    
}

public class Register {

    public static void main(String[] args) {
        
        System.out.println("Name\t\tMatric ID\t\tYear");
        
	Student alexaObj = new Student ("Alexa", 1007, 2);
	Student siriObj = new Student ("Siri", 5018, 4);
        Student omegaObj = new Student ("Omega", 2020, 1);
        Student betaObj = new Student ("Beta", 2371, 4);

        alexaObj.showInfo();
        siriObj.showInfo();
        omegaObj.showInfo();
        betaObj.showInfo();
			      
    }
}\
◣━━━━━━━━━━━━━━━━━━━━━━━━━━◢

## Question 3
**Task 3 : Registering students using multiple 'unchained' constructors.**
a) There are some new additions to the list below. As you can see, this time, the information is incomplete. Therefore, create multiple constructors to initialise different objects with different info.

