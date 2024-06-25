### 1. `object` - value(s) to be printed
You can pass one or multiple objects to the `print()` function, and it will print their values.
```python
# Single object
print("Hello, World!")

# Multiple objects
print("Hello", "World", 123)
```

### 2. `sep` (optional) - allows us to separate multiple objects inside print().
The `sep` parameter defines the separator between multiple objects. The default is a space.
```python
# Default separator (space)
print("Hello", "World", 123)

# Custom separator
print("Hello", "World", 123, sep="-")
```

### 3. `end` (optional) - allows us to add specific values like new line `\n`, tab `\t`
The `end` parameter defines what to print at the end of the `print` statement. The default is a newline character.
```python
# Default end (newline)
print("Hello, World!")

# Custom end (space)
print("Hello, World!", end=" ")
print("This is the next statement on the same line.")

# Custom end (tab)
print("Hello, World!", end="\t")
print("This is the next statement after a tab.")
```

### 4. `file` (optional) - where the values are printed. Its default value is `sys.stdout` (screen)
The `file` parameter defines the file-like object to which the print output is sent. By default, it is `sys.stdout` (the screen).
```python
# Import sys module to use sys.stdout
import sys

# Print to standard output (screen)
print("Hello, World!")

# Print to a file
with open("output.txt", "w") as f:
    print("Hello, World!", file=f)
```

### 5. `flush` (optional) - boolean specifying if the output is flushed or buffered. Default: False
The `flush` parameter controls whether the output is flushed immediately or buffered. By default, it is `False`.
```python
import time

# Without flush (default behavior)
print("Start without flush", end="")
time.sleep(2)
print(" - End without flush")

# With flush
print("Start with flush", end="", flush=True)
time.sleep(2)
print(" - End with flush")
```

These examples illustrate how to use each parameter of the `print()` function in Python to control how and where the output is printed.

```
# print("Loading", end="")
# for i in range(100):
#     print(".", end="", flush=True)
#     time.sleep(5 / 100)

#     input("Press Enter to continue...")

# num = int(input("Enter a number: ")) 

# print('The number you entered is ', num)
# print('datatype of num is', type(num))
```
