# Python Two 
- Contains important information regarding the two-week period where Python was taught
## Week 2
- OOP (Object-Oriented Programming)
  - Four major pillars of OOP
    - Abstraction
        - Hiding unnecessary data, such as when importing modules or looking up the PC specs, it doesn't tell us how it's done, just the answer
    - Inheritance
        - Inherit data from another class, such as how a database extracts data from different databases 
    - Encapsulation
        - When you need to restrict access, such as a bank account. _age = 22 means the variable is private
    - Polymorphism
        - Once code has been inherited from another class, you can change, add new etc without effecting the parent class that the data code was taken from
  - keyword for implementing these modules is 'import'
  - Important for OOP code:
    - All classes after the parent class require:
      - from 'previous_file_name' import 'previous_class_name'
      - def __init__(self):
      - super().__init__()
    - Requires an object for the class to be called from
### Functions
- `def` is used to initialise the function
    - example: `def eat():`
- called via `eat()`
### Classes
- Allows for functions to be used on other files through:
  - `import` or `from file_name import class_name`
- File work
  - `try`, `except` and `finally` blocks of code
  - works similar to `if` and `else:` code
    ```python
    def greeting():  #| throws indention error, missing 'pass'
        name = 'DevSecOps'
        year = 2021
        print(name + year)  #| throws TypeError, cannot put a string and int together
        
        file = open('order.txt')  #| throws FileNotFoundError, file doesnt exist
        
        try:
            file = open('order.txt')
        except FileNotFoundError:
             print('File not found')
        try:
            file = open('order.txt')
        except FileNotFoundError as errmsg:
            # creating aliases
            print('File not found' + str(errmsg))  #|Displays a print with the error message

    ```
### API (Application Programming Interface)
  - An API, or Application Programming Interface, is a server that you can use to retrieve and send data to using code. APIs are most commonly used to retrieve data, and that will be the focus of this beginner tutorial. When we want to receive data from an API, we need to make a request.
    - API call is what UberEats uses (FOod on its way, food delivered etc)
### TDD (Test Driven Development)
  #### use pip to install the packages
  | Mode |Description|
  | :----: |:---- |
  |'r' |This is the default mode. It Opens file for reading. |
  |'w' |This Mode Opens file for writing. If file does not exist, it creates a new file. If file exists it truncates the file.|
  |'x' |Creates a new file. If file already exists, the operation fails.|
  |'a' |Open file in append mode. If file does not exist, it creates a new file.|
  |'t' |This is the default mode. It opens in text mode.|
  |'b' |This opens in binary mode.
  |'r+' |This will open a file for reading and writing (updating)|

    - TDD
    - Starts with RED (everything failing)
    - then GREEN to write the code to pass the test
    - BLUE is refactoring - then start again
    - `unittest` and `pytest`
        - at least two .py files, test.py and functional.py
        - test.py is for the test functions
        - functional.py is for the actual code
        - test functions must start with 'test'
        - assertEqual is a function from pytest(like .upper())
        - must set the object to the class from the functional.py file
        - the values in the test functions are (parameter1, parameter2, answer)
            - example: (10, 50), 60) = 10 + 50 = 60
        - can include hidden parameters
            - example for percentage: (10, 50), 20) = (10 / 50) * 100 = 20