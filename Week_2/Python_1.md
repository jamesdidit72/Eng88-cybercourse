# Python One 
- Contains important information regarding the two-week period where Python was taught
## Operators
| Operand | Description | Example |
|:---------: |:----------------------------: |:--------: |
| > | True if left operand is greater than the right| x > y |
| < | True if left operand is less than the right| x < y |
| == | True if both operands are equal | x == y |
| != | True if both operands are equal | x != y |
| >= | True if left operand is greater than or equal to the right| x >= y |
| <= | True if left operand is less than or equal to the right| x <= y |
## Collection types
- lists | syntax = [ ] | can be edited/ mutable | type = list
- dictionaries | syntax = {"keys":"values"} | type = dict
- tuples | syntax = ( ) | can't be edited once created/ immutable | type = tuple
- sets | syntax = { } | same as a list, but UNORDERED | type = set
## Indexes
- shopping_list = ['juice', 'strawberries', 'yogurt', 'chicken', 'raspberries', 'butter']  # a list contains 6 indexes
- 'juice' = index 0,'strawberries' = index 1,'yogurt' = index 2,'chicken' = index 3,'raspberries' = index 4,'butter' = index 5
- print(shopping_list[3])  # prints the 4th index of list
- print(shopping_list[-1])  # prints the 6th index of list because it is the end of the list
- print(shopping_list[3:6])  # prints the 4th, 5th and 6th index from the list
## Week 1
- dictionaries
  ```python
        contact_list = {
            "a": {
                "james": "76987256"
            },
            "b": {
                "kane": "3498597234"
            },
            "c": {
                "aidan": "29875405"
            }
        }
    
        print(contact_list["b"].keys())
        print(contact_list["b"]["kane"])

  ```
- control flow
    ```python
    user_age = 0
    
    if user_age <= 12:
        print("U, PG, and 12 films")
    elif user_age <= 15:
        print("U, PG, 12 and 15 films")
    else:
        print("you can see every film")
    
    time = 0
    
    if time > 5 and time < 12:
       print("good morning")
    elif time > 12 and time < 18:
        print("Good afternoon")
    else:
        print("Good evening")
    ```
- while loop | loops are used to ITERATE through data
    ```python
    game_active = True
    while game_active:
        game_random_number = random.randint(1, 10)
        user_guess = int(input("Enter a guess:  "))
        if user_guess == game_random_number:
            print(game_random_number, ".You guessed correctly")
            game_active = False
        else:
            print(game_random_number, ".Unlucky, try again")
    print("well done!")
    ```
- for loop | loops are used to ITERATE through data
    ```python
    # DICTIONARY
    student_1 = {
        'name': 'James',
        'key': 'value',
        'stream': 'Cyber Security',  # string
        'completed_lessons': 3,  # int
        'completed_lesson_names': ["variables", "operators", "data_collections"]  # list
    
    }
    for data in student_1:
        print(data)  # only prints the keys
    for data in student_1.values():
        print(data)  # only prints the values
    
    for data in student_1.values():
        if data == "Cyber Security":
            break
        print(data)
    ```