# **PYTHON**

- ### Python is a _CASE SENSITIVE_ language

* ## print(args)

  - ### helps in displaying whatever argument that is passed to it
  - ### eg.

    ```python

    print("Display some text here...")

    ```

* ## input(args)

  - ### helps in taking input from the user

  - ### eg.

    ```python
    variablee = input('Enter your name ? ')

    print('Hi '+ variablee)
    ```

  - ### By default returned value of input() is considered as a **string** by python interpreter so we've to specify the required data-type when needed using following functions

* ## type()

  - ### helps in checking the data-type of the argument passed

  - ### eg.

    ```python
    age = input("What's your age ? ")

    print('Type : ', type(age), 'Age : ' + age)
    ```

* ## int()

  - ### converts to int value

    ```python
    print('Type : ', type(int(age)), 'Age : ' + age)
    ```

* ## float()

  - ### converts to float value

    ```python
    height = input("What's your height ? (cm) ")

    print('Type : ', type(float(height)), 'Height : ' + height + 'cm')
    ```

* ## bool()

  - ### converts to bool value ( True / False )

* ## **Strings**

  - ### **Multiline string**

    - eg.

      ```python
      msg1 = '''

          Hi Sohan

          Just checking out this string format

          Thanks

      '''

      print(msg1)
      ```

  - ### **String Array Index**

    - As usual index of 1st character of the string is '0' and it goes on

    - To access the particular character of string following is the syntax

      ```python
      string_name[index]
      ```

  - ### eg.

    ```python
    msg2 = 'Ironman'
    print(msg2[0]) # prints the 1st character of the string msg2
    print(msg2[-1]) # prints the last character of the string msg2
    ```

    - Similarly '**-2**' prints the 2nd last character of the string msg2

  - ### **Getting a set of characters from a string**

    - eg.

      ```python
      print(msg2[0:3]) # prints 'Iro' from index '0' till index '3'
      print(msg2[:4]) # prints 'Iron'
      print(msg2[4:]) # prints 'man'
      print(msg2[:]) # prints 'Ironman'
      ```

  * ### **Formated Strings**

    - For long string outputs with loads of variables reading code can cause issue hence we use formatted strings

    - ### syntax:

      ```python
      f' text {variable} text {variables} text'
      ```

    - ### eg

      ```python
      msg3 = f"I'm {variablee} and I'm {age} old"
      print(msg3)
      ```

  * ### **len()**

    - returns length of the string passed as argument

    - **NOTE** : len() is a general purpose function and is not specific to strings

      ```python
      print('String Length : ', len(msg2))
      ```

  * ### **String class methods**

    - ### **string_name.upper()**

      - Returns an uppercase version of the provided string

        ```python
        print(msg2.upper())
        ```

    - ### **string_name.lower()**

      - Returns an lowercase version of the provided string

        ```python
        print(msg2.lower())
        ```

    - ### **find('character/string')**

      - Returns the index of the specified character/ starting index of the string

        ```python
        print(msg2.find('n'))
        ```

      - ### There's one more way to check if string or character exists in a paricular string or not

      - ### syntax :

        ```python
        'string/character' in string_name
        ```

      - ### this thing returns a boolean value unlike find() which returns index of the specified character/string

        ```python
        print('m' in msg2) # returns 'True'
        ```

    - ### replace('character/string destination', 'character/string source')
      - Replaces the 1st string with the 2nd string
        ```python
        print(msg2.replace('n', 'o'))
        ```

## **Arithemetic operators**

- > ### Addition +

- > ### Subtraction -

- > ### Multiplication \*

- > ### Division (/ & //)

  ```
  (there are actually two types of division to get int result and float result)

  # float / eg. 5 / 2 ---> 2.50

  # int // eg. 5 // 2 ---> 2
  ```

- > ### Exponent \*\*

  - eg.

  ```
  10 ** 3 ---> 1000
  ```

- Just like any other programming language, Python also follows BODMAS rule

## **Math Functions**

1. ### **round(args)**

   - returns the rounded off of the variable passed

   - eg.
     ```python
     x = 3.3
     print(round(x))
     ```

2. ### **abs(args)**

   - returns positve value

   - eg.
     ```python
     print(abs(-x))
     ```

## **Importing and using python modules**

- ### syntax :

  ```python
  import module_name
  ```

- ### **Accessing module methods**

  - ### syntax:
    ```python
    module_name.method()
    ```

- ### eg.

  ```python
  import math
  ```

  - ### ceil()

    - returns the ceiling of the argument passed
      ```python
      print(math.ceil(2.6))
      ```

  - ### floor()
    - returns the integer value of the argument passed
      ```python
      print(math.floor(4.69))
      ```

- ### Refer python 3 docs to learn more about modules

