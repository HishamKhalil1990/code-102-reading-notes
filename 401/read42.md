# Pythonisms
## Dunder Methods
### Dunder methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for example `__init__` or `__str__`. they let you emulate the behavior of built-in types.
### Python’s data model is powerful API that you can interface with by implementing one or more dunder methods. various dunder methods like:
- Initialization of new objects
    - `__init__` is to construct account objects from the Account class
- Object representation
    - `__str__` and `__repr__` are to provide a string representation of your object for the consumer of your class 
- Enable iteration
    - `__len__`, `__getitem__` and `__reversed__` are to iterate over our account object I need to add some transactions
- Operator overloading (comparison)
    - `__eq__` and `__lt__`  are to compare python objects
- Operator overloading (addition)
    - `__add__` is to add python objects together
- Method invocation
    -  `__call__` is to make an object callable like a regular function
- Context manager support (with statement)
    - `__enter__` and `__exit__` are a simple “protocol” (or interface) that your object needs to follow so it can be used with the `with` statement 
## Iterators
### Objects that support the __iter__ and __next__ dunder methods automatically work with for-in loops. Iterators are working together to support Python’s iterator protocol. The two dunder methods `__iter__` and `__next__`, are the key to making a Python object iterable. 
```
class Repeater:
def __init__(self, value):
    self.value = value

def __iter__(self):
    return RepeaterIterator(self)

class RepeaterIterator:
def __init__(self, source):
    self.source = source

def __next__(self):
    return self.source.value
```
### Python iterators normally can’t be “reset”—once they’re exhausted they’re supposed to raise StopIteration every time `next()` is called on them. To iterate anew you’ll need to request a fresh iterator object with the `iter()` function.
### There’s a small but important difference between Python 2 and 3 when it comes to implementing class-based iterators:
- In Python 3, the method that retrieves the next value from an iterator is called `__next__`.
- In Python 2, the same method is called next (no underscores).
## Generators
### Generators look like regular functions but instead of using the return statement, they use yield to pass data back to the caller as:
```
def repeater(value):
    while True:
        yield value
```
### They look like normal functions, but their behavior is quite different. For starters, calling a generator function doesn’t even run the function. It merely creates and returns a generator object. The code in the generator function only executes when `next()` is called on the generator object. The `yield` keyword in there somehow stops this generator function in mid-execution and then resumes it at a later point in time. When a `yield` is invoked, it also passes control back to the caller of the function but it only does so temporarily.