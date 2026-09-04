

    Write a comment
    Write a multiline comment """ """
    Do variable declaration
    Write Rules for varibale declaration - must start with a letter or the underscore, cannot start with a number can only contain alpha-numeric characters and underscores. Its case sensative. varibale name cannot be python keyword.
    multiple assignment of varibales --ignore
    check type of variable
    cast one varibale type to another int str float
    String and print by concatinating the values 9.String / List / Tuple / Set / Dictionary /

Functions Of String Name ="Aman" print(Name.capitalize()) print(Name.upper()) print(Name.lower()) print(Name.swapcase()) print(len(Name)) print(Name.replace('a','$')) # find the text or word and replaces it with the provided value print(Name.split()) # converts it into list. print(Name.find('n')) # when found it retunrs the value starting from 0 and if not then returns -1

Functions Of List sort(): Sorts the list in ascending order. append(): Adds a single element to a list. extend(): Adds multiple elements to a list,insert value within a list. min(list): It returns an item from the list with min value. max(list): It returns an item from the list with max value. type(list): It returns the class type of an object. list(seq): Converts a tuple into a list. len(list): It gives the total length of the list.

Functions Of Tuple index(): It takes one argument and returns the index of the first appearance of an item in a tuple sorted(): a sorted version of the tuple. count(): It takes one argument and returns the number of times an item appears in the tuple. min(): Returns item from the tuple with min value. max(): Returns item from the tuple with max value. sum(): returns the arithmetic sum of all the items in the tuple. any(): If even one item in the tuple has a Boolean value of True, it returns True. Otherwise, it returns False. all(): returns True only if all items have a Boolean value of True. Otherwise, it returns False. tuple(seq): Converts a list into tuple. len(): total length of the tuple.

Functions Of Dictionary clear(): Removes all the elements from the dictionary - copy(): Returns a copy of the dictionary - get(): Returns the value of the specified key - values(): Returns a list of all the values in the dictionary keys(): Returns a list containing the dictionary's keys - items(): Returns a list containing a tuple for each key value pair -

Skips for beginners

fromkeys(): Returns a dictionary with the specified keys and value for a list/tuple/string. You can also assign default values.

pop(): Removes the element with the specified key - popitem(): Removes the last inserted key-value pair setdefault(): Returns the value of the specified key. If the key does not exist: inserts the key, with the specified value update(): Updates the dictionary with the specified key-value pairs, or insert new ones.

Functions Of Set clear(): Removes all the elements from the set copy(): Returns a copy of the set add(): Adds an element to the set pop(): Removes any random element from the set remove(): Removes the specified element, raises error if not found discard(): Removes the specified item, does not raise any error if value is not found issubset(): Returns whether another set contains this set or not issuperset(): Returns whether this set contains another set or not isdisjoint(): Returns whether two sets have any element in common. If even single element common then False, if both have unique then true. union(): Return a set containing the union of sets update(): Update the set with another set, or any other iterable. It is like doing multiple add() calls in a single step. It’s often used for merging sets or adding multiple items efficiently. intersection(): Returns a set, that is the intersection of two or more sets intersection_update(): Removes the items in this set that are not present in other, specified set(s) difference(): Returns a set containing the difference between two or more sets difference_update(): Removes the items in this set that are also included in another, specified set symmetric_difference(): Returns a set with the symmetric differences of two sets symmetric_difference_update(): inserts the symmetric differences from this set and another

List - A collection which is ordered and changeable where duplicates are allowed. (items have a defined order,and that order will not change.If you add new items to a list, the new items will be placed at the end of the list)

Tuple - A collection which is ordered and unchangeable, duplicates are allowed.

Dictionary - A collection which is ordered, changeable, indexed. No duplicates allowed.

Set - A collection which is unordered and unindexed, duplicates are not allowed. Set items can appear in a different order every time you use them, and cannot be referred to by index or key. The values True and 1 are considered the same value in sets, and are treated as duplicates

Frozenset in Python is an immutable version of a set. Normal sets can be changed after creation, but a frozenset cannot be modified.

10. Write a function and write a definition of a function
11. create function with default value
12. Function that returns a value
13. what is parameter and arguments  -
A parameter is the variable listed inside the parentheses in the function definition.
An argument is the value that is sent to the function when it is called.

