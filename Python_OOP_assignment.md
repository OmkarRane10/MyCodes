Q1. What is the purpose of Python's OOP?

    -> In Python, object-oriented Programming (OOPs) is a programming paradigm that uses objects and classes in programming.
       It aims to implement real-world entities like inheritance, polymorphisms, encapsulation, etc. in the programming.
       The main concept of OOPs is to bind the data and the functions that work on that together as a single unit so that no other part of the code can access this data.
       
Q2. Where does an inheritance search look for an attribute?

    -> An inheritance search looks for an attribute first in the instance object,
       then in the class the instance was created from, then in all higher superclasses, progressing from left to right (by default).
       
Q3. How do you distinguish between a class object and an instance object?

    -> A class is a template for creating objects in a program, whereas the object is an instance of a class.
       A class is a logical entity, while an object is a physical entity.
       A class does not allocate memory space; on the other hand, an object allocates memory space.
       
Q4. What makes the first argument in a class’s method function special?

    -> The first argument of every class method, including init , is always a reference to the current instance of the class.
       Any class method must have self as first argument. self represents an (arbitrary) instance of the class.
       So this self argument makes the class's method function special.
       
Q5. What is the purpose of the init method?

    -> The Default __init__ method is used as a Constructor in python class. Constructors are used to initializing the object’s state.
       The task of constructors is to initialize(assign values) to the data members of the class when an object of the class is created.
       Like methods, a constructor also contains a collection of statements(i.e. instructions) that are executed at the time of Object creation.
       It is run as soon as an object of a class is instantiated. The method is useful to do any initialization you want to do with your object.
       
Q6. What is the process for creating a class instance?

    -> We can create a instance of a class by calling a name of a class and assinging the same values in the argument as defined in the constructor method of that class.
       To create instances of a class, we call the class using class name and pass in whatever arguments its __init__ method accepts.
       for ex - class Person:
                    def __init__(self, name, age):
                    self.name = name
                    self.age = age
                    print('The name of person is: ',self.name)
                    print('The age of person is: ',self.age)
                 p1 = Person("John", 36)       # here p1 is the instance of class Person
                 
Q7. What is the process for creating a class?

    -> TO create a class in python we use a keyword 'class' followed by the classname we assign to a class and a colon.
       for ex - class Employee:
       
Q8. How would you define the superclasses of a class?

    -> A superclass is the class from which many subclasses can be created. The subclasses inherit the characteristics of a superclass.
       The superclass is also known as the parent class or base class.
       The superclass is defined at the moment when a child class is created using a exisitng class name in its definiton.
       for ex - class A:
                    def __init__(self,name):
                           self.name = name
              
                class B(A):
                    def __init__(self, bname):
                    super().__init__(bname)
                    print('The name of B person is: ', self.name)
                    
                b1  = B('Omkar')
       
Q9. What is the relationship between classes and modules?

    -> Modules are collections of methods and constants. They cannot generate instances like we create an instance of a class.
       Classes may generate instances (objects), and have per-instance state (instance variables).
       So a module in python is simply a way to organize the code, and it contains either python classes or just functions.
       If we need those classes or functions in our project, we just import them.
       For ex - the math module in python contains just a bunch of functions, and wejust call those whenever needed.
       
Q10. How do you make instances and classes?

    -> Code : class A:
    		  def __init__(self,name):
                      self.name = name
                      print('The name of A person is: ', self.name)
                   
              class B(A):
                  def __init__(self, bname):
			super().__init__(bname)
			print('The name of B person is: ',self.name)
		a1 = A('Omkar')
		b1 = B('Omkar')
	      
Q11. Where and how should be class attributes created?

     -> Class attributes belong to the class itself they will be shared by all the instances.
     	Such attributes are defined in the class body parts usually at the top, for legibility.
     	So the class atrributes are defined inside a class but outside a function so that every function in that class can use those class attributes.
     	
Q12. Where and how are instance attributes created?

     -> Instance attributes are defined in the constructor. They are defined directly inside a class.
        They are defined inside a constructor using the self parameter.
        
Q13. What does the term "self" in a Python class mean?

     -> The self parameter is a reference to the current instance of the class, and is used to access variables that belongs to the class.
     
Q14. How does a Python class handle operator overloading?

     -> Operator Overloading means giving extended meaning beyond their predefined operational meaning.
     	For example operator + is used to add two integers as well as join two strings and merge two lists.
     	It is achievable because ‘+’ operator is overloaded by int class and str class.
     	We have seen that the same built-in operator or function shows different behavior for objects of different classes, this is called Operator Overloading. 
     	
