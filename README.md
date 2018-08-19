# MATLAB
MATLAB Tutorial

This tutorial is for beginners who wants to learn MATLAB. Let's begin with commands.

#### Course Contents

This course describes about the following topics.

1. Course Overview
  Familiarize yourself with the course.
  Course Overview
2. Commands
  Enter commands in MATLAB to perform calculations and create variables.
  Entering Commands
  Storing Data in Variables
  Using Built-in Functions and Constants
  Desktop Overview
3. Vectors and Matrices
  Create MATLAB variables that contain multiple elements.
  Manually Entering Arrays
  Creating Evenly-Spaced Vectors
  Array Creation Functions
4. Importing Data
  Bring data from external files into MATLAB.
  Saving and Loading Variables
  Import Tool
5. Indexing into and Modifying Arrays
  Use indexing to extract and modify rows, columns, and elements of MATLAB arrays.
  Indexing into Arrays
  Extracting Multiple Elements
  Changing Values in Arrays
6. Array Calculations
  Perform calculations on entire arrays at once.
  Performing Array Operations on Vectors
7. Calling Functions
  Call functions to obtain multiple outputs.
  Obtaining Multiple Outputs from Function Calls
8. Obtaining Help
  Use the MATLAB documentation to discover information about MATLAB features.
  Obtaining Help
9. Plotting Data
  Visualize variables using MATLAB's plotting functions.
  Plotting Vectors
  Annotating Plots
  Plots Tab
10. Review Problems
  Bring together concepts that you have learned with a project.
  Project - Electricity Usage
  Project - Audio Frequency
11. MATLAB Scripts
  Write and save your own MATLAB programs.
  The MATLAB Editor
12. Logical Arrays
  Use logical expressions to help you to extract elements of interest from MATLAB arrays.
  Logical Operations and Variables
  Combining Logical Conditions
  Logical Indexing
13. Programming
  Write programs that execute code based upon some condition.
  Decision Branching
  For Loops
14. Final Project
  Bring together concepts that you have learned with a project.
  Project - Stellar Motion
  Project - Stellar Motion (Script)



### What is MATLAB ..?
MATLAB (matrix laboratory) is a multi-paradigm numerical computing environment and proprietary programming language developed by MathWorks. ... Although MATLAB is intended primarily for numerical computing,

#### Download & Installation:

Download the latest MATLAB from [Download MATLAB](https://in.mathworks.com/downloads/web_downloads) and install it as per your operating system. To get free trail for limited days, please register with your email in MATLAB website.

##### Entering Commands
- You can execute commands by entering them in the command window after the MATLAB prompt (>>) and pressing the Enter key.
- Unless otherwise specified, MATLAB stores calculations in a variable named **ans**.
- The equals sign (=) in MATLAB is the assignment operator, meaning that the expression on the right of the equals sign is assigned to the variable on the left. So, when you enter x = 3+4, MATLAB first evaluates 3+4 and then assigns the result (7) to the variable x.
- Notice that the Workspace window (on the right) shows all the variables currently in the workspace.
- Adding a semicolon to the end of a command will suppress the output, though the command will still be executed, as you can see in the Workspace. When you enter a command without a semicolon at the end, MATLAB displays the result in the command window.
- You can recall previous commands by pressing the Up arrow key on your keyboard. Note that the Command Window must be the active window for this to work.
- When you enter just a variable name at the command prompt, MATLAB returns the current value of that variable.

##### Storing Data in Variables
- You can name your MATLAB variables anything you'd like as long as they start with a letter and contain only letters, numbers, and underscores **_**.

        3sq = 9
          ↑
        Error: Invalid expression. Check for missing multiplication operator, missing or unbalanced delimiters, or other      
        syntax error. To construct matrices, use brackets instead of parentheses.

        Did you mean: sq = 9 ?

- Try clearing all variables by entering the command **clear**
- **clear** command removes workspace variables, and **clc** clears the Command Window.

##### Using Built-in Functions and Constants
- Info: MATLAB contains built-in constants, such as pi to represent π.
      a = pi
      a =
      3.1416

Also, although only four decimal places are shown for π, it is represented internally with greater precision.
      x = pi/2
      1.5708

- MATLAB contains a wide variety of built-in functions, such as abs (absolute value) and eig (calculate eigenvalues).

      a = sin(-5)
      a =
      0.9589

      another example
      x = sin(10)

Note that MATLAB uses parentheses to pass inputs to functions, similar to standard mathematical notation.

- Now try using the **sqrt** function to calculate the square root of -9. Assign the result to a variable named z.

      z = sqrt(-9)
      z=
      0.0000 + 3.0000i

- Note that the solution contains the imaginary number, i, which is a built-in constant in MATLAB.

You can now move to the next section, or, if you are interested, explore a sampling of some of the other built-in functions in MATLAB (linked below).
      [Elementary math](http://www.mathworks.com/help/matlab/elementary-math.html)
      [Descriptive statistics](http://www.mathworks.com/help/matlab/descriptive-statistics.html)
      [Linear algebra](http://www.mathworks.com/help/matlab/linear-algebra.html)

##### Manually Entering Arrays

- All MATLAB variables are arrays, meaning that each variable can contain multiple elements. A single number, called a scalar, is actually a 1-by-1 array, meaning it contains 1 row and 1 column.

Create a variable named x with a value of 4.

      x=4
      x=
      4
- You can create arrays with multiple elements using square brackets.

      >> x = [3 5]
      x =
          3    5

Create an array named x with two elements in a single row: 7 and 9

      >> x = [7 9]
      x =
      7 9

- When you separate numbers by spaces (or commas), MATLAB combines the numbers into a row vector, which is an array with one row and multiple columns (1-by-n). When you separate them by semicolons, MATLAB creates a column vector (n-by-1)

      >> x = [1;3].

Now create an array named x with two elements, 7 and 9, in a single column. Try recalling the previous command and changing the space between the numbers to a semicolon (;).

      >> x [7;9]
      x =
       7
       9

- Now try creating a 1-by-3 row vector named x that contains the values 3, 10, and 5 in that order.

       >> x = [3 10 5]
        x =
        3  10  5

- Now try creating a 3-by-1 column vector named x that contains the values 8, 2, and -4 in that order.

        >> x = [8;2;-4]
        x =
          8
          2
          -4

- You can combine spaces and semicolons to create matrices, which are arrays with multiple rows and columns. When entering matrices, you must enter them row by row.

        >> x = [3 4 5;6 7 8]
        x =
            3    4    5
            6    7    8

Try creating a matrix named x with the values shown below.

            5    6    7
            8    9   10

          >>x = [5 6 7;8 9 10]
          x =
            5    6    7
            8    9   10

- In MATLAB, you can perform calculations within the square brackets.

        >> x = [abs(-4) 4^2]
        x =
             4    16

Try creating a 1-by-2 row vector named x that contains **sqrt(10)** as its first element and **pi^2 (π2)** as its second element.

        >> x = [sqrt(10) pi^2]
          x =
          3.1623 9.8696

-
