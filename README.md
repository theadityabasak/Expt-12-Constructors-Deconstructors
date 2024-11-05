# Constructors-Deconstructors
# App USed: VS Code
# Theory
## Constructors Defination:
Constructor in C++ is a special method that is invoked automatically at the time an object of a class is created. It is used to initialize the data members of new objects generally. The constructor in C++ has the same name as the class or structure. It constructs the values i.e. provides data for the object which is why it is known as a constructor.

## Syntax of Constructors in C++
The prototype of the constructor looks like this: (){ ... }

## Properties of Constructors:
The name of the constructor is the same as its class name.
Constructors are mostly declared in the public section of the class though they can be declared in the private section of the class.
Constructors do not return values; hence they do not have a return type.
A constructor gets called automatically when we create the object of the class.
You can overload constructors in a class, meaning you can have multiple constructors with different parameter lists.
If no constructor is explicitly defined, the compiler provides a default constructor that initializes data members to default values.
A special constructor that initializes an object using another object of the same class. It is often used for deep copying.
Constructors can take parameters to initialize objects with specific values.
Advantages of Constructors:
Automatic Initialization: Constructors ensure that an object is initialized to a valid state when it is created. This reduces the chances of encountering uninitialized data.
Encapsulation of Initialization Logic: They encapsulate the logic required to set up an object, making the code cleaner and more maintainable.
Support for Overloading: By allowing multiple constructors with different parameter lists, constructors provide flexibility in object creation.
Initialization of Complex Objects: Constructors can be used to initialize complex objects, including those involving dynamic memory allocation.
Consistency: Using constructors helps maintain consistency in object initialization. It ensures that every object of a class starts life in a well-defined state.
Resource Management: Constructors can handle resource allocation, such as memory or file handles, ensuring that resources are properly allocated when an object is created.
Compatibility with Class Hierarchies: Constructors support initialization in class hierarchies. Base class constructors are called before derived class constructors, allowing for proper setup of inherited properties.
Avoiding Redundant Code: They help avoid redundant initialization code by centralizing it in the constructor rather than spreading initialization code across various parts of the program.

# Algorithms
## 1. Date class
Start
Define date Class
int d (Day)
int m (Month)
int y (Year)
Define public members:
Constructor date()
Output: "Constructor called"
Initialize d to 4
Initialize m to 9
Initialize y to 2024
Method display()
Output: "Today's date is: d/m/y" where d, m, and y are the values of day, month, and year. Main Function (main())
Create an object mydate of class date
The constructor date() is automatically called.
Call mydate.display()
This displays the date initialized in the constructor.
End
## 2. Constructors outside class
Start
Define Student Class
Declare private members:
int rno (Roll number)
char name[50] (Name)
double fee (Fee)
Define public members: 3.Constructor Student()
Prompt the user to enter rno, name, and fee.
Read the values from user input.
Method display()
Print the rno, name, and fee. Main Function (main())
Create an object s of class Student
The constructor Student() is called automatically.
The constructor prompts the user for input and initializes the object with these values.
Call s.display()
This method displays the values of rno, name, and fee that were initialized by the constructor.
End
## 3.Copy Constructors 
Start

Define Wall Class

Declare private members:
double length (Length of the wall)
double height (Height of the wall)
Define public members:
Constructor Wall(double len, double hgt)

Initialize length with len.
Initialize height with hgt.
Copy Constructor Wall(const Wall& obj)

Initialize length with obj.length.
Initialize height with obj.height.
Method calculateArea() const

Calculate and return the area of the wall as length * height. Main Function (main())
Create an object wall1 of class Wall with 10.5 and 8.6 as arguments.

The constructor Wall(double len, double hgt) initializes length to 10.5 and height to 8.6.
Create another object wall2 using the copy constructor by copying wall1.
The copy constructor initializes wall2 with the same length and height as wall1. 7.Call wall1.calculateArea()
This calculates and prints the area of wall1.
Call wall2.calculateArea()
This calculates and prints the area of wall2, which should be the same as wall1.
End
Algorithm for Construct Class Program
Start
Define Construct Class
Declare private members:
int a (An integer variable)
int b (Another integer variable)
Define public members:
Default Constructor Construct()
Initialize a with 10.
Initialize b with 20.
Method display()
Calculate the sum of a and b.
Print the result as "Addition result is: " followed by the calculated sum.
Main Function (main())
Create an object myconstruct of class Construct
The default constructor Construct() is called.
This initializes a to 10 and b to 20.
Call myconstruct.display()
This method calculates the sum of a and b and prints "Addition result is: 30".
End
Algorithm for Student Class with Object Count
Start

Global Variable Declaration:

Declare a global integer variable count initialized to 0.
This variable keeps track of the number of Student objects currently active.
Define Student Class

Constructor Student()
Increment the count variable by 1.
Print the current number of objects created.
Destructor ~Student()
Decrement the count variable by 1.
Print the current number of objects destroyed.
Main Function (main())

Create objects aa, bb, and cc of class Student
Each object creation calls the Student() constructor.
The constructor prints the number of objects created after each object is created.
Create a block of code:
Within this block, create an object dd of class Student.
This calls the Student() constructor, incrementing the count.
When the block ends, dd goes out of scope.
The Student() destructor is called for dd, decrementing the count.
End

# Conclusion
We learnt to use the concepts of Constructors and Deconstructors.
