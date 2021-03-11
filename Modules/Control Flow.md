##### Boolean
True or False

### Relational Operators: Boolean expression is created using relational operators
Equals and not equals
Relational operators compare two items and return either True or False.

The two relational operators are:

Equals: ==

Not equals: !=


```python
3 * (2 - 1) == 4 - 1
```




    True




```python
13 - 6 != (3 * 2) + 1
```




    False




```python
(5 * 2) - 1 == 8 + 1
```




    True




```python
# Boolean variables: True and False are the only bool types, and any variable that is assigned one of these values is called a boolean variable.
set_to_true = True
set_to_false = False
# boolean expression.
bool_one = 5 != 7 
bool_two = 1 + 1 != 2
bool_three = 3 * 3 == 9
```


```python
print(bool_one)    # True
 
print(bool_two)    # False
 
print(bool_three)  # True
```

    True
    False
    True
    


```python
my_baby_bool = "true"
print(type(my_baby_bool))
my_baby_bool_two = True
print(type(my_baby_bool_two))
```

    <class 'str'>
    <class 'bool'>
    


```python
# If Statement (donot miss == or the conditional statement)
if 2 == 4 - 2: 
  print("apple")
```

    apple
    


```python
# Enter a user name here, make sure to make it a string
user_name = "angela_catlady_87"

if user_name == "Dave":
  print("Get off my computer Dave!")
if user_name == "angela_catlady_87":
  print("I know it is you, Dave! Go away!")

```

    I know it is you, Dave! Go away!
    

# Relational Operators II
- > greater than
- >= greater than or equal to
- < less than
- <= less than or equal to


```python
x = 20
y = 20

# Write the first if statement here:
if x == y:
  print("These numbers are the same")


credits = 120

# Write the second if statement here:
if credits >= 120:
  print("You have enough credits to graduate!")

```

    These numbers are the same
    You have enough credits to graduate!
    

# Boolean operators : AND

There are three boolean operators that we will cover:

and
or
not
Let’s start with and.

and combines two boolean expressions and evaluates as True if both its components are True, but False otherwise.


```python
S1 = (2 + 2 + 2 >= 6) and (-1 * -1 < 0)
S2 = (4 * 2 <= 8) and (7 - 1 == 6)
```


```python
S1
```




    False




```python
S2
```




    True



# Boolean operators : Or
The boolean operator or combines two expressions into a larger expression that is True if either component is True.


```python
S1 = (2 - 1 > 3) or (-5 * 2 == -10)
S1
```




    True




```python
S2 = (9 + 5 <= 15) or (7 != 4 + 3)
S2
```




    True




```python
statement_one = True

statement_two = True

credits = 118
gpa = 2.0

if credits >= 120 or gpa >= 2.0:
  print("You have met at least one of the requirements.")
```

    You have met at least one of the requirements.
    

# Boolean Operators: not
This operator is straightforward: when applied to any boolean expression it reverses the boolean value. So if we have a True statement and apply a not operator we get a False statement.

not True == False

not False == True


```python
S1 = not (4 + 5 <= 9)

S2 = not (8 * 2) != 20 - 4

S1   
```




    False




```python
S2
```




    True




```python
statement_one = False

statement_two = True

credits = 120
gpa = 1.8
if not credits >= 120:
  print("You do not have enough credits to graduate.")
if not gpa >= 2.0:
  print("Your GPA is not high enough to graduate.")
if not (credits >= 120) and not (gpa >= 2.0):
  print("You do not meet either requirement to graduate!")
```

    Your GPA is not high enough to graduate.
    

# Else Statements
- else statements allow us to elegantly describe what we want our code to do when certain conditions are not met.


```python
credits = 120
gpa = 1.9

if (credits >= 120) and (gpa >= 2.0):
  print("You meet the requirements to graduate!")
else:
  print("You do not meet the requirements to graduate.")
```

    You do not meet the requirements to graduate.
    

# Else If Statements
An elif statement checks another condition after the previous if statements conditions aren’t met.


```python
grade = 86
if grade >= 90:
  print("A")
elif grade >= 80:
  print("B")
elif grade >= 70:
  print("C")
elif grade >= 60:
  print("D")
else:
  print("F")
```

    B
    

