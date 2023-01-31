# User Interaction

## Learning Goals

- Prompt user for input.
- Store user input in variables.
- Use the input value.

## Introduction

We have been providing our own values for all the programs we have written. But
most programs have some form of interaction to make them more useful or
interesting. Python offers a convenient way to accept and use input from users.

## Taking User Input

We can use the `input` function to prompt the user for input:

```python
name = input('What is your name? ')
print(name)
```

When you run this code, the console will prompt you to enter your name:

![Untitled](https://curriculum-content.s3.amazonaws.com/intro-to-coding-python/user-interaction/01.png)

Once you enter your name, it will be assigned to the `name` variable label. The
next line of code will display the value `Al` in the console.

![Untitled](https://curriculum-content.s3.amazonaws.com/intro-to-coding-python/user-interaction/02.png)

## Taking Numbers as Input

Here’s another example of taking and using user input:

```python
num1 = input('Enter the first number: ')
num2 = input('Enter the second number: ')
total = num1 + num2
print(total)
```

And here’s the output when we enter `5` for the first prompt and `3` for the
second prompt:

```python
53
```

What went wrong here? Think about the data type we are working with.

```python
num1 = input('Enter the first number: ')
num2 = input('Enter the second number: ')
print(type(num1)) # <class 'str'>
print(type(num2)) # <class 'str'>
total = num1 + num2
print(total) # 53
```

The `input` always gives us a string unless we explicitly convert the type.

Python provides an `int` function that allows us to convert other data types to
numbers. Here’s how to use the function:

```python
current_year_str = "2023"
current_year_int = int(current_year_str)
print(type(current_year_int))
```

We can fix our previous code by using the `int` function:

```python
num1 = int(input('Enter the first number: '))
num2 = int(input('Enter the second number: '))
print(type(num1)) # <class 'int'>
print(type(num2)) # <class 'int'>
total = num1 + num2
print(total) # 8
```

## Conclusion

Now that we can take input from users, we will be able to make more interesting
programs! Remember to always note what data type you’re working with on every
line or you will run into errors that are hard to understand and fix.
