



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



Q81. Write a Python program to find the n-th Fibonacci Number.

		n = int(input('Enter a number to find the fibonacci: '))

		def fib(n):
		    a = 0
		    b = 1

		    if n<=0:
			print('The fibonacci number is :',a)
		    elif n == 1:
			print('The fibonacci number is :',b)
		    else:
			for i in range(2,n):
			    c = a+b
			    a = b
			    b = c
			print(c)

		fib(n)
		
		
Q82. Write a Python program to interchange the first and last element in a list.

		list1 = [1,2,3,4,5,6,7,8,9,10]

		def interchange():

		    
		    print(list1)
		    tmp = list1[0]
		    list1[0] = list1[len(list1) - 1]
		    list1[len(list1) - 1] = tmp
		    print(list1)

		interchange()


Q83. Write a Python program to swap two elements in a list.

		list2 = [34,45,87,23,67,63]
		pos1 , pos2 = 1, 4

		def swapelements(list,pos1,pos2):
		    print(list2)
		    tmp = list2[pos1]
		    list[pos1] = list2[pos2]
		    list[pos2] = tmp
		    return list2

		print(swapelements(list2,pos1 - 1,pos2 - 1))
		
		
Q84. Write a Python program to find N largest element from a list.

		def Nmaxelements(list1, N):
		    final_list = []
		 
		    for i in range(0, N):
			max1 = 0
			 
			for j in range(len(list1)):    
			    if list1[j] > max1:
				max1 = list1[j];
				 
			list1.remove(max1);
			final_list.append(max1)
			 
		    print(final_list)
		 
		
		list1 = [2, 6, 3, 85, 0, 3, 7, 90, 10]
		N = 2
		 
		Nmaxelements(list1, N)


Q85. Write a Python program to find cumulative sum of a list.


		list=[10,20,30,40,50]
		new_list=[]
		j=0
		for i in range(0,len(list)):
		    j+=list[i]
		    new_list.append(j)
		     
		print(new_list)


Q86. Write a Python program to check if a string is palindrome or not.

		str1 = 'razar'

		def palindrome(s):
		    print(s)
		    print(s[ : :-1])
		    return s == s[ : : -1]

		out = palindrome(str1)

		if out:
		    print('Yes it is a palindrome')
		else:
		    print('No it is not a palindrome')


Q87. Write a Python program to remove i'th element from a string.

		def remove(strin, i):
		    a = strin[0 : i]

		    b = strin[i+1 : ]

		    return a + b

		c = 5

		string1 = 'MynameIsOmkar'

		output = remove(string1, c)

		print(output)


Q88. Write a Python program to check if a substring is present in a given string.

		str1 = str(input('Enter a string: '))
		substring = str(input('Enter the substring to check in string: '))

		if substring in str1:
		    print('Yes, the substring is present in the string')
		else:
		    print('No, the substring does not present in the string')
		    
		    
Q89. Write a Python program to find words which are greater than given length k.

		def find_words(string, k):
		    str1 = []
		    text = string.split()

		    for i in text:
			if len(i) > k:
			    str1.append(i)
		    return str1

		inputstring = str(input('Enter a string first: '))
		b = int(input('Enter the length to find the greater length words: '))

		output = find_words(inputstring, b)

		print('The words more than the length ',b,'are: ', output)
    
    
Q90. Write a Python program to extract unquire dictionary values.

		test_dict = {'gfg': [5, 6, 7, 8],
			     'is': [10, 11, 7, 5],
			     'best': [6, 12, 10, 8],
			     'for': [1, 2, 5]}

		print("The original dictionary is : ", test_dict)

		x=[]
		for i in test_dict.keys():
		    x.extend(test_dict[i])
		x=list(set(x))
		x.sort()
		print("The unique values list is : ", x)
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    