## **Conditional Operators**

- ## if statements

  - ### syntax :

    ```python

        if condition:

            statement

        elif condition:

            statement

        else:

            statement

        statement          # if needed
    ```

  - eg.

    ```python
      is_true = False

      is_false = True

      if is_true:

        print('Yes, This is True')

        print('Some more text here')

      elif is_false:

        print('Oops! This was False')

        print('What now?')

      else:

        print('Go get some life dude!')

        print('Noice (*-\_)')
    ```

  - ### **elif = else if**

## **Logical Operators**

- ### **_and_** Operator

  - eg.

    ```python
      is_greater = True

      is_from_india = True

      if is_greater and is_from_india:

        print('That sounds great!')
    ```

- ### **_or_** Operator

  - eg.

    ```python
    if is_true or is_false:

      print('I knew it...')

    is_greater = False
    ```

- ## **_not_** operator

  - eg.

    ```python
    if is_from_india and not is_greater:

      print('Result is Inversed')
    ```

## **Comparison Operators**

```python
 '<' '>' '<=' '>=' '==' '!='
```

## **Loops**

- ### **_while_** loop

  - syntax:

    ```python
    while condition:

      body

      update_condition

    #out of loop
    ```

  - eg.

    ```python
    i = 0

    while i < 5:

      print(i) #Inside loop

      i += 1

    print(i) #Outside loop
    ```

- ### **_for_** loop

  - syntax:

    ```python
    for i in array_name

      statement

      statement
    ```

  - eg.

    ```python
    for item in 'Sohan':

    print(item)
    ```

## **range()**

- ### creates a object

- eg

  ```python
  for item in range(10):

    print(item)

    for item in range(5, 10):

      print(item)

    for item in range(1, 10, 2):

      print(item)
  ```

## **Nested for loop**

- eg.

  ```python
    for x in range(4):
      for y in range(3):
        print(f'({x},{y})')

    numbers = [5, 2, 5, 2, 2]
    pattern = ''

    for i in numbers:
      for j in range(i):
        pattern += 'X'
        print(pattern)
      pattern = ''
  ```

## **List**

- ### Syntax :

  ```python
  list_name = ['item1', 'item2', 'item3', 'item4']
  ```

- ### Accessing specific items in a list

  - syntax :

    ```python
    list_name[n]

    #where n is the item no. or range of items just like strings
    ```

  - eg.

    ```python
    list_name[2:4]
    ```

  - eg.
    ```python
    list_name[2] = 'item10'
    ```

- ## **_2-D_** List

  - ### syntax :
    ```python
    list = [ [row], [row], [row] ]
    ```
  - ### eg.

    ```python
      matrix = [
      [1, 2, 3],
      [4, 5, 6],
      [7, 8, 9]
      ]

    for row in matrix:
      for element in row:
        print(element)
    ```

- ## **_List functions_**

  - ### Consider the following list
    ```python
    numbers = [1, 5, 3, 8, 6]
    ```
  - ### **.append(** _args_ **)**

    - Appends the passed args to the end of the list

    - eg.
      ```python
      numbers.append(0)
      print(numbers) # [1, 5, 3, 8, 6, 0]
      ```

  - ### **.insert(** _index,value_ **)**

    - Inserts element at specified index position
    - eg.
      ```python
      numbers.insert(0, 10)
      print(numbers) # [10, 1, 5, 3, 8, 6, 0]
      ```

  - ### **.remove(** _element_ **)**
    - Removes the specified element from the list
    - eg.
      ```python
          numbers.remove(1)
          print(numbers) # [10, 5, 3, 8, 6, 0]
      ```
  - ### **.clear()**

    - Removes all the elements of the list

  - ### **.index(** _element_ **)**

    - Returns the index of the first appearance of the specified element
    - eg.
      ```python
          print(f'Index : {numbers.index(5)}')
      ```

  - ### **.pop()**

    - Pops the last element
    - eg.
      ```python
          numbers.pop()
          print(numbers) # [10, 5, 3, 8, 6]
      ```

  - ### **.count(** _element_ **)**

    - Returns the count of how many times the specified element is repeated in the list

  - ### **.sort()**

    - Sorts the list elements in ascending orders

  - ### **.reverse()**

    - Reverses the order of the list

  - ### **.copy()**

    - creates a copy of that specific list

    - eg.
      ```python
      list2 = numbers.copy()
      print(list2) # [10, 5, 3, 8, 6]
      ```

# **Tuple**

- ## syntax:

  ```python
    tuple_name = ('item1', 'item2', 'item3')
  ```

- ### **NOTE :** Tuple is similar yet different from the 'list', it does not offer same functionalities as list like

  - ### we can only get info from tuple but we cannot change it once it is defined

  - ### accessing 'Tuple' is same as accessing 'List'

    - eg.
      ```python
      tuple_name = (1, 2, 5, 3, 8)
      print(tuple_name[3])
      ```

