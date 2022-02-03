# A small thing nobody taught you in Python


Have you ever noticed that some stuffs like `lower()`, `upper()`, `sort()` etc. are called like this `variable.lower()` or `variable.sort()`. But most of the other function are called like this `len(variable)`, `str(variable)`.\
What's the difference?

<!--more-->

Actually, the first set of examples are actually called **attributes** or **methods**.

Let's take the example of `lower()`, which acts on the `str` datatype.

`str` datatype is actually a class and has a number of functions inside it. These functions are called attribute and can be accessed by using the `.` notation.

```python
class Hello:
    def world(self):
        print("Hello World")

hello = Hello()        # Instantiate the class Hello
hello.world()          # Access the attribute world()

# Prints: Hello World
```

{{< admonition type=info title="Refresh your OOP" open=true >}}
If you are familiar with OOP programming, this is all very familiar to you. If not, you can read more [here](https://www.tutorialspoint.com/python/python_classes_objects.htm).
{{< /admonition >}}

So, back to our example:

```python
string = "Hello World"
print(string.lower())   # Here, I have called string's (str class)
                        # attribute lower() which changes case to
                        # lowercase

l = [1, 3, 2]
l.sort()                # Here, sort() is an attribute of l
                        # (list datatype) which sorts the list
```

{{< admonition type=tip open=true >}}
Thus, lower() and sort() are actually functions inside the str and list class respectively
{{< /admonition >}}

On the other hand, the latter examples were all **functions**, like your normal `def func()` thing. They perform a certain task on the argument that is passed to them. The task may or may not be unique to a particular datatype.

```python
string = "Hello World"
l = [1, 2, 3]

print(len(string))      # Prints the no. of characters in string
                        # (str datatype)
print(len(l))           # Notice, len() can be applied to list
                        # datatype (and various other types) too
```
I hope you leaned something new today :smile:.