# Points
- Boolean expressions are statements that can be either True or False
- A boolean variable is a variable that is set to either True or False.
- We can create boolean expressions using relational operators:

==: Equals
!=: Not equals
>: Greater than
>=: Greater than or equal to
<: Less than
<=: Less than or equal to

- *if* statements can be used to create control flow in your code.
- *else* statements can be used to execute code when the conditions of an if statement are not met.
- *elif* statements can be used to build additional checks into your if statements


```python
print("I have information for the following planets:\n")

print("   1. Venus   2. Mars    3. Jupiter")
print("   4. Saturn  5. Uranus  6. Neptune\n")
 
weight = 185
planet = 3

# Write an if statement below:

if planet == 1:
  weight = weight * 0.91
elif planet == 2:
  weight = weight * 0.38
elif planet == 3:
  weight = weight * 2.34
elif planet == 4:
  weight = weight * 1.06
elif planet == 5:
  weight = weight * 0.92
elif planet == 6:
  weight = weight * 1.19
 
print("Your weight:", weight)
```

    I have information for the following planets:
    
       1. Venus   2. Mars    3. Jupiter
       4. Saturn  5. Uranus  6. Neptune
    
    Your weight: 432.9
    

# C2: 1. Large Power
For the first code challenge, we are going to create a method that tests whether the result of taking the power of one number to another number provides an answer which is greater than 5000. We will use a conditional statement to return True if the result is greater than 5000 or return False if it is not. In order to accomplish this, we will need the following steps:

Define the function to accept two input parameters called base and exponent

Calculate the result of base to the power of exponent

Use an if statement to test if the result is greater than 5000. If it is then return True. Otherwise, return False


```python
def large_power(base, exponent):
    result = base ** exponent
    return result

print(large_power(2, 13))
```

    8192
    


```python
def large_power(base, exponent):
  if base ** exponent > 5000:
    return True
  else:
    return False
```


```python
large_power(2, 13)
```




    True




```python
large_power(2, 12)
```




    False



# 2. Over Budget
Let’s say we are trying to save some money and we are watching our budget. We need to make sure that the result of our spending is less than the total amount we have allocated for each of the categories. Our function will accept a parameter called budget which describes our spending limit. The next four parameters describe what we are spending our money on. We need to sum all of our spendings and compare it to the budget. If we have gone over budget, we will return True. Otherwise we return False. Here are the steps we need:

Define the function to accept five parameters starting with budget then food_bill, electricity_bill, internet_bill, and rent

Calculate the sum of the last four parameters
Use if and else statements to test if the budget is less than the sum of the calculated sum from the previous step.

If the condition is true, return True otherwise return False


```python
def over_budget(budget, food_bill, electricity_bill, internet_bill, rent):
    Sum = food_bill + electricity_bill + internet_bill + rent
    if budget < Sum:
        return True
    else:
        return False
# if u write true there will be name error...make sure to write True
```


```python
over_budget(80, 20, 30, 10, 30)
```




    True




```python
over_budget(100, 20, 30, 10, 40)
```




    False



# 3. Twice As Large
In this challenge, we will determine if one number is twice as large as another number. To do this, we will compare the first number with two times the second number. Here are the steps:

Define our function with two inputs num1 and num2

Multiply the second input by 2

Use an if statement to compare the result of the last calculation with the first input

If num1 is greater then return True otherwise return False


```python
def twice_as_large(num1, num2):
    double = num2 * 2
    if num1> double:
        return True
    else:
        return False
```


```python
twice_as_large(10, 5)
```




    False




```python
twice_as_large(11, 5)
```




    True



# 4. Divisible By Ten
To make things a bit more challenging, we are going to create a function that determines whether or not a number is divisible by ten. A number is divisible by ten if the remainder of the number divided by 10 is 0. Using this, we can complete this function in a few steps:

Define the function header to accept one input num

Calculate the remainder of the input divided by 10 (use modulus)

Use an if statement to check if the remainder was 0. If the remainder was 0, return True, otherwise, return False


```python
def divisible_by_ten(num):
    rem = num % 10
    if rem == 0:
        return True
    else:
        return False
```


```python
divisible_by_ten(20)
```




    True




```python
divisible_by_ten(25)
```




    False




