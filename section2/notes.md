# Section #2

## 4. Introduction

## 5. The Python Type Hierarchy

Numbers

1. Integral: integers, booleans
2. Non-integral: floats, complex, decimals, fractions

Collections

1. Sequences
    1. Mutable
        1. lists
    2. Immutable
        1. tuples
2. Sets
    1. Mutable
        1. sets
    2. Immutable
        1. frozed sets
3. Mappings
    1. Dictionaries

Callables

_Anything that you can invoke... like a function._

- User-defined functions
- Classes
- Instance methods
- Class Instance
- Built-in functions
- Built-in methods

Singletons

- None
- NotImplemented
- Ellipsis

## 6. Multi-line Statements and Strings

Physical newline vs. logical newline

Allow us to write a single statement over multiple lines

All multiple line statements are terminated by a logical newline (token)

Implicit

- list []
- tuple ()
- dictionaries {}
- set {}
- function arguments / parameters

Explicit

Use the \ (backslash) character.

This won't work 👇

```python3
if a
    and b
    and c:
```

This will work 👇

```python3
if a \
    and b \
    and c:
```

**Comments can be used in when using backslashes to mark explicit multiple lines statements.**

Multi-line String Literals

```python3
"""This is 👈 _This line token will be retained._
a multi-line string"""
```

You can use `\n` or `\t`.

Not comments... but can be used as comment. What is different is that they stay with the code.

Comments are thrown out during the compiling process

## 7. Variable Names

identifier names

are case-sensitive

this is why we generally stick to always using lower case

must start with an underscore or a letter

must be made up of underscores, letters, or digits

Can't start with a digit

"Dunder" means double underscore

Cannot be reserved words

- None
- True
- False
- and
- or
- not
- if
- else
- elif
- for
- while
- break
- continue
- pass
- def
- lambda
- global
- ...

Conventions

`_my_var` - Begins with a single underscore - This is a internal or private object. These will not be imported with the "import"

`__my_var` - Begins with a double underscore - Used to "mangle" class attributes - useful for inheritance

`__my_var__` - Begins and ends with a double underscore - system defined names. special meaning to the interpreter

See "PEP 8 Style Guide" for more information about conventions

Packages: short, all lower case. no underscores

Modules: short, all lower case, can have underscores

Classes: Upper camel case

Functions: lower case, snake_case

Variables: lower case, snake_case

Constants: upper case, snake_case

## 8. Conditionals

`if`

Closest we have to a switch statement in Python is the `elif` statement

## 9. Functions

Functions are objects that we assign to a variable

Annotations

```python3
def func_1(a: int, b:int):
    return a * b
```

👆 These annotations are just like comments/documentations...

## 10. While

``` python3
i = 0
while i < 5:
    print(i)
    i += 1
```

"Do while"

``` python3
i = 5
while True:
    print(i)
    if i >=5:
        break # terminates the loop
```

`continue` allows you to continue the while loop, but breaks out of an iteration of it... Could be called, "break out of this iteration of the loop, but continue the loop"

`else` runs if the `while` never hit the `break` condition and finished the loop

## 11. Break, Continue and the Try statement

