## Variable Declaration

Earlier we printed the ```"Hello, world!"``` string to the console. After it was printed we couldn't reuse that string, unless we retyped it all out from scratch, as shown below:
```python
print("Hello, world!")
print("Hello, world!")
```
But what if we wanted to use that string multiple times in our code? This is where __variables__ come in. With the following code, we can store the string in a variable and print it multiple times:
```python
message = "Hello, world!"
print(message)
print(message)
```
Output:
```
Hello, world!
Hello, world!
```
In the code above, we stored the string ```"Hello, world!"``` in a variable called ```message```. Then, instead of passing a raw string to the ```print()``` function, we passed the variable ```message```. This way, we can print the same string multiple times without having to retype it.

Variables are like containers that hold values.

## Challenge

```python

# don't modify the code below this line
print(message)
print(message)
```

Update the code so that it prints ```this string is stored in a variable``` to the console twice. You should be able to accomplish this by only adding one line of code.