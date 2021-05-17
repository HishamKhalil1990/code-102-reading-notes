# List Comprehensions
### List comprehensions is a way to create list by evaluating an expression inside the list brackets. The expressions can be all kinds of objects in lists and the list comprehension always returns a result list
![ex](https://i.ibb.co/SKRpBX6/2.jpg)
### List Comprehensions consists of: 
- the `expression` that evaluate the list items' values and append it to the list
- `for` loop to repeat the condition 
- `if` condition to determine whether the expression is used or skipped
### the expression can be:
- expression for multiplying parts (`item*3`) of a list as `multiplied = [item*3 for item in list1]`
- expression for showing the first letter (`word[0]`) of each word as `items = [word[0] for word in listOfWords ]`
- a defined function (`double(x)`) as `double = [double(x) for x in range(10)]`
