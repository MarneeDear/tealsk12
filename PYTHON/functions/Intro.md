# Intro to Functions

https://tealsk12.gitbook.io/intro-cs-2/unit_3/lesson

Functions let you define chunks of code that you can re-use in your code.

Functions should do one thing and one thing only. This is to help with understanding your code -- being able to reason about your program. 

> Pro tip: Keep functions simple and short.

Why would I keep a function simple and short?

* Easier to reason about
* Easier to keep track of what that function does
* Easier to maintain
* Easier to use
* Easier to test

>Pro tip: A way to help you write a simple function that only does one thing, remember that it is best if a function return the same `type` of data no matter what the logic of the function is.

For example, a function should return only integers, or a function should return only strings.


When you define a function you are defining a `contract` with the user of the function. The contract tells us how the function is should be used.

## Function syntax

With this syntax we can define our own functions:

```python
def my_function():
    # do something
    return 'something'
```

### Returning -- produce a value

Here I have defined a function called `my_function`. It returns `something`. You can return any kind of value or type from a function:

Functions can create new values and then return them back. We do this with the `return` keyword. 

```python
def my_function():
    # my code might do something to create a list
    my_list = ['a', 'b', 'c']
    return my_list
```

I can use that function like this:

```python
my_new_list = my_function() # returns a list
print(my_new_list) # what is my_new_list
```

What is the difference between returning and printing?

> print sends the value of the thing being printed to the output on the command line

> return creates a new thing or value that you can use later. You can print it or use it is some other way

## Side-effects

> Pro tip: A well defined function will not have any side-effects. A common side-effect to avoid is changing the value of a variable that was defined outside of the function.

### Avoid this

```python
def calculate_points(inventory):
    if 'prize' in inventory:
        game_state = 'you win'
        return 1000
    else
        game_state = 'keep playing'
        return 0

game_state = 'keep playing'

points = calculate_points([])

# what is the value of game_state? Did I need to change it in that function?
```

Does this make more sense?

```python
def calculate_points(inventory):
    if 'prize' in inventory:
        return 1000
    else
        return 0

game_state = 'keep playing'
inventory = ['rocks','napkin']

points = calculate_points(inventory)

if points > 99:
    game_state = 'you win'

```

Or maybe this?

```python
def calculate_points(inventory):
    if 'prize' in inventory:
        return 1000
    else
        return 0

def update_game_state(points):
    if points > 99:
        return 'you win'

game_state = 'keep playing'

inventory = ['rocks', 'napkin']

points = calculate_points(inventory)

game_state = update_game_state(points)

```

## Function parameters

Functions can also take parameters. Parameters are like variable that you can use in your function.

```python
def my_function_with_parameters(my_list, my_integer):
    my_list.append(my_integer)
    return my_list

my_new_list = my_function_with_parameters([1, 2, 3], 4)
print (my_new_list) # what will this be?

# you can use variables too
nums_list = [1, 2, 3]
num = 4
my_new_list = my_function_with_parameters(nums_list, num)
print(my_new_list) # what will this be?
```

Using a function is called called `calling` a function. In the above example I `called` the function my_function_with_parameters passing it two arguments `num_list` and `num`.

The `contract` of the function is that it take two parameters: a list and an integer, and the function adds that integer to the list and returns a new list.

The order of the parameters matters. You have to pass in your values to a function in the same order in which they appear in the parameters list.

You can also call a function using `named notation`. It looks like this:

```python
my_new_list = my_function_with_parameters(my_list=nums_list, my_integer=num)
```

See more here:
https://treyhunner.com/2018/04/keyword-arguments-in-python/

## Using built-in functions

Python has many built-in functions you can use in your code. We have seen a number of them.

```python

my_list = ['a', 'b', 'c']

len(my_list) # what does this do?

my_list.append('e') # what does this do?

type(1) # what does this  do?
type('hello world') # what does this do?

input('Please enter something:') # what does this do?

```

`len` is a function that `returns` a value -- the number of elements in the list

`append` is a function that can be used on lists.

`type` if a function that returns the type of the value

`input` is a function that sends a prompt to the command line and get the string entered at the command line

We can also import new functions.

A number of students have already tried using `random`. The built-in random functions let you create random numbers.

https://docs.python.org/2/library/random.html

We can use it like this:

```python
import random

random_int = random.randint(1,10)

```

`import` makes it possible to reference the `random` functions in your code. It is not automatically available. `random` is a Python `library` of code that does a lot of `random` things.

`randint` creates a random number between 1 and 10 including 1 and 10

`randint` takes two `arguments`. The starting number and the ending number

This is the range of numbers in which `randint` will create a new number

## Terms

`function` : defines a chunk of code, logic, you can re-use in your program

`parameters`: the variables you can use in your function

`call`: Calling a function means to use your function

`arguments`: the values or things you will pass to your function when you `call` the function.

`built-in`: Python functions like `len`, `append`, `random.randint`

`contract`: how a function is used. What parameters it takes, the types of those parameters, and what the function returns.

`side-effect`. A common side-effect to avoid is changing the state of a variable that is outside the function definition

## Resources

Teals Gitbook -- Intro to Functions
https://tealsk12.gitbook.io/intro-cs-2/unit_3/lesson

Parameterized Functions -- Python for Beginners
https://www.youtube.com/watch?v=sKW-zdYZNX4

Python Docs -- Random
https://docs.python.org/2/library/random.html

Python functions -- parameters and arguments
https://treyhunner.com/2018/04/keyword-arguments-in-python/