* ## Unpacking in Python

  - ### **NOTE :** Not limited to 'tuples' but can be used with things like 'list' also

  - ### Main point of using unpacking is to simplify accessing individual elements from list and tuple

    - ### eg. each element of 'tuple_name' can be easily assigned differnt value to access 'em faster just by doing following thing

      ```python
      a, b, c, d, e = tuple_name

      # here,
      # a = tuple_name[0]
      # b = tuple_name[1]
      # c = tuple_name[2]
      # d = tuple_name[3]
      # e = tuple_name[4]

      total = a + b + c + d + e
      print(f'Total : {total}')
      ```

# **Dictionary**

- ### Syntax :
  ```python
    dictionary_name = { 'key' : value , 'key' : value }
  ```
- ### eg.

  ```python
    customer = {
    'name': 'Sohan Vaigankar',
    'age': 20,
    'is_verified': True
    }
  ```

- ### **Adding new key or changing value to the existing key of an existing dictionary**

  - ### Syntax :

    ```python
    customer['birthday'] = '17 Aug 2000'
    ```

  - ### When accessing a key that doesn't exist, the interpreter flashes a Keyerror and to get rid of that error **_.get()_** is used
    ````python
      print(customer.get('address'), 'Khai Tari Ravta (Default Value)')
      ```
    ````

## **Functions**

- ### syntax :

  ```python
  def function_name():
    statement
  ```

- ### 'def' keyword is used to define a function

- ### **NOTE :** Leave 2 blank lines after every function definition

- ### Function should be defined prior to the function call

- ### eg.

  ```python

    # function definition

      def function_name():
      print('Hello')
      print('This is the function')

      # function call

        function_name()

      # Function Paramaters

      # eg.

        def para_function(first_name, last_name):
        print(f"Parameters passed = '{first_name} {last_name}'")

        para_function('Sohan', 'Vaigankar')
  ```

* ### **Keyword as Function Arguments**

  - ### With Keyword Arguments the order of the arguments passed to the function doesn't matter.

  - ### In short, the argument passed will be alloted to the specified parameter.

  - ### **Positional arguments** _(keyword arguments)_ should be passed first i.e. to the right end of the function parameters when both normal arguments and positional args are used

  - eg.
    ```python
      para_function(last_name='Vaigankar', first_name='Sohan')
    ```

* ### **Return Statements**

  - eg.

  ```python
        def square(number):
          return number**number

      print(f'Square : {square(5)}')

  ```

* ## **Exception Handling**

  - ### syntax:

    ```python
    try:

      # 'main code goes here'

    except Type_of_Error:

      # 'tell what to do if exception is encountered'

    ```

  - ### **NOTE :** **_Type_of_Error_** is actually predefined in the interpreter, you just need to specify it correctly

    - ### like ZeroDivisionError, ValueError, etc.

    - eg.

      ```python

      try:

        age = int(input('Age : '))

        print(age)

      except ValueError:

        print('Invalid Value type')

      ```

## **Class and object**

- ### Syntax for creating a class :

  ```python
  # defining class

  class ClassName:

    method_name(self):

      #method_stuff

    statement
  ```

- ### Syntax for creating object of class :
  ```python
      variable_to_store_object = ClassName()
  ```
- ## **Accessing members / member functions of the class**
  - ### Syntax :
    ```python
      variable_to_store_object.methode_name()
    ```

* ### eg.

  ```python
  class Point:
  def move(self):
  print('move')

      def draw(self):
          print('draw')

  point1 = Point()
  point2 = Point()
  point1.move()
  ```

* ### **NOTE :** 'self' is reference to the current object

* ## **Object Attributes**

  - ### These are basically variables which can be given to a particular object and are limited to only that particular object

  - ### eg.

    ```python
        point1.x = 10    # point1 object attribute 'x'
        print(point1.x)  # 10

        # print(point2.x) # if 'point2.x' is called then it flashes error saying that point2 object has no attribute 'x'

        # to access 'point2.x' we'll have to declare attribute 'x' for 'point2' object first

        point2.x = 20
        print(point2.x)
    ```

- ## **Constructor**

  - ### Constructor function syntax :
    ```python
    def __init__(self, attribute)
    ```
  - ### eg.

    ```python
      class ClassName:

        # Constructor definition
        def __init__(self, name):
          # assigning 'name' arg to 'fist_name' attribute of that particular object
          self.first_name = name

        # Accessing constructor values
        def display(self):
          # to access attributes syntax : 'self.attribute'
          print(f'Hi, I am {self.first_name}')

      obj1 = ClassName('Sohan')
      obj1.display()
    ```

## **Inheritance**

- ### Syntax :

  ```python
    class BaseClass:
      def method(self):
        # method definition

    class DerivedClass1(BaseClass):
      pass

    # The word 'pass' shall be used if you want to keep the derived class empty otherwise no need
  ```

- ### eg.

  ```python

        class Animals:
        def mammals(self):
        print('Mammal Gang!')

        class Dog(Animals):
        pass

        class Cat(Animals):
        def meow(self):
        print('Meow :)')

        dog_object = Dog()
        dog_object.mammals()

        cat_object = Cat()
        cat_object.meow()
        cat_object.mammals()

  ```

## **Modules**

- ### It's a set of functions and classes defined in a file which can be imported into any other file whenever aparticular function from module is required

- ### **NOTE :** module_name = filename (w/o extensions)

- ### Syntax to import modules :

  ```python
    import module_name

    # Accessing module functions (2 diff methods)

    # Method 1

    module_name.function_name()

    # Method 2

    # First type the following line right below 'import module' statement

    from module_name import function_name (w/o brackets)

    # Now, to access the function defined in that module just call the function normally without preattaching the module_name

    # syntax:

    function_name()
  ```

- ### eg.

  ```python
  import test_module1
  from test_module1 import *

  print(f'Square : {square(5)}')
  print(f'cubee : {test_module1.cube(5)}')

  numbers = [5, 12, 7, 3, 1, 9]
  print(f'Largest element : {find_max(numbers)}')
  ```

- ## Syntax to **create modules**:

  - ### Create a Python file ('.py') with desired module name

  - ### eg. 'test_module.py' and write function definitions inside that module

  - ### eg. following functions were defined in test_module.py

    ```python
      def square(number):
        return number**number

      def cube(number):
        return number*number*number

      def find_max(numbers):
        max_val = numbers[0]
        for element in numbers:
          if element > max_val:
          max_val = element
        return max_val
    ```

## **Packages**

- ### A project can contain hundreds of modules and to organise them they're put in a package

- ### Basically, Package is a container (directory / folder) with muliple modules
- ### **Creating a Package**

  - ### You can simply create a package by creating a folder and addding an empty '\_\_init\_\_.py' file to it

  - ### When interpreter sees the file '\_\_init\_\_.py' it automatically treats that folder as a package

  - ### Add modules to it and use it

- ### **Importing modules from packages**

  - ### **Mehtod 1**

    - ### syntax :

      ```python
      import package_name.module_name #On top of the page obviously -_-
      ```

    - ### **Accessing module functions :**

      - ### syntax :
        ```python
          package_name.module_name.function_name()
        ```

  - ### **Method 2**

    - ### Syntax (to import specific function(s) of a module):

      ```python
      from package_name.module_name import function_name

      #(function_name w/o brackets)
      ```

                                     OR

      ```python
      from package_name.module_name import function1_name, function2_name
      ```

    - ### **Accessing module functions**

      - ### syntax :

        ```python
        function_name()
        ```

    - ### Syntax (to **import** the **entire module** ):

      ```python
        from package_name import module_name
      ```

    - ### **NOTE :** in this case the module_name becomes an object hence it can be acessed using a ' . ' operator

    - ### **Accessing Syntax :**
      ```python
         module_name.function_name()
      ```
    - ### eg.

      - ### Assume that a folder 'test_package' is created and two files '\_\_init\_\_.py' & 'module1.py' are added and the file 'module1.py' contains following function definition

        ```python
            def some_function():
              print('Hello from the test_module!')
        ```

      - ### To call the above function from 'test_package' package we have to perform following steps

        ```python
            import test_package

            module1.some_function()
        ```

- ## **Built-in Python Modules**

  - ### Python has some cool built in modules, to know more about 'em search for 'python 3 module index on google'

  - ### **Using built-in modules**

    - ### syntax :
      ```python
          import module_name
      ```

  - ### **Accessing module function**

    - ### syntax :

      ```python
          module_name.function_name()
      ```

    - ### eg.

      ```python
          import random
          # Printing 3 random numbers b/w 10 and 20
          for i in range(3):
              print(random.randint(10, 20))
      ```

    - ### eg.

      ```python
          import random

          members = ['Ironman', 'Hulk', 'Captain America', 'Spider-man', 'Ant man']
          #Randomly chosing 1 member as the leader
          leader = random.choice(members)
          print(leader)
      ```
- ## **Additional Python Modules**

  - ### We can use more external python packages by going to [Python Package Index](https://pypi.org/) Website

  - ### **Downloading modules from Python Package Index using *pip***

    - ### syntax :
      ```bash
          $ pip install module_name
      ```
    - eg: 
      ```bash
          $ pip install openpyxl
      ```