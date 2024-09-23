# Lab 4 - Practice with Iteration

### Due - Monday, September 30, 2024

Assignment Link:
[https://classroom.github.com/a/WtOvuqgC](https://classroom.github.com/a/WtOvuqgC)

<hr/>

This lab assignment requires the following concepts:
- Loops
- Lists
- Strings and string operations 

For this assignment, you will complete the following three programs:

## Find Greater
Write a Python program that uses a function `find_greater(values: list[int],
target: int) -> int` to determine the number of values in a list of integers that
are greater than a value specified by the user. The function will take as a
parameter a list of integers and a single int provided by the user. It will
return the number of values in the list that exceed the user's target number.

Your main function will test your function implementation by calling
`find_greater` at least five times with arguments to exercise different test cases.

## Count ing Words
Write a Python program that implements a function `count_ing_words() -> int`. The function will use a while loop to read words from the user until the user enters 'quit'. Return the number of words the user entered that ended with the characters 'ing'. The last line of the output below will be printed by the main function.

Requirements and Hints:

- Your solution must be case *insensitive*. The function lower() can be used on a string to convert all of the characters to lower case.
- You will need to use another string function that we have not discussed in class. Refer to the String Methods portion of the Python documentation: https://docs.python.org/3/library/stdtypes.htmlLinks to an external site.

Sample output is as follows. Make sure to test thoroughly!

```
srollins@ada lab4 % python count_ing_words.py
Enter next word -- use 'quit' to end input: waiting
Enter next word -- use 'quit' to end input: enjoy
Enter next word -- use 'quit' to end input: happy
Enter next word -- use 'quit' to end input: working
Enter next word -- use 'quit' to end input: flyING
Enter next word -- use 'quit' to end input: quit
You entered 3 words ending with 'ing'.
```

Your main function will call the count_ing_words function and print the result.

## Passwordify
Write a Python program that uses a function `passwordify(original: str) -> str` to convert a phrase to a version of the phrase that you might use as a password. The function will take as a parameter the original phrase and will return the passwordified phrase as output. The rules for passwordification are as follows:

1. All instances of the character 's' or 'S' will be replaced with '$'
2. All instances of the character 'l' or 'L' will be replaced with 1.
3. All spaces will be replaced with '-'.
4. The word 'two' will be replaced by 2.
5. The word 'ten' will be replaced by 10.
6. The word 'three' will be replaced by 3.
7. The rules must be applied in the order they appear above. 

**For full credit, you may NOT use the `replace` method of String. You may find
it helpful to use the find method for requirements 4-6.**

Example:

```
input = ""sleeping in a tent"
output = "$1eeping-in-a-10t"
```

## Assignment Submission

To earn credit for this assignment you must commit all of your changes to your GitHub repository prior to the deadline. It is strongly recommended that you commit your changes regularly. Do not wait until you complete all parts of the assignment to upload your (partial) solution.

Step 1 - *Stage Changes*: Select the Source Control icon in the VSCode left menu. In the Changes section, click the + to *Stage All Changes*.

Step 2 - Commit Message: In the text box that says Message enter a meaningful message that describes the change you just completed.

Step 3 - *Commit & Push*: Select the down arrow in the blue box that says Commit. Choose *Commit & Push*.

Step 4 - Verify: Visit the repository on GitHub to confirm that your changes were uploaded successfully