15. if else elif

num = 7
if num > 0:
    print("Positive")
elif num < 0:
    print("Negative")
else:
    print("Zero") 

16. For Lopp

Loop for list
---------------
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)
    

------------ Reversed loop: for i in reversed(range(5)):
    
Loop for string
----------------
word = "Python"
for char in word:
    print(char)
  
Loop using Range
--------------------
for i in range(5):
    print(i)  # 0,1,2,3,4
    
Loop through Dictionary
------------------------
d = {"a": 1, "b": 2}

for key in d:
    print(key, d[key])
    
# OR using items()
for key, value in d.items():
    print(key, value)
    
Looping over dictionary items, keys, values
--------------------------------------------   
d = {'a': 1, 'b': 2}
for k, v in d.items():
    print(k, v)

for k in d.keys():
    print(k)

for v in d.values():
    print(v)
    
Nested loop
------------
for i in range(1, 4):
    for j in range(1, 4):
        print(i, j)

    
While loop
-------------
i = 1
while i < 6:
  print(i)
  i += 1

17. OOPS
 class, object, init, polymorphism (inbuilt, with class, with inheritance),
 Inheritance (Single,multiple,multilevel,hierarchical,hybrid)


OOPS in Python

class - A class is a user-defined data type. It consists of data members and
        member functions, which can be accessed by creating an instance of that class.
   
object - An Object is an instance of a Class. 

When a class is defined, no memory is allocated but when it is instantiated (i.e. an object is created) memory is allocated.
   
Encapsulation - Wrapping of data and function into a single unit is called encapsulation.

Data Abstraction - Hiding the real implementation of an application from the user and emphasizing only on usage of it.

Inheritance - it is the capability of a class to inherit the properties from another class.

Polymorphism - A function with same name can be used with multiple class or object.

Class and Object example code:
----------------------------------------

class Employee:
    def __init__(self, lappa, salary):
        self.nike = lappa
        self.salary = salary
    def aman_check(self):
        print('function inside of aman class',self.nike)

emp = Employee("Aman", 50000)

emp.nike



Single Inheritance 

Parent
  |
Child

# Base class
class Parent:
    def func1(self):
        print("This function is in parent class.")

# Derived class
class Child(Parent):
    def func2(self):
        print("This function is in child class.")

# Driver code
obj = Child()
obj.func1()
obj.func2()


Multiple Inheritance

   A     B
    \   /
     \ /
      C

# Base class 1
class Mother:
    mothername = ""

    def mother(self):
        print(self.mothername)

# Base class 2
class Father:
    fathername = ""

    def father(self):
        print(self.fathername)

# Derived class
class Son(Mother, Father):
    def parents(self):
        print("Father :", self.fathername)
        print("Mother :", self.mothername)

# Driver code
s1 = Son()
s1.fathername = "RAM"
s1.mothername = "SITA"
s1.parents()


Multi level inheritance


A → B → C


# Base class
class Grandfather:
    def __init__(self, grandfathername):
        self.grandfathername = grandfathername

# Intermediate class
class Father(Grandfather):
    def __init__(self, fathername, grandfathername):
        self.fathername = fathername
        # Call the constructor of Grandfather
        Grandfather.__init__(self, grandfathername)

# Derived class
class Son(Father):
    def __init__(self, sonname, fathername, grandfathername):
        self.sonname = sonname
        # Call the constructor of Father
        Father.__init__(self, fathername, grandfathername)

    def print_name(self):
        print('Grandfather name :', self.grandfathername)
        print('Father name :', self.fathername)
        print('Son name :', self.sonname)

# Driver code
s1 = Son('Prince', 'Rampal', 'Lal mani')
print(s1.grandfathername)
s1.print_name()



Hierarchical Inheritance

      A
    /   \
   B     C

# Base class
class Parent:
    def func1(self):
        print("This function is in parent class.")

# Derived class 1
class Child1(Parent):
    def func2(self):
        print("This function is in child 1.")

# Derived class 2
class Child2(Parent):
    def func3(self):
        print("This function is in child 2.")

# Driver code
object1 = Child1()
object2 = Child2()

object1.func1()
object1.func2()
object2.func1()
object2.func3()


