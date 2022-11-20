

  Q76. Write a Python program to find the factorial of a given number.

      -> Code :def fact_of_num(x):

    count_var = 1
    for i in range(1,x+1):
        count_var = count_var * i
    return count_var


output = fact_of_num(1)

print('The factorial of number is: ',output)
