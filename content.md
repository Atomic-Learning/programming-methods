
In programming, a **method** is an attribute of an object that can be called like a function and may operate on the object itself. It's one of the core concepts in object-oriented programming and appears in almost every modern programming language.

# Methods Can Return Values or Modify Objects

Methods can behave in different ways:

- **Return a new value:** The method computes something and gives you the result, leaving the original object unchanged
- **Modify in place:** The method changes the object itself and doesn't return anything meaningful
- **Do both:** Some methods both modify an object and return a value

For example, a list is a collection of items. Methods might let you modify it directly (e.g. add an item, remove an item, sort the list) or retrieve information (e.g. find the number of items, check whether a value appears in it).

# Methods Versus Functions

Both methods and functions are pieces of code that can be called and passed arguments, and can execute code. However, while functions are standalone pieces of code, methods are functions that are defined within a class or object. This means they have access to the internal state of the object they belong to.

# Method Syntax

The general pattern for calling a method (noting that details may vary between languages) is:

```
object.method_name(argument1, argument2, ...)
```

Breaking this down:

- **object:** The thing the method belongs to
- **.** (dot): The accessor — tells the language to look inside the object
- **method_name:** The name of the method to call
- **(arguments):** Additional information the method needs (optional)

If a value is returned, you can capture it in a variable:

```
result = object.method_name(arguments)
```

# Why Methods Matter

Methods are important because they:

- **Organize code logically:** Related actions are grouped with their objects
- **Hide complexity:** You don't need to know how the method works, just how to use it
- **Enable code reuse:** Many objects of the same type share the same methods
- **Make code readable:** `person.get_age()` is clearer than `extract_age(person)`