Hybrid Inheritance

# Base class
class School:
    def func1(self):
        print("This function is in school.")

# Derived class 1 (Single Inheritance)
class Student1(School):
    def func2(self):
        print("This function is in student 1.")

# Derived class 2 (Another Single Inheritance)
class Student2(School):
    def func3(self):
        print("This function is in student 2.")

# Derived class 3 (Multiple Inheritance)
class Student3(Student1, School):
    def func4(self):
        print("This function is in student 3.")

# Driver code
obj = Student3()
obj.func1()
obj.func2()

skip polymorphism code all together
------------------------------------------------------------

1. Compile-time Polymorphism (Method Overloading)

class Calculator:
    def multiply(self, a=1, b=1, *args):
        result = a * b
        for num in args:
            result *= num
        return result

# Create object
calc = Calculator()

# Using default arguments
print(calc.multiply())            
print(calc.multiply(4))           

# Using multiple arguments
print(calc.multiply(2, 3))       
print(calc.multiply(2, 3, 4))

2. Runtime Polymorphism (Overriding)

class Animal:
    def sound(self):
        return "Some generic sound"

class Dog(Animal):
    def sound(self):
        return "Bark"

class Cat(Animal):
    def sound(self):
        return "Meow"

# Polymorphic behavior
animals = [Dog(), Cat(), Animal()]
for animal in animals:
    print(animal.sound())

-------------------------------------------------------------------------------------

super() is used to call methods (especially constructors) from a parent class
in a child class, without directly referring to the parent class name.

Calls parent constructor
Extending parent methods
Handling multiple inheritance safely

class Animal:
    def animal_speak(self):
        print("Animal speaks")

class Dog(Animal):
    def speak(self):
        super().animal_speak()
        print("Dog barks")

d = Dog()
d.speak()

Animal speaks
Dog barks


🧠 6. Multiple Inheritance (INTERVIEW CRITICAL)

class A:
    def show(self):
        print("A")

class B(A):
    def show(self):
        print("B")
        super().show()

class C(A):
    def show(self):
        print("C")
        super().show()

class D(B, C):
    def show(self):
        print("D")
        super().show()

d = D()
d.show()

OUTPUT

D
B
C
A

Always check MRO when multiple inheritance is involved:
    
print(ClassName.mro())

MRO(Method Resolution Order) flow - D → B → C → A → object

Step by Step Execution:
    
D.show()
Prints "D"
Calls super().show() → next in MRO → B.show()

B.show()
Prints "B"
Calls super().show() → next in MRO → C.show()

C.show()
Prints "C"
Calls super().show() → next in MRO → A.show()

A.show()
Prints "A"
Calls super().show() → next in MRO → object.show() (doesn’t exist, stops here)

18. try except else finally raise


19. Module - a file with set of predefined functions

Import datetime # get me the datetime module
from datetime import date # get me only the date function from the datetime module

20. Variable Scope in Python

Python Local variable: Local variables are those that are initialized within a function and 
                       are unique to that function. A local variable cannot be accessed outside of the function.
Python Global variables: Global variables are the ones that are defined and declared outside 
                         any function and are not specified to any function.

21. Identity Operators

is   Returns True if both variables are the same object x is y
is not Returns True if both variables are not the same object x is not y

22. Membership Operators

in   Returns True if a sequence with the specified value is present in the object x in y
not in Returns True if a sequence with the specified value is not present in the object x not in y

23. range() Function along with loops range(2, 30, 3) increments by x when defined else by 1 (here its 3)

24. *Args & **Kwargs

Arbitrary Arguments, *args

If you do not know how many arguments that will be passed into your function,
add a * before the parameter name in the function definition.
This way the function will receive a tuple of arguments

def add_numbers(*args):
    total = 0
    for num in args:
        total += num
    return total

print(add_numbers(1, 2, 3))       # Output: 6
print(add_numbers(5, 10, 15, 20)) # Output: 50

Arbitrary Keyword Arguments, **kwargs

If you do not know how many keyword arguments that will be passed into your function,
add two asterisk: ** before the parameter name in the function definition.
This way the function will receive a dictionary of arguments

