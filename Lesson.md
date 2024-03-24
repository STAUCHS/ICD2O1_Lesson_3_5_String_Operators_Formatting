# 3.5 Strings Operations & Formatting

## Success Criteria
- [ ] I understand and can use string concatenation effectively
- [ ] I understand and can use escape characters effectively
- [ ] I understand and can format strings effectively

## String Concatenation

So far, when we use our print statements, we have been separating each argument with a comma `,`. Another way we can print is to use `String Concatenation`. Concatenation is a fancy word for sticking strings together. In Python we use the addition operator to accomplish this:

### Examples
```EXAMPLE #1:```
```python
print("Hello" + "World")

# Output: ____
```

Notice how it doesn’t insert a space character automatically. You have to explicitly add a space character.

```EXAMPLE #2:```
```python
print("Hello " + "World")

# Output: ____
```

```EXAMPLE #3:```
If strings are stored in variables, you can treat the variables like strings and concatenate them.
```python
first_name = "Bob"
last_name = "Smith"

print(first_name + last_name)

# Output: ____
```

```EXAMPLE #4:```
How could you explicitly add a space character when using variables? Just add a space in the print statement using string concatenation.
```python
first_name = "Bob"
last_name = "Smith"

print(first_name + " " + last_name)

# Output: ____
```

```EXAMPLE #5:```
You can also use multiplication with strings and integers:
```python
first_name = "Bob"

print(first_name * 3)

# Output: ____
```

```EXAMPLE #6:```
What if you wanted to have an integer or float in a string?
```python
first_name = "Bob"
num = 3

print(first_name + num)

# Output: ___
```

We need to change the `int` to a `str`
```python
first_name = "Bob"
num = 3

print(first_name + str(num))

# Output: ___
```

### SUMMARY
| Expression       | Example           | Output    |
| ---------------- | ----------------- | --------- |
| string + string  | `"a" + "b"`       | `ab`      |
|                  | `"a" + "b" + "c"` | `abc`     | 
| string * integer | `"a" * 3`         | `aaa`     |
| integer * string | `3 * "a"`         | `aaa`     | 


## Escape Characters
An escape character is a backslash \ followed by a character you want to insert.

| Escape Character | What does it do?                                | Example                                    | Output                                 |
| ---------------- | ----------------------------------------------- | ------------------------------------------ | -------------------------------------- |
| `\'` or `\"`     | For when you want to use quotations in a string | `"\'This is a quote with single quotes\'"` | 'This is a quote with single quotes'   |
| `\n`             | To create a newline (acts as "Enter")           | `First line\nSecond line`                  | First Line                             |
|                  |                                                 |                                            | Second Line                            |
| `\t`             | To add a tab in your string                     | `Hello\tWorld`                             | Hello &nbsp; &nbsp; &nbsp; World       |

## f-Strings
```EXAMPLE #7:```
To use formatted string literals:
- Begin a string with `f` or `F` before the opening quotation mark. For example,
```python
print(f"Your string goes here")

# Output: Your string goes here
```

```EXAMPLE #8:```
- Inside this string, you can write a Python expression between { and } that can refer to variables or literal values. For example,
```python
var_1 = "Hello"
var_2 = "World"

print(f"Your string has {var_1} and {var_2}.")
# Output: Your string has Hello and World.
```