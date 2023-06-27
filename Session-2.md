# Session-2
### Operators

- Operators are symbols that perform operations on different variables
- There are different type of operators

---

### Arithmetic operators

```python
#Add
print(5+6) => 11

#Sub
print(5-6) => -1

#Multiply
print(5*6) => 30

#Divide
print(5/6) => 0.83

#Floor Division (Quotient)
print(5//6) => 0

#Modulus (Remainder)
print(5%6) => 5

#Exponential
print(5**6) => 15625
```

### Relational Operators

```python
#Greater than
print(5>7) => False

#Greater than or equal to
print(5>=7) => False

#Less than
print(5<7) => True

#Less than or equal to
print(5<=7)  => True

#Equal to
print(5==7) => False

#Not equal to
print(5=!7) => True
```

### Logical Operators

```python
#AND (if both inputs are equal to 1 then the output is equal to 1)
print(1 and 0) => False

#OR (if atleast 1 input is equal to 1 then the output is equal to 1)
print(1 or 0) => True

#NOT (if input is 1 it returns 0 and vice versa)
#Python assumes any non-zero number as True so when not gate is applied then returns false
print(not 1) => False 
```

### Bitwise Operators

```python
#Converts all the integers to binary first and then compute the operation

#bitwise and (If both bits are 1, the resulting bit is 1; otherwise, it is 0.)
print(5&6) => 4

#bitwise or (If at least one of the bits is 1, the resulting bit is 1; otherwise, it is 0)
print(5|3) => 7

#bitwise xor (If the bits are different, the resulting bit is 1; otherwise, it is 0.)
print(5^7) => 3 

#bitwise not (It converts 1 to 0 and 0 to 1.)
print(~5) => -6

#left shift (Shifts the bits of the left operand to the left by a specified number of positions)
print(4<<2) => 16

#right shift (Shifts the bits of the left operand to the right by a specified number of positions)
print(4<<2) => 1
```

### Assignment Operators

```python
#Assign (Assigns a value to a variable. The value on the right side of the operator is assigned to the variable on the left side.)
Example: x = 10

#Add and Assign (+=): (Adds the value on the right side to the existing value of the variable and stores the result back into the variable.)
Example: x += 5 is equivalent to x = x + 5

#Subtract and Assign (-=): (Subtracts the value on the right side from the existing value of the variable and stores the result back into the variable.)
Example: x -= 3 is equivalent to x = x - 3

#Multiply and Assign (*=): (Multiplies the value on the right side with the existing value of the variable and stores the result back) into the variable.
Example: x *= 2 is equivalent to x = x * 2

#Divide and Assign (/=): (Divides the existing value of the variable by the value on the right side and stores the result back into the variable.)
Example: x /= 4 is equivalent to x = x / 4

#Modulus and Assign (%=): (Performs the modulus operation on the existing value of the variable with the value on the right side and stores the remainder back into the variable.)
Example: x %= 3 is equivalent to x = x % 3

#Exponentiate and Assign (**=): (Raises the existing value of the variable to the power of the value on the right side and stores the result back into the variable.)
Example: x **= 2 is equivalent to x = x ** 2
```

### Membership Operators

```python
#in/not in (Checks if the required varibale is there in the datatype)

print('H' in 'Hyderabad') => True

print('R' not in 'Hyderabad') => False #Case sensitive
```

### Program

```python
#Find the sum of a 3 digit Numbner enter by the user 
#input = 615, Output = 12
#Use Operators only

#Take input from the user
userInput = int(input('Enter a three digit number')

#Using Modulus get the individual numbers from back
lastNumber = userInput%10
#Update the original input
userInput = userInput//10

middleNumber = userInput%10
userInput = userInput//10

firstNumber = userInput%10
userInput = userInput//10

#Sum of all the numbers
Sum = firstNumber + middleNumber + lastNumber

#Print the result
print(Sum)
```

---

### If-else

- Helpful in controlling the flow of the program
- It allows you to execute different blocks of code depending on whether a given condition is true or false.
- We can write an if-else statement inside an if-else statement, It is called Nested loop
- Use `elif` if you have multiple parameters to check

```python
#Syntax: (Check the indentation)

if condition:
	#Code to be executed
else:
	#Code to be executes
```

```python
# Write a program to check the login details of a user
#email: rohith@campusx.in
#password: r123

#take login details from the user
email = input('Enter the email')
password = input('Enter the password')

#Write a if-else statement to check the user
if (email=='rohith@campusx.in' and password == 'r123'):
	print('Welcome rohith')
else:
	print('Try Again')
```

```python
# Write a program to check the login details of a user and notify email or password is wrong
#email: rohith@campusx.in
#password: r123

#take login details from the user
email = input('Enter the email')
password = input('Enter the password')

# Using loops and Nested loops
#Check if both are correct
if (email == 'rohith@campusx.in' and password == 'r123'):
	print('Welcome rohith')

#Check if password is wrong and give another chance
elif(email=='rohith@campusx.in' and password != 'r123'):
	print('Wrong Password')
	password = input('Enter the password')
	if password == 'r123':
		print('Welcome rohith')
	else:
		print('Try Again')
else:
	print('Try Again')
```

```python
#Program
#Find the minimum number from the given numbers

#Take input from the user
firstNumber = int(input('Enter the first Number')
secondNumber = int(input('Enter the secong Number')
thirdNumber = int(input('Enter the third Number')

#Check the minimum number
if (firstNumber<secondNumber and firstNumber < thirdNumber):
	print('Minimum number is ', firstNumber)
elif (secondNumber < thirdNumber):
	print('Minimum number is ', secondNumber)
else:
	print('Minimum number is', thirdNumber)
```

---

### Modules

- Module is a file containing Python code that defines functions, classes, and variables that can be used in other Python programs.
- Syntax: `import moduleName` access the module using `moduleName.Example`
    - **Math Module:** It provides all the mathematical formulas and functions
    - **random Module:** It provides random values based on the request
    - **datetime Module:** It provides all the information related date and time, can perform operations on it

---

### Loops

- loops are used to repeatedly execute a block of code until a certain condition is met.
- **How are loops used real world example?**
    - Let's say you are developing a web application that displays a list of products available on an e-commerce platform, similar to Amazon. You have a database or a list of products that you want to display on the website.Using a loop, you can iterate over the list of products and generate HTML markup dynamically for each product. This allows you to display all the products without having to manually write HTML code for each one.

---

### While Loop

- The "while" loop is used to repeatedly execute a block of code as long as a certain condition is true.
    
    ```python
    while condition:
        # Code to be executed as long as the condition is true
    ```
    
    ```python
    #Write a program that takes a number and print's it table
    
    number = int(input('enter the number'))
    
    i = 1
    #print 10 numbers
    while i<11:
        print(number, '*', i , '=',number*i)
        i+=1
    ```
    
- To understand any code step by step use the [python tutor](https://pythontutor.com/python-debugger.html#mode=edit) website, Can be really handy when your stuck
- We can use while and else together, If the while condition breaks it enters into the else condition

---

### For loop

- We use range functin in for loop, It iterates throught the given range rang one by one.

```jsx
for item in range:
    # Code to be executed for each item
```