def print_details(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

print_details(name="Alice", age=25, city="Kolkata")

25. Recursion
-----------------

A function calling itself repeatedly until a stopping condition is met.

def print_numbers(n):
    if n > 5:      # base condition
        return
    print(n)
    print_numbers(n + 1)   # recursive call

print_numbers(1)


def factorial(n):
    if n == 1:          # base case
        return 1
    return n * factorial(n - 1)
print(factorial(5))


factorial(5)
= 5 * factorial(4)
= 5 * 4 * factorial(3)
= 5 * 4 * 3 * factorial(2)
= 5 * 4 * 3 * 2 * factorial(1)
= 5 * 4 * 3 * 2 * 1
= 120

26. Scope

Funciton inside function
The variable x is not available outside the function, 
but it is available for any function inside the function. 
   

def check():
    name='Aman'
    def inside_check():
        surname='Ansari'
        print(name,surname)
    inside_check()
    
check()
    
    
    
27. User Input

username = input("Enter username:")
print("Username is: " + username)


28.Difference Between Modules and Packages in Python

Module -- not for beginer memorization

The module is a simple Python file that contains collections of functions and global variables and 
with having a .py extension file. It is an executable file and to organize all the modules we have 
the concept called Package in Python.

A module is a single file (or files) that are imported under one import and used. E.g.
import my_module


Package

The package is a simple directory having collections of modules. 
This directory contains Python modules and also having __init__.py file by which the 
interpreter interprets it as a Package. The package is simply a namespace. The package also contains sub-packages inside it.

A package is a collection of modules in directories that give a package hierarchy.
from my_package.abc import a

29. Data Type in python

 DataType
Mutable Or Immutable?
Boolean (bool)    Immutable
Integer (int)     Immutable
Float             Immutable
String (str)      Immutable
tuple             Immutable
frozenset         Immutable
list              Mutable
set               Mutable
dict              Mutable

30. Break, Continue, Pass

A break statement, when used inside the loop, will terminate the loop and exit. If used inside nested loops,
it will break out from the current loop.

A continue statement will stop the current execution when used inside a loop, and 
the control will go back to the start of the loop.

A pass statement is a null statement. When the Python interpreter comes across the pass statement, 
it does nothing and is ignored.

practice chat gpt program 


31. The ‘self’ parameter is a reference to the current instance of the class, and is used to access
variables that belongs to the class.



32. Difference Between Anonymous and Lambda Function

Lambda function:

It can have any number of arguments but only one expression.The expression is evaluated and returned.

Anonymous function:

In Python, Anonymous function is a function that is defined without a name/variable.
While normal functions are defined using the def keyword, Anonymous functions are defined using the lambda keyword.
Hence, anonymous functions are also called lambda functions.

Syntax:

lambda [arguments] : expression


Example:

square = lambda x : x * x
square(5) #25

The above lambda function definition is the same as the following function:
def square(x):
    return x * x

Lambda function and its definition - can take any number of arguments but can have 1 expression.
lambda arguments : expression
x = lambda  a,b,c: a+b+c
x(1,2,3)


Anonymous Function:  We can declare a lambda function and call it as an
    anonymous function, without assigning it to a variable.
print((lambda x: x*x)(5))

Above, lambda x: x*x defines an anonymous function and call it once
by passing arguments in the parenthesis (lambda x: x*x)(5).



33. Difference Between Shallow Copy and Deep Copy

A shallow copy creates a new object, but nested objects inside are shared 
between the original and the copy. Changes to nested objects affect both.

import copy
original = [1, 2, [3, 4]]
shallow = copy.copy(original)

shallow[0] = 100        # top-level change does NOT affect original
shallow[2][0] = 999     # nested change affects original

print(original)  # [1, 2, [999, 4]]
print(shallow)   # [100, 2, [999, 4]]


A deep copy creates a completely independent object, recursively copying
all nested objects. Changes in the copy do not affect the original.

import copy
original = [1, 2, [3, 4]]
deep = copy.deepcopy(original)

deep[2][0] = 999  # change in copy
print(original)    # [1, 2, [3, 4]]  -> original unaffected
print(deep)        # [1, 2, [999, 4]]

Use shallow copy for flat structures (lists without nested objects)
Use deep copy for nested structures (lists of lists, dicts, custom objects)

34.

# Map,Reduce,filter,slice,



  0   1   2   3   4   5  6   7   8   9  10  11 
------------------------------------------------
| H | E | L | L | O |  | P | Y | T | H | O | N |
------------------------------------------------
-12 -11  -10 -9  -8  -7 -6  -5  -4  -3  -2  -1 


str = 'HELLO PYTHON'
String Slicing

str1[0:5] (output = Hello, 0 to 4 index)- String slicing - Fetch all characters from 0 to 5

str1[6:12] (output = 'PYTHON',6 to 11 index last one is skipped)
# String slicing - Retreive all characters between 6 - 12 index

str1[-4:] # start from -4 until end


List Comprehension
----------------------------
mylist2 = [ i for i in range(40) if i % 2 == 1]

Expression for item in list( meaning for will execute and for each iteration it will check the if condition,
                             when found true it will returned to the first i expression )

Dictionary comprehension
----------------------------
square = {i:i**2 for i in range(10)}

Key value pair for var iteratable

MAP REDUCE FILTER LAMBDA
----------------------------
FILTER(function, iterable)
Multiple iterable not possible, workaround can be possible with zip function

list1 = [1,2,3,4,5,6,7,8,9]
# The below Filter function filters "list1" and passes all odd numbers using lamb
odd_num = list(filter(lambda n: n%2 ==1 ,list1))

MAP(function, iterable)

list1 = [1,2,3,4]
list2 = [5,6,7,8]
def double(x):
return x+x
def add(x,y):
return x+y
def square(x):
return x*x

print(list(map(double, list1)))
print(list(map(add, list1, list2)))

[2, 4, 6, 8]
[6, 8, 10, 12]

REDUCE(function, iterable)

list2 = [1,2,3,4]

product = reduce (operator.mul,list2) # Product of all numbers in a list
add = reduce(operator.add,list2) # Add all numbers in the list

print(product)
print(add)

24
10


Zip() is used to combine multiple iterables (like lists, tuples, etc.)
------------------------------------------------------------------------

names = ["Alice", "Bob", "Charlie"]
scores = [85, 90, 95]

result = zip(names, scores)
print(list(result))

[('Alice', 85), ('Bob', 90), ('Charlie', 95)]

----------------------------------------------------

a = [1, 2]
b = [3, 4]
c = [5, 6]

print(list(zip(a, b, c)))

[(1, 3, 5), (2, 4, 6)]

-----------------------------------------------------

keys = ["a", "b", "c"]
values = [1, 2, 3]

d = dict(zip(keys, values))
print(d)

{'a': 1, 'b': 2, 'c': 3}

# Have to look for list comprehension from subham wadekar pdf and manish kumar videos 

List comprehension 

nums = [1, 2, 3, 4]
squares = [x * x for x in nums]
print(squares)  # [1, 4, 9, 16]

With condition

nums = [1, 2, 3, 4, 5]
evens = [x for x in nums if x % 2 == 0]
print(evens)  # [2, 4]

With if else (Very important)

nums = [1, 2, 3, 4]
labels = ["Even" if x % 2 == 0 else "Odd" for x in nums]
print(labels)
# ['Odd', 'Even', 'Odd', 'Even']

Tricky interview favourite 

[x if x % 2 == 0 else -x for x in range(5)]
# [0, -1, 2, -3, 4]

With functions

def square(x):
    return x * x

result = [square(x) for x in range(5)]

With multiple conditions

nums = range(10)

result = [x for x in nums if x % 2 == 0 if x > 4]
print(result)  # [6, 8]


Dictionary comprehension (its basically same as list comprehension)
--------------------------------------


Different between in used in Dictionary and list

Dict use O(1) time complexity
List uses O(n) time complexity


Join method in python 
--------------------------------------

words = ["Hello", "World"]

result = " ".join(words)
print(result)
Hello World

Common interview traps

nums = [1, 2, 3]

",".join(nums)   # ❌ TypeError

Fix 

nums = [1, 2, 3]

result = ",".join(map(str, nums))
print(result)  # "1,2,3"

d = {"a": 1, "b": 2}

print(" ".join(d))          # joins keys → "a b"
print(" ".join(d.keys()))   # same

Advanced use of join

words = ["  hello", "world  "]
cleaned = " ".join(word.strip() for word in words)

Mixing types don't work with join(), it only works with strings 

["a", 1, "b"]  # ❌

35. What are Decorators?

Decorators are a powerful and flexible way to modify or extend the behavior of functions or methods,
without changing their actual code. A decorator is essentially a function that takes another function
as an argument and returns a new function with enhanced functionality.

Decorators are often used in scenarios such as logging, authentication and memorization, allowing us
to add additional functionality to existing functions or methods in a clean, reusable way.




36. What are Generators in Python?

In Python, the generator is a way that specifies how to implement iterators. It is a normal function
except that it yields expression in the function. It does not implement __itr__ and __next__ method 
and reduces other overheads as well.

If a function contains at least a yield statement, it becomes a generator. The yield keyword pauses
the current execution by saving its states and then resumes from the same when required.

def count_up_to(n):
    i = 1
    while i <= n:
        yield i
        i += 1
        
counter = count_up_to(3)

for num in counter:
    print(num)
    
Output 

1
2
3

Iteration begins

When the loop starts:

First iteration:
i = 1
yield 1 → returns 1
Function pauses
Second iteration:
resumes from where it stopped
i = 2
yield 2
Third iteration:
i = 3
yield 3
Next:
i = 4 → condition fails → function ends
🔹 Key Idea

does not store all values in memory
produces values on demand (lazy evaluation)

🔑 Summary
yield makes a function a generator
It returns values one by one
Keeps track of where it left off
More memory-efficient than lists



✅ Real-World Example: Reading a Large File

Imagine you have a very large file (like logs or data).
You don’t want to load the whole file into memory ❌

👉 Instead, you read it line by line using a generator ✅

“Generators are useful when working with large datasets, streams, or pipelines 
because they produce values on demand instead of storing everything in memory.”


✅ 3. Explicitly Closing a Generator

Python lets you force-stop it using .close():

gen = numbers()

print(next(gen))  # 1
gen.close()

👉 After close():

Generator is terminated
Further next() calls → error


37. What is a zip function?

The zip() function combines multiple iterables into a single iterator of tuples by pairing elements with the same index.

    Syntax:
    zip(*iterables) 

38. What are Pickling and Unpickling?

Pickling: The pickle module converts any Python object into a byte stream/ binary format (not a string representation). 
          This byte stream can then be stored in a file, sent over a network, or saved for later use. 
          The function used for pickling is pickle.dump().
    
Unpickling: The process of retrieving the original Python object from the byte stream
            (saved during pickling) is called unpickling. The function used for unpickling is pickle.load().
        

        
39. What is the difference between @classmethod, @staticmethod and instance methods in Python?

1. Instance Method operates on an instance of the class and has access to instance 
   attributes and takes self as the first parameter. Example:

     def method(self): 

2. Class Method directly operates on the class itself and not on instance, it takes
   cls as the first parameter and defined with @classmethod.

    Example: @classmethod def method(cls): 

3. Static Method does not operate on an instance or the class and takes no self or 
   cls as an argument and is defined with @staticmethod.

    Example: @staticmethod def method(): align it and dont bolod anything and not bullet points

Python coding practice Questions
-----------------------------------

1. Move zero to the end in array/list (Important)
2. Check if a string is subsequence of another string (important )
3. Frequency of word count (important interview question)
4. Find smallest and largest number in array/list
5. find pair sum for a give number in list [1,2,3,4,5], target_sum = 5, output (1,4)(2,3)
6. reverse a string input - 'blue is sky the' output - 'the sky is blue'
7. Prime number 
8. Fibonacci series
9. sort a list without using sort keyword (bubble sort will be used important )
10. sort a list using sort keywords
11. check for palindrome string 
12. Factorial
13. Common letter in 2 string (use set and interseaction function)
14. Convert two list in dictionary (use zip function)
15. Non negative integer not present in the array sequence
16. Factorial using recursion
17. Repeat Each character N times ('HELLO','HHHEEELLLLLLOOO')
18. FIND K MOST FREQUENT ELEMENT OF AN ARRAY
19. CHECK IF THE LIST IS SORTED OR NOT
20. Find the unique words from the give input string
21. Python program to find even numbers that come before odd numbers
22. Print elements in nested list in Python 
- https://www.youtube.com/watch?v=9K1rSQo-V_0&list=PLxy0DxWEupiOkz6d22HQk3-A9rC-paq3y&index=26
23. One List Sort with Numerical Value (important question good for manipulation)
- https://www.youtube.com/watch?v=zWaZNxIeuOM&list=PLxy0DxWEupiOkz6d22HQk3-A9rC-paq3y&index=27
24. Solve this questions using Dictionary in Python
- https://www.youtube.com/watch?v=gVkNJUvCiT8&list=PLxy0DxWEupiOkz6d22HQk3-A9rC-paq3y&index=28
25. Flatten a list and count occurrences in Python 
- https://www.youtube.com/watch?v=xWWd6coRj6A&list=PLxy0DxWEupiOkz6d22HQk3-A9rC-paq3y&index=29
26. Common letters in two strings in Python
- https://www.youtube.com/watch?v=oAGUya3297k&list=PLxy0DxWEupiOkz6d22HQk3-A9rC-paq3y&index=31
27. Count of each alphabets in strings in Python 
- https://www.youtube.com/watch?v=Ff0X1SPwXbU&list=PLxy0DxWEupiOkz6d22HQk3-A9rC-paq3y&index=32
28. Find Maximum Marks from List of Tuple in Python
- https://www.youtube.com/watch?v=bD2Y6ZEwD9k&list=PLxy0DxWEupiOkz6d22HQk3-A9rC-paq3y&index=33
29. Flatten the Nested List in Python
- https://www.youtube.com/watch?v=T6NU0cI4zHk&list=PLxy0DxWEupiOkz6d22HQk3-A9rC-paq3y&index=34
30. https://www.youtube.com/watch?v=-LElp8Xr3YU&list=PLxy0DxWEupiOkz6d22HQk3-A9rC-paq3y&index=35
31. Anagram string
32. Check if needed - https://www.youtube.com/watch?v=p2TZJiZWlAY&list=PLxy0DxWEupiOkz6d22HQk3-A9rC-paq3y&index=40
33. Find maximum value in a list. s = [3,5,1,1,2,2,4,5]
34. Write a script to identify repeated element from the list and no of time its getting repeated.
    Without using inbuilt functions.
list1 = [2,3,4,3,10,3,5,6,3,3,31, 10]
35. Implement a string compression algorithm.
Example: Input "AAABBBCCCDDDDAAA" → Output "A3B3C3D4A3"
36. Write Python code to sort a list of dictionaries by a key.



1. Find first non-repeating character
Input: "aabbcddde" Output: c
        
2. Remove duplicates but keep order
Input: "banana" Output: "ban"
        
3. Frequency of each character
Input: "malayalam" Output: {'m':2,'a':4,'l':2,'y':1}
        
4. Find max occurring character
Input: "success" Output: s
        
5. Merge two sorted lists (like merge step)
Input: [1,3,5], [2,4,6] — Output: [1,2,3,4,5,6]
        
6. Check balanced parentheses
Input: "( [ ] )" — Output: True
        
7. num = [15, 50, 5, 9, 20] find the 3rd largest number

8. Sorting a list of dictionaries in Python:
students = [
{"name": "Alice", "age": 20, "grade": "A"},
{"name": "Bob", "age": 22, "grade": "C"},
{"name": "Charlie", "age": 19, "grade": "B"},
{"name": "David", "age": 20, "grade": "A+"},
{"name": "Eve", "age": 21, "grade": "B-"},
]
# --- Sorting by 'age' (ascending order) –

9. Find Common Elements Between Two Lists
list1 = [1, 2, 3, 4]
list2 = [3, 4, 5, 6]

10. Sort Dictionary by Its Values --- very important question
data = {'apple': 3, 'banana': 1, 'orange': 2}

11. Merge Two Lists into a Dictionary

12. Find Missing Numbers from a Sequence
nums = [1, 2, 4, 6, 7, 9]
Output: [3, 5, 8]
    
13. Count Uppercase and Lowercase Letters
text = "HelloWorld"

15. Longest word in a sentence

16. Remove all duplicates characters
Input: "engineering" Output: "enginr"
        
17. Print unique elements from list

