# Lab 3 - Practice with Functions

### Due - Monday, September 23, 2024

Assignment Link: [https://classroom.github.com/a/ZR7QQ2C7](https://classroom.github.com/a/ZR7QQ2C7)

This lab assignment requires the following concepts:
- Functions
- Conditionals
- Logic operators

For this assignment, you will complete the following three programs:

## Camera Sales
Write a Python program that uses functions to solve the salesperson exercise here: [https://pymbook.readthedocs.io/en/latest/operatorsexpressions.html](https://pymbook.readthedocs.io/en/latest/operatorsexpressions.html). The exercise is described as follows:

In this example we are going to calculate the salary of a camera salesperson. Their basic salary is $1,500, for every camera they will sell they will get $200 and the commission on the month’s sale is 2%. The input will be number of cameras sold and total price of the cameras.

For full credit, your solution must have all of the following functions:

- A function `welcome` that takes no parameters and returns no values. The function will print a friendly welcome message to the user.
- A function `get_cameras_sold` that takes no parameters, prompts the user for the number of cameras sold, and returns the user's input as an integer.
- A function `get_camera_price` that takes no parameters, prompts the user for the price of each camera, and returns the user's input as a float.
- A function `calculate_total_pay` that takes two parameters: the number of cameras sold and the price per camera. The function will calculate the total pay as described above and return that value.
- A function `display_total` that will take as input the total and print it for the user in a nicely formatted message.
- A main function that will call the functions above appropriately.

## Lucky Sum
Write a Python program that implements a function 

`lucky_sum(a: int, b:int , c:int) -> int `

that takes as input three integers and returns their sum. However, if one of the values is 13 then it does not count towards the sum and values to its right do not count. So for example, if b is 13, then both b and c do not count.

Implement a main method that tests this function by calling it at least **five**
times with different test cases. For full credit, make sure your test cases test
different possible conditions.

This exercise is taken from the [coding bat](https://codingbat.com/python) website. 

## Rock, Paper, Scissors
Write a Python program that uses functions to play the game rock, paper, scissors. Play will proceed as follows:

- A random number will be selected to represent the computer choice. A 1 will be "rock"; a 2 will be "paper"; and a 3 will be "scissors".
- The user will be prompted to enter a choice of rock, paper, or scissors.
- If the user choice is valid the computer choice and user choice will be compared and a winner will be declared.
  * paper beats rock 
  * rock beats scissors
  * scissors beats paper
- If the user choice is not valid then play will end.

Hints:
- Grading will primarily depend upon how you decompose your program into
functions. Consider the steps listed above as you think about which functions to
implement. Also, consider going back to the preliminary design we discussed in class.
- You must validate the user input to confirm that it is either rock, paper, or
  scissors.

There are no required functions; however, much of your grade will depend upon the design that you choose for your program.

## Assignment Submission

To earn credit for this assignment you must commit all of your changes to your GitHub repository prior to the deadline. It is strongly recommended that you commit your changes regularly. Do not wait until you complete all parts of the assignment to upload your (partial) solution.

Step 1 - *Stage Changes*: Select the Source Control icon in the VSCode left menu. In the Changes section, click the + to *Stage All Changes*.

Step 2 - Commit Message: In the text box that says Message enter a meaningful message that describes the change you just completed.

Step 3 - *Commit & Push*: Select the down arrow in the blue box that says Commit. Choose *Commit & Push*.

Step 4 - Verify: Visit the repository on GitHub to confirm that your changes were uploaded successfully
