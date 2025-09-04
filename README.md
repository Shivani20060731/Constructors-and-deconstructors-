# Constructors-and-deconstructors-


Constructors and Destructors

Aim

To study and implement Constructors and Destructors in C++.

Tools Used

VS Code

Programiz Online Compiler


Theory

Constructors in C++

A constructor is a special member function of a class that is automatically invoked when an object is created.

Its purpose is to initialize data members of the class.

Naming Rules:

Constructor has the same name as the class.

It does not have a return type (not even void).



Types of Constructors:

1. Default Constructor – Takes no arguments; initializes objects with default values.


2. Parameterized Constructor – Accepts arguments to initialize objects with specific values.


3. Copy Constructor – Creates a new object as a copy of an existing object.



Destructors in C++

A destructor is a special member function that is automatically invoked when an object goes out of scope or is deleted.
Its purpose is to free resources (memory, files, database connections, etc.).

Naming Rules:

Destructor has the same name as the class but is preceded by a tilde (~).

It does not take arguments and does not return anything.




Programs and Algorithms

Program-1: Default Constructor

Defines a class Marks with 5 subjects.

Constructor automatically asks for input at object creation.


Algorithm:

1. Define class Marks with five data members.


2. Inside constructor, take user input for marks.


3. In main(), create object → constructor executes automatically.



Program-2: Constructor Outside Class

Defines constructor outside the class.

Includes a display() function to show marks.


Algorithm:

1. Declare constructor in class, define it outside.


2. Take input for marks in constructor.


3. Define display() function.


4. In main(), create object → call display().




Program-3: Parameterized Constructor

Uses a constructor with parameters to set values at object creation.


Algorithm:

1. Define class Num with two integers.


2. Define Num(int a, int b) constructor to set values.


3. Define display() function.


4. In main(), create object with values (23, 78).




Program-4: Copy Constructor (Two Numbers)

Demonstrates object copying.


Algorithm:

1. Define class Num with two integers.


2. Create parameterized constructor.


3. Define copy constructor Num(const Num &n) → copy values.


4. Create n1 using parameterized constructor.


5. Create n2 as copy of n1.


6. Display both.




Program-5: Copy Constructor (Book Details)

Class Book with name, author, price.


Algorithm:

1. Define class Book with three members.


2. Define parameterized constructor → set values.


3. Define copy constructor → copy details from another book.


4. Define display() function.


5. In main(), take book details, create object b1.


6. Copy into b2 using copy constructor.


7. Display both.




Program-6: Destructor (Car Counter)

Uses static counter to track objects created/destroyed.


Algorithm:

1. Define static variable count = 0.


2. In constructor → increment count, print count.


3. In destructor → decrement count, print count.


4. In main(), create multiple objects inside and outside block scope.


5. Observe creation and destruction sequence.




Program-7: Destructor (No Explicit Constructor)

Shows destructors without user-defined constructor.


Algorithm:

1. Define class Date with destructor printing a message.


2. In main(), create objects outside and inside a loop.


3. Observe destructor call when objects go out of scope.




Conclusion

Constructors initialize data when objects are created.
Default constructors set default values, while parameterized constructors allow specific initialization.
Copy constructors enable duplicating object data safely.
Destructors handle cleanup when objects go out of scope.
Programs demonstrated object lifecycle:

Creation (constructor called)

Duplication (copy constructor)

Destruction (destructor called).
