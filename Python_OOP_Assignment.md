

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
       
       
       
       
       
       
