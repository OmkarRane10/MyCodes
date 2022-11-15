
Q1. Why do we call Python as a general purpose and high-level programming language?

-> Python is an object-oriented, high-level programming language.
  Object-oriented means this language is based around objects (such as data) rather than functions, and high-level means it's easy for humans to understand.
  Python is a general-purpose language because it can be used to create a variety of different programs and isn't specialized for any specific problems.
  Such languages are easier and more natural for people to use than machine code or assembly language, which require knowledge of details that are hidden from the user by the High level lanuage as pyhton.

Q2. Why is Python called a dynamically typed language?

-> Python is called a dynamically typed language because Dynamic typing means that the type of the variable is determined only during runtime.
Python stores the value of a variable at some memory location and then binds that variable name to that memory container and makes the contents of the container accessible through that variable name.
So the data type does not matter. As it will get to know the type of the value at run-time.

Q3. List some pros and cons of Python programming language?

-> Pros of python language:
    - Beginner-friendly: Python is an excellent platform for beginners who want to step into coding. This programming language is easy to learn, understand and code.
    - Large Community: The Python community boasts many coders, developers, professionals, and students on the same platform as it is free and opens source language
    - Extensive Libraries: Python features an extensive set of libraries and contains code for various purposes. Hence, it eliminates the need to write the complete code manually.
    - Flexible and Extensible: Python is extremely flexible and can be extended to other languages. Developers can write code in C  and C++ and build new features in the dynamically-typed language.
    - Portable: Python is portable, which means it can be run on any other platform. Here, you need to code only once, and you can run it anywhere.
-> Cons of python language:
    - Issues with Design: Python developers sometimes have to deal with complicated designs. Therefore, highly efficient and experienced developers are preferred over beginners.
    - Slower than Compiled Languages: Python is slow compared to other non-compiled languages as it requires a lot of computational power.
    - Security: Python is not 100% secure. You need to take the necessary steps to ensure the code’s security.
    - Dynamically Typed: There is a chance of lot of errors and bugs in the system than the statically typed language.
    - High memory consumption: Python language comes with high memory usage. It uses reference counting in its garbage collection, which often leads to potential memory losses.
    
 Q4. In what all domains can we use Python?
 
 -> Pyhton is used extnesively in below domains:
    - Data science
    - Automation
    - Application Development
    - AI and machine learning
    - Audio/Video applications
    - Console Applications
    
 Q5. What are variable and how can we declare them?
 
  -> A variable is a container where we can store a value. We can directly declare a variable using an alphabet or letters and assignment operator(=).
  Variables do not need to be declared with any particular type, and can even change type after they have been set.
  ex- int x=10, float y = 40.65, abc = "myname"
  
 Q6. How can we take an input from the user in Python?
 
  -> We can take inputs in python using a funcation called as input() function.
   for ex - name = input("Enter your name : ")
   
 Q7. What is the default datatype of the value that has been taken as an input using input() function?
 
  -> The default datatype of the value that has been taken as an input by using the input function is the 'String' datatype.
  
 Q8. What is type casting?
 
  -> Type casting is the method used to convert the datatype of any variable in python. There are different methods to convert the datatypes.
  for ex- int(), float(), str(),etc
  
 Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?
  -> Yes, we can take more than one input from the user using single input function. 
  For this purpose we need to use one more function with the input function which is called as split function.
  Here when the input is given by the user, the user needs to enter the values separated by a space so that it could be idnetifies as a different value entered.
  For ex- a, b = input("Enter two values: ").split()  
          print("Enter Your First Name: ", a)  
          print("Enter Your Last Name: ", b)
          
 Q10. What are keywords?
 
  -> Python keywords are special reserved words that have specific meanings and purposes and can't be used for anything but for those specific purposes.
 for ex- int, float, for, if, elif, else, etc
  
 Q11. Can we use keywords as a variable? Support your answer with reason.
 
  -> No, we cannot use keywords as a variable. Keywords define the language's syntax rules and structure, and they cannot be used as variable names.
  If we use any of the keywords as variable it will throw us a syntax error.
  
 Q12. What is indentation? What's the use of indentaion in Python?
 
  -> Python indentation refers to adding white space before a statement to a particular block of code.
  In another word, all the statements with the same space to the right, belong to the same code block.
  Python indentation is a way of telling a Python interpreter that the group of statements belongs to a particular block of code.
  A block is a combination of all these statements.Block can be regarded as the grouping of statements for a specific purpose.
  It is also convenient and useful for a programmer or viewer who is working on the code to identify that which statments belongs to the particular block   of code.
  
 Q13. How can we throw some output in Python?
 
  -> We can throw a output in python using print() function.
  ex - print('This is sample output')
 
 Q14. What are operators in Python?
  
  -> Operators are used to perform operations on variables and values in python.
  Some of the operators used in python are arithmetic opearators, assignment operators, comparison operators, logical operators,etc.
  
 Q15. What is difference between / and // operators?
 
  -> (/) operator is used for the float division and (//) operator is used for integer divison.
  Generally (//) operaoter is used to ignore the decimal values.
  
 Q16. Write a code that gives following as an output. O/P(iNeuroniNeuroniNeuroniNeuron)
 
  -> x = "iNeuron"
     x *= 4
     print(x)
     
 Q17. Write a code to take a number as an input from the user and check if the number is odd or even.
 
  -> x = int(input('Enter a number: '))
     if x%2==0:
         print('The entered number is a even number')
     else:
         print('The entered number is a odd numner')
         
  Q18. What are boolean operator?
  
   -> Boolean Operators are those operators that result in the Boolean values of True and False. Here Logical check will happen for expression result.
       ex - and,or and not operators.
         and -> Returns true if both statements are true 
          or -> Returns true if one of statements are true
         not -> Reverse the result, returns false if the result is true
         
  Q19. What will the output of the following?
     1 or 0 ----> 1 (as for 'or' opearator if one value is true then the result will be true)

     0 and 0 ---> 0 (as for 'and' opearator if both the values are true then the result will be true)

     True and False and True ---> False (as in 'and' operator if one value is also false then the result becomes false)

     1 or 0 or 0 ---> 1 (as for 'or' opearator if one value is true then the result will be true)
     
  Q20. What are conditional statements in Python?
  
    -> A conditional statement is used to handle conditions in a program.
    These statements guide the program while making decisions based on the conditions encountered by the program.
    Python has 3 key Conditional Statements: if statement. if-else statement and else statement.
    
  Q21. What is use of 'if', 'elif' and 'else' keywords?
  
    -> These keywords are used to execute a set of statements or a block of code based on the conditions declared with those keywords.
    
  Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".
  
    -> age = int(input('Enter your age: '))
          if age>=18:
              print('I can vote')
          else:
              print("I can't vote")
              
   Q23. Write a code that displays the sum of all the even numbers from the given list.
   
    -> numbers = [12, 75, 150, 180, 145, 525, 50]
       sum=0
       for i in numbers:
           if i%2==0:
               sum=sum+i
        
       print(sum)
       
   Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.
   
    -> a=int(input("Enter the first number: "))
       b=int(input("Enter the second number: "))
       c=int(input("Enter the third number: "))

       if a>b and a>c:
            print("The highest number is: ",a)
       elif b>a and b>c:
            print("The highest number is: ",b)
       else:
            print("The highest number is: ",c)
            
    Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]

          ---->> Code :
                      numbers = [12, 75, 150, 180, 145, 525, 50]
                        for i in numbers:
                            if i > 500:
                                break
                            if i%5==0:
                                if i > 150:
                                    continue
                                else:
                                    print(i)
                                           
                                           
                                           
          