Q15. When do you consider allowing operator overloading of your classes?

     -> Python operators work for built-in classes. But the same operator behaves differently with different types.
        For example, the + operator will perform arithmetic addition on two numbers, merge two lists, or concatenate two strings.
	This feature in Python that allows the same operator to have different meaning according to the context is called operator overloading.
	So we can allow operator overloading in our classes when we want to perform different operations on different datatypes using the same operator.
	
Q16. What is the most popular form of operator overloading?

     -> A very popular and convenient example is the Addition (+) operator.
     	Just think how the '+' operator operates on two numbers and the same operator operates on two strings.
     	It performs “Addition” on numbers whereas it performs “Concatenation” on strings and also lists.
     	
Q17. What are the two most important concepts to grasp in order to comprehend Python OOP code?

     -> Encapsulation is wrapping the code and data together into a single unit. Class is an example of encapsulation, because it wraps the method and property.
        Abstraction is hiding internal details and showing functionality only. Abstraction focus on what the object does instead of how it does.
        Data abstraction and encapsulation are synonymous as data abstraction is achieved through encapsulation.
        Abstraction is used to hide internal details and show only functionalities.
        Abstracting something means to give names to things, so that the name captures the basic idea of what a function or a whole program does.
    
Q18. Describe three applications for exception processing.
     -> 1) When we provide a web form for users to fill in and submit.but incase there are a lot of conditions to be handled and the conditions keeps 		changing periodically,you use exception handling to simplify the process.
     	2) database connectivity uses exception handling, this is because the reason for database connectivity failure cannot be predicted and handled as 	  it can be caused by many variables such as power failure, unreachable server,failure at client front/back end and so on.
     	3) Arithmetic exceptions such as division by zero and so on.

Q19. What happens if you don't do something extra to treat an exception?

     -> When an exception occurrs and if we don't handle it, the program will br forced to terminate abruptly and the code past the line that caused the exception will not get executed.
	       
Q20. What are your options for recovering from an exception in your script?

     -> We can use exception handling in python to avoid the exceptions or be precautious from the exceptions that might get occured in our python script.
     	This can be achieved using try and except block to write our code in python. We can provide a generic except clause, which handles any exception.
     	After the except clause(s), we can include an else-clause. The code in the else-block executes if the code in the try: block does not raise an exception.
     	
Q21. Describe two methods for triggering exceptions in your script.

     -> In Python, exceptions can be handled by two new methods:
     	Try: Catches exceptions raised by Python or a program.
     	Raise: A custom exception that triggers an exception manually
     	
     	for ex - Try and except block to catch and raise the exception
			try:
			Your statements

			except Exception_1:
			If there is Exception_1 then execute this block- statement

			except Exception_2:
			If there is Exception_2 then execute this block-statement

			else:
			if no exception was raised-statement
			
	for ex - raise block of code to catch exception
			try:
			fp = open(‘myfile.txt’)
			line = f.readline()
			i = int(s.strip())

			except (IOError,ValueError) as e:
			print (“check if the file is read-only.”,e.errno)

			except:
			print (“Unexpected error”)

Q22. Identify two methods for specifying actions to be executed at termination time, regardless of whether or not an exception exists.

      -> The two methods which can be used to be executed at termination time, regardless of whether or not an exception exists are 'else' block and 'finally' block.
      	 Finally block always executes irrespective of an exception being thrown or not. The finally keyword allows to create a block of code that follows a try-catch block.

Q23. What is the purpose of the try statement?

      -> In Python, exceptions can be handled using a try statement. The critical operation which can raise an exception is placed inside the try clause.
      	 So we use try clause to write the code that might throw us an exception in the script.
      	 
Q24. What are the two most popular try statement variations?

      -> The two most popular try statement variations are as below.
      		1st variation - 
      		try:
      		    statements
      		except Exception_1:
      		    statements to be exectued when exception occurs
      		finally:
      		    statements to be executed regardless of the result of the try- and except blocks.
      		
		2nd variation - 
		try:
      		    statements
      		except Exception_1:
      		    statements to be exectued when exception occurs
      		else:
      		    statements to be executed when no error or exceptions occurs.
      		    
  
  
  I will complete and update the rest of the assignment once vishal's github repository is up again







	       
	       
	       
	       
	       
	       
	       
	       

