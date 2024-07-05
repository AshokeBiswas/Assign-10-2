Q1. Create a python program to sort the given list of tuples based on integer value using a lambda function. 
Here's a Python program that sorts a list of tuples based on the integer value using a lambda function:
python
Copy code
# List of tuples
tuple_list = [(1, 'b'), (3, 'a'), (2, 'c')]

# Sorting based on the first element of each tuple (integer value)
sorted_list = sorted(tuple_list, key=lambda x: x[0])

print(sorted_list)  # Output: [(1, 'b'), (2, 'c'), (3, 'a')]
In this example:
•	sorted() function is used with key=lambda x: x[0] to sort tuple_list based on the first element (integer value) of each tuple.
Q2. Write a Python Program to find the squares of all the numbers in the given list of integers using lambda and map functions. [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
Here's a Python program that uses lambda and map() function to find the squares of all numbers in the given list of integers:
python
Copy code
# List of integers
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Using lambda and map to find squares
squared_numbers = list(map(lambda x: x**2, numbers))

print(squared_numbers)
Output:
csharp
Copy code
[1, 4, 9, 16, 25, 36, 49, 64, 81, 100]
In this program:
•	lambda x: x**2 defines an anonymous function that squares each element x.
•	map(lambda x: x**2, numbers) applies this function to each element in numbers.
•	list() converts the map object into a list of squared numbers.
Q3. Write a python program to convert the given list of integers into a tuple of strings. Use map and
lambda functions
Given String: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
Expected output: ('1', '2', '3', '4', '5', '6', '7', '8', '9', '10')

Here's a Python program that converts a given list of integers into a tuple of strings using map() and lambda functions:
python
Copy code
# Given list of integers
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Using map and lambda to convert integers to strings
tuple_of_strings = tuple(map(lambda x: str(x), numbers))

print(tuple_of_strings)
Output:
arduino
Copy code
('1', '2', '3', '4', '5', '6', '7', '8', '9', '10')
In this program:
•	lambda x: str(x) defines an anonymous function that converts each integer x to its string representation.
•	map(lambda x: str(x), numbers) applies this function to each element in numbers.
•	tuple() converts the resulting map object into a tuple of strings.
Q4. Write a python program using reduce function to compute the product of a list containing numbers
from 1 to 25.

To compute the product of numbers from 1 to 25 using the reduce() function from the functools module in Python, you can do the following:
python
Copy code
from functools import reduce

# List containing numbers from 1 to 25
numbers = list(range(1, 26))

# Using reduce to compute the product
product = reduce(lambda x, y: x * y, numbers)

print("Product of numbers from 1 to 25:", product)
Output:
css
Copy code
Product of numbers from 1 to 25: 15511210043330985984000000
In this program:
•	reduce(lambda x, y: x * y, numbers) applies the lambda function lambda x, y: x * y cumulatively to the items of numbers, from left to right, so as to reduce the sequence to a single value which is the product of all elements in numbers.
Q5. Write a python program to filter the numbers in a given list that are divisible by 2 and 3 using the
filter function.
[2, 3, 6, 9, 27, 60, 90, 120, 55, 46]
can use the filter() function in Python to filter numbers in a given list that are divisible by both 2 and 3. Here's how you can do it:
python
Copy code
# Given list of numbers
numbers = [2, 3, 6, 9, 27, 60, 90, 120, 55, 46]

# Filter numbers divisible by 2 and 3
filtered_numbers = list(filter(lambda x: x % 2 == 0 and x % 3 == 0, numbers))

print(filtered_numbers)
Output:
csharp
Copy code
[6, 60, 90, 120]
In this program:
•	lambda x: x % 2 == 0 and x % 3 == 0 defines a lambda function that checks if a number x is divisible by both 2 and 3.
•	filter(lambda x: x % 2 == 0 and x % 3 == 0, numbers) applies this function to each element in numbers and returns a filter object containing only those elements that satisfy the condition.
•	list() converts the filter object to a list for easier inspection and printing.
Q6. Write a python program to find palindromes in the given list of strings using lambda and filter
function.
['python', 'php', 'aba', 'radar', 'level']

To find palindromes in a given list of strings using lambda and the filter() function in Python, you can do the following:
python
Copy code
# Given list of strings
strings = ['python', 'php', 'aba', 'radar', 'level']

# Filter palindromes
palindromes = list(filter(lambda x: x == x[::-1], strings))

print(palindromes)
Output:
css
Copy code
['aba', 'radar', 'level']
In this program:
•	lambda x: x == x[::-1] defines a lambda function that checks if a string x is equal to its reverse (x[::-1]), identifying palindromes.
•	filter(lambda x: x == x[::-1], strings) applies this function to each element in strings and returns a filter object containing only those elements that are palindromes.
•	list() converts the filter object to a list for easier inspection and printing.



