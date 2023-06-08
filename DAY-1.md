# Day - 1
### Why learn Python

- **Design Philosophy:** It is very easy to understand, It is easy for human to read and understand
- **Batteries Included:** It has lot of inbuilt functions which will come in handy while developing any applications
- **General Purpose:** It supports different programming paradigms like procedural, OOPS, functional. We can build desktop apps, Web apps or even games
- **Libraries/Community:** It has a vast community support and lot of libraries are being developed everyday

---

### Why Python for Data Science?

- **Easy to Learn:** It is very easy to learn python even for a person who doesn't have any experience in programming
- **Proximity with Maths:** It has lot of libraries related to math computation which is very helpful in the data driven field
- **Community:** The community is vast and can get help from other's and libraries are being developed quickly.

---

### About Python

- It is case sensitive
- It has various inbuilt functions
- It has 32 Keywords

---

### Definitions

- **Function:** It's like a mathematical formula, We build the logic and with that we can pass any parameter to execute it
    - Built in function are like ready made tools that the language has, You use them where ever you want
- **Keywords:** Keywords are reserved words, they have specific purpose for it. They cannot be used as variable names
- **Variables:** A variable is a container where information can be stored.
- **Comments:** Line of code that doesn't get executed, It can be used to give instructions for other programmers.
    - You can use `#` to write a comment at any line
    - Always write comments for every program

---

### First Programm

- **Printing anything:** To print anything on the console we used an inbuilt function print()
- `print("This is my first programm")`
- This output is `This is my first programm`, Everything inside the function is enclosed in single or double quotes

---

### Data Types

- **Integer:** Represents positive or negative numbers, not decimals
- **Float:** Represents decimal numbers
- **Boolean:** Represents truth values True of False, used for logic building
- **String:** Represents a sequence of characters enclosed in single or double quotation marks
- **List:** Represents an ordered list enclosed in [] square brackets
    - lists are mutable, i.e elements can be added, removed or modified.
- **Tuple:** It is very similar to list enclosed in () round brackets
    - tuples are not mutable, i.e elements cannot be added or removed
- **Sets:** Represents an unordered list in {} curly brackets
    - It doesn't allow duplicate values
- **Dictionary:** Represents collection of key value pairs enclosed in curly braces `{key:value}` Ex. {name:"rohith"}

---

### Type function

- It is an inbuilt function that allows you to determine what type is the object or element `type()`
- Ex. type("Rohith") -> String, type(7) -> Integer

---

### Variables

- A variable is a container where information can be stored for the future use
- `name = "rohtih"`, When we `print(name)` It returns the value stores in the variable.
- We can create multiple variables at a time like this `a,b,c=1,2,3`

---

### Dynamic typing

- Python can automatically determine the datatype of the variable, no need to mention it explicitly. `num=5`

---

### Static typing

- Unlike python in java or C programming languages we need to mention the datatype before creating a new variable `int number = 5`

---

### Dynamic binding

- Python can change the datatype of any variable at any given time
- First we can store integer in a variable and later change it to string if needed.

---

### Identifiers

- Naming convention for variables
- They can consist upper case, lower case, digits and underscore
- The first letter must be a underscore or a letter
- It is case sensitive
- Don't use any keywords or reserved words
- It is always best to use lowercase separated by underscore `first_number` or use camelCase `firstNumber`

---

### Input

- It is an inbuilt function `input()` that allows to take input from the user
    - Ex. `input("Enter your name")`

---

Programing Task:

```python
#Take input from the user
firstNumber = int("Enter the first number");
secondNumber = int("Enter the second number");

#Add both the numbers taken from the user
sum = firstNumber + secondNumber

#Print the result
print("sum")
```

---

### Type conversion:

- It is the process of changing the datatype of a value from one type to another
- `int()`, `float()`, `str()`, `list()`, `dict()` these type functions are used to convert the data type

---

### Literals

- Python has inbuilt notations for representing values to the variables
- ****************************************Numerical Literals:**************************************** Integer, Float, Complex, Binary, Complex,
    
    ```python
    Integer = 10
    Float = 3.14
    Binary = 1010
    Complex = 2+3j
    ```
    
- **Sting Literals:** We can use single or double quotes
    
    ```python
    str_single = 'Hello'  
    str_double = "World"
    ```
    
- **Boolean Literals:** These represents truth values
    
    ```python
    is_true = True
    is_false = False
    ```
    
- **********************None Literals:********************** In Python to declare an empty variable we need to assign a None literal, We can assign different values later but to have an empty variable we need to use None literal.
    
    ```python
    k = None
    k = 3
    ```
    

---