



Q76. Write a Python program to find the factorial of a given number.


		def fact_of_num(x):

		    count_var = 1
		    for i in range(1,x+1):
			count_var = count_var * i
		    return count_var


		output = fact_of_num(1)

		print('The factorial of number is: ',output)
		
		
Q77. Write a Python program to calculate the simple interest. Formula to calculate simple interest is SI = (PRT)/100

		pnpl_am = int(input('Enter the principal amount: '))
		rate_of_int = float(input('Enter the rate of interest '))
		time = int(input('Enter the time: '))

		output = (pnpl_am*rate_of_int*time)/100
		    
		print('The simple interest is:',output)
		
		
Q78. Write a Python program to calculate the compound interest. Formula of compound interest is A = P(1+ R/100)^t.

		pnpl_am = int(input('Enter the principal amount: '))
		rate_of_int = float(input('Enter the rate of interest '))
		time = float(input('Enter the time: '))

		output = pnpl_am*(pow(1+(rate_of_int/100),time))
		    
		print('The simple interest is:',output)
		

Q79. Write a Python program to check if a number is prime or not.

		def prime():

		    num = int(input('Enter the number to check if prime or not: '))
		    for i in range(2,num):
			if num % i == 0:
			    print('The entered number is not a prime number')
			    break
		    else:
			print('The entered number is a prime number')

		prime()


Q80. Write a Python program to check Armstrong Number.