```python
def divisible_by_ten(num):
  if (num % 10 == 0):
    return True
  else:
    return False
```

# 5. Not Sum To Ten
Finally, we are going to check if the summation of two inputs does not equal ten. Our function will accept two inputs and add them together. If the two numbers added together are not equal to ten, then we will return True, otherwise, we will return False. Here is what we need to do:

Define the function to accept two parameters, num1 and num2
Add the two parameters together
Test if the result is not equal to 10
If the sum is not equal, return True, otherwise, return False


```python
def not_sum_to_ten(num1, num2):
    if (num1+num2) != 10:
        return True
    else:
        return False  
```


```python
not_sum_to_ten(9, 1)
```




    False




```python
not_sum_to_ten(9, -1)
```




    True



# 1. In Range
Let’s start the advanced challenge problems by testing if a number falls within a certain range. We will accept three parameters where the first parameter is the number we are testing, the second parameter is the lower bound and the third parameter is the upper bound of our range. These are the steps required:

Define the function to accept three numbers as parameters
Test if the number is greater than or equal to the lower bound and less than or equal to the upper bound
If this is true, return True, otherwise, return False


```python
def in_range(num, lower, upper):
    if num >= lower and num <= upper:
        return True
    else:
        return False
```


```python
in_range(10, 10, 10)
```




    True




```python
in_range(5, 10, 20)
```




    False



# 2. Same Name
We need to write a program that checks different names and determines if they are equal. We need to accept two strings and compare them. Here are the steps:

Define the function to accept two strings, your_name and my_name
Test if the two strings are equal
Return True if they are equal, otherwise return False


```python
def same_name(your_name, my_name):
    if your_name == my_name:
        return True
    return False
```


```python
same_name("Tina", "Amber")
```




    False




```python
same_name("Colby", "Colby")
```




    True



# 3. Always False
There are some situations that you normally want to avoid when programming using conditional statements. One example is a contradiction. This occurs when your condition will always be false no matter what value you pass into it. Let’s create an example of a function that contains a contradiction. It will contain a few steps:

Define the function to accept a single parameter called num

Use a combination of <, > and and to create a contradiction in an if statement.

If the condition is true, return True, otherwise return False. 

The trick here is that because we’ve written a contradiction, the condition should never be true, so we should expect to always return False.


```python
def always_false(num):
    if num > 1 and num < 0:
        return True
    return False
```


```python
always_false(-1)
```




    False




```python
always_false(0)
```




    False




```python
always_false(1)
```




    False



# 4. Movie Review
We want to create a function that will help us rate movies. Our function will split the ratings into different ranges and tell the user how the movie was based on the movie’s rating. Here are the steps needed:

Define our function to accept a single number called rating

If the rating is equal to or less than 5, return "Avoid at all costs!"

If the rating was less than 9, return "This one was fun."

If neither of the if statement conditions were met, return "Outstanding!"


```python
def movie_review(rating):
    if(rating <= 5):
        return "Avoid at all costs!"
    if(rating < 9):
        return "This one was fun."
    return "Outstanding!"
```


```python
movie_review(9)
```




    'Outstanding!'




```python
movie_review(4)
```




    'Avoid at all costs!'




```python
movie_review(6)
```




    'This one was fun.'



# 5. Max Number
For the final challenge, we are going to select which number from three input values is the greatest using conditional statements. To do this, we need to check the different combinations of values to see which number is greater than the other two. Here is what we need to do:

Define a function that has three input parameters, num1, num2, and num3
Test if num1 is greater than the other two numbers
If so, return num1
Test if num2 is greater than the other two numbers
If so, return num2
Test if num3 is greater than the other two numbers
If so, return num3
If there was a tie between the two largest numbers, then return "It's a tie!"


```python
def max_num(num1, num2, num3):
    if num1> num2 and num1>num3:
        return num1
    elif num2> num1 and num2>num3:
        return num2
    elif num3>num2 and num3> num1:
        return num3
    else:
        return "It's a tie!"
```


```python

max_num(2, 3, 3)
```




    "It's a tie!"




```python

max_num(-5, -10, -10)

```




    -5




```python
max_num(-10, 5, -30)

```




    5




```python
max_num(-10, 0, 10)

```




    10




```python

```
