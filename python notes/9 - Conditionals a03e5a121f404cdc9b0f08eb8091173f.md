# 9 - Conditionals

## Conditionals

By default, statements in Python script are executed sequentially from top to bottom. If the processing logic require so, the sequential flow of execution can be altered in two way:

- Conditional execution: a block of one or more statements will be executed if a certain expression is true
- Repetitive execution: a block of one or more statements will be repetitively executed as long as a certain expression is true. In this section, we will cover *if*, *else*, *elif* statements. The comparison and logical operators we learned in previous sections will be useful here.

### If Condition

In python and other programming languages the key word *if* is used to check if a condition is true and to execute the block code. Remember the indentation after the colon.

```python
# syntax
if condition:
    this part of code runs for truthy conditions
```

**Example: 1**

```python
a = 3
if a > 0:
    print('A is a positive number')
# A is a positive number
```

As you can see in the example above, 3 is greater than 0. The condition was true and the block code was executed. However, if the condition is false, we do not see the result. In order to see the result of the falsy condition, we should have another block, which is going to be *else*.

### If Else

If condition is true the first block will be executed, if not the else condition will run.

```python
# syntax
if condition:
    this part of code runs for truthy conditions
else:
     this part of code runs for false conditions
```

- *Example: **

```python
a = 3
if a < 0:
    print('A is a negative number')
else:
    print('A is a positive number')
```

The condition above proves false, therefore the else block was executed. How about if our condition is more than two? We could use _ elif_.

### If Elif Else

In our daily life, we make decisions on daily basis. We make decisions not by checking one or two conditions but multiple conditions. As similar to life, programming is also full of conditions. We use *elif* when we have multiple conditions.

```python
# syntax
if condition:
    code
elif condition:
    code
else:
    code
```

- *Example: **

```python
a = 0
if a > 0:
    print('A is a positive number')
elif a < 0:
    print('A is a negative number')
else:
    print('A is zero')
```

### Short Hand

```python
# syntax
code if condition else code
```

- *Example: **

```python
a = 3
print('A is positive') if a > 0 else print('A is negative') # first condition met, 'A is positive' will be printed
```

### Nested Conditions

Conditions can be nested

```python
# syntax
if condition:
    code
    if condition:
    code
```

- *Example: **

```python
a = 0
if a > 0:
    if a % 2 == 0:
        print('A is a positive and even integer')
    else:
        print('A is a positive number')
elif a == 0:
    print('A is zero')
else:
    print('A is a negative number')
```

We can avoid writing nested condition by using logical operator *and*.

### If Condition and Logical Operators

```python
# syntax
if condition and condition:
    code
```

- *Example: **

```python
a = 0
if a > 0 and a % 2 == 0:
        print('A is an even and positive integer')
elif a > 0 and a % 2 !=  0:
     print('A is a positive integer')
elif a == 0:
    print('A is zero')
else:
    print('A is negative')
```

### If and Or Logical Operators

```python
# syntax
if condition or condition:
    code
```

- *Example: **

```python
user = 'James'
access_level = 3
if user == 'admin' or access_level >= 4:
        print('Access granted!')
else:
    print('Access denied!')
```

## 💻 Exercises: Day 9

### Exercises: Level 1

1. Get user input using input(“Enter your age: ”). If user is 18 or older, give feedback: You are old enough to drive. If below 18 give feedback to wait for the missing amount of years. Output:
    
    ```python
    Enter your age: 30
    You are old enough to learn to drive.
    Output:
    Enter your age: 15
    You need 3 more years to learn to drive.
    ```
    
2. Compare the values of my_age and your_age using if … else. Who is older (me or you)? Use input(“Enter your age: ”) to get the age as input. You can use a nested condition to print 'year' for 1 year difference in age, 'years' for bigger differences, and a custom text if my_age = your_age. Output:
    
    ```python
    Enter your age: 30
    You are 5 years older than me.
    ```
    
3. Get two numbers from the user using input prompt. If a is greater than b return a is greater than b, if a is less b return a is smaller than b, else a is equal to b. Output:

```python
Enter number one: 4
Enter number two: 3
4 is greater than 3
```

```python
### Exercises: Level 2

```

1. Write a code which gives grade to students according to theirs scores:
    
    ```python
    80-100, A
    70-89, B
    60-69, C
    50-59, D
    0-49, F
    ```
    
2. Check if the season is Autumn, Winter, Spring or Summer. If the user input is: September, October or November, the season is Autumn. December, January or February, the season is Winter. March, April or May, the season is Spring June, July or August, the season is Summer
3. The following list contains some fruits:
    
    ```python
    fruits = ['banana', 'orange', 'mango', 'lemon']
    ```
    
    If a fruit doesn't exist in the list add the fruit to the list and print the modified list. If the fruit exists print('That fruit already exist in the list')
    
    ### Exercises: Level 3
    
4. Here we have a person dictionary. Feel free to modify it!

```python
        person={
    'first_name': 'Asabeneh',
    'last_name': 'Yetayeh',
    'age': 250,
    'country': 'Finland',
    'is_marred': True,
    'skills': ['JavaScript', 'React', 'Node', 'MongoDB', 'Python'],
    'address': {
        'street': 'Space street',
        'zipcode': '02210'
    }
    }
```

```
 * Check if the person dictionary has skills key, if so print out the middle skill in the skills list.
 * Check if the person dictionary has skills key, if so check if the person has 'Python' skill and print out the result.
 * If a person skills has only JavaScript and React, print('He is a front end developer'), if the person skills has Node, Python, MongoDB, print('He is a backend developer'), if the person skills has React, Node and MongoDB, Print('He is a fullstack developer'), else print('unknown title') - for more accurate results more conditions can be nested!
 * If the person is married and if he lives in Finland, print the information in the following format:

```

```python
    Asabeneh Yetayeh lives in Finland. He is married.
```