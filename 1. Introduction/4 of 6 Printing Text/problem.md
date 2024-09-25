## Printing Text
You may have noticed that we used double quotes ```""``` around the text. This is known as a string in programming. Most languages use double quotes to define a string.

Some languages like Python (and JavaScript) also allow you to use single quotes ```''``` to define a string.

A string is just a sequence of characters between the opening and closing quotes.

But what if we wanted to print a string that also contains quote characters? For example, how would the Python interpreter know where the following string ends?

```python
print("They said, "Hello, world!"")
```
This code will cause an error. Python thinks we have a string "They said, ", followed by Hello, world!, which is outside of the quotes (not apart of the string).

One possible solution to this is to use a backslash \, aka the escape character, before each quote character inside the string.
```python
print("They said, \"Hello, world!\"")
```
This tells Python we want to interpret the quote ```"``` as a character inside the string, not as a quote that ends the string.

## Challenge
Correct the starting code to print the following text to the console:
```
My favorite quote is "To be or not to be."
```
Starting code:
```python
print("My favorite quote is "To be or not to be."")
```
