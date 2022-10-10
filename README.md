# Python (Part 3)
# Function
- in Math, a function is a process that relates an input and an output
- in Python, in addition to those relational functions. Functions are also a way to organize code with the ultimate goal of reusability.
- It is recommended that functions have only one specific use but can be reused
- Common functions are available in Python
- But we can always define our own function
### Definition
- Functions are defined with the def keyword followed by the name of the function and its parameters in brackets ()
- Optionally, you can add docstring-string documentation describing the context of the function
- The code block in each function starts with a colon using an indentation
- The function stops when there is a return statement (expression) that returns (expression) to the caller
- You can also make the function return no output by returning None
### Return
- the return statement (expression) will make the program execution exit the current function, while returning a certain value
- The return value in a function can be stored in a variable
- This is what distinguishes a function that returns a value from a function that does not return a value (often called a procedure).
### Pass by Reference vs Value
- All the parameters in the python language are passed by reference. So, if we change what a parameter refers to within a function, the change also reflects back in the calling function.
### Function Arguments and Parameters
- Paremeter is the definition of input that a function accepts.
- Arguments are the things we enter when calling the function.

# Pydoc
- The pydoc module automatically generates documentation from Python modules. The documentation can be presented as pages of text on the console, served to a web browser, or saved to HTML files.
- To view python documentation using pydoc, we can open command prompt(Anaconda Prompt).

# Txt File
- A TXT file is a standard text document that contains plain text. It can be opened and edited in any text-editing or word-processing program

### Open
- The file you want to open must be in the same location as the python file used to run the command.
- If the file is located in a different location, you will have to specify the file path.
- To open the file, use the built-in open() function.

### Read
- **read()** method use to read the content of the file.
- By calling **readline()** two times, you can read the two first lines.
- If you want to display the third line, you must calling **readline()** for the first line then forthe second line fisrt.

### Close
-	It is a good practice to always close the file when you are done with it.
-	To close file you can use : _varibel_name.close_

### Write
- By adding the "w" parameter in the open() function then the file will open to write.
- If the file exists, the function will truncate all the contents as soon as you open it.
- If the file doesn’t exist, the function creates a new file.

### Check Existence
- we can check existence of txt file by using os module
- to check existence we must using os.path.isfile('filename.txt') query will return boolean value

### Remove
- We can remove txt file by using os module and call remove function
- to remove file we must using os.remove('filename.txt') query will remove file in the directory

# Module In Python
- A Python module is a file containing Python definitions and statements. A module can define functions, classes, and variables. A module can also include runnable code. Grouping related code into a module makes the code easier to understand and use. It also makes the code logically organized.
## Math
- math module is python module that can handle these complex calculations. Both simple mathematical calculations like addition (+), and subtraction (-), and advanced mathematical calculations like trigonometric operations, and logarithmic
## IO
- Python io module allows us to manage the file-related input and output operations. The advantage of using the IO module is that the classes and functions available allows us to extend the functionality to enable writing to the Unicode data.
## Datetime
- Python Datetime module supplies classes to work with date and time. These classes provide a number of functions to deal with dates, times and time intervals.There are 6 main classes in Datetime module :
•	date <br />
•	time <br />
•	datetime <br />
•	timedelta <br />
•	tzinfo <br />
•	Timezone <br />
## Sys
- Sys module in Python provides various functions and variables that are used to manipulate different parts of the Python runtime environment. It allows operating on the interpreter as it provides access to the variables and functions that interact strongly with the interpreter. Let’s consider the below example.
## Random
- Python Random module is an in-built module of Python which is used to generate random numbers. These are pseudo-random numbers means these are not truly random. This module can be used to perform random actions such as generating random numbers, print random a value for a list or string, etc.

## NumPy
- NumPy is used for working with arrays.
- NumPy is short for "Numerical Python".

### NumPy Creating Arrays
- NumPy is used to work with arrays. The array object in NumPy is called ndarray.
We can create a NumPy ndarray object by using the array() function.

### Dimensions in Arrays
- A dimension in arrays is one level of array depth (nested arrays). 
nested array: are arrays that have arrays as their elements.
- 0-D arrays
0-D arrays, or Scalars, are the elements in an array. Each value in an array is a 0-D array.
- 1-D arrays : An array that has 0-D arrays as its elements is called uni-dimensional or 1-D array. These are the most common and basic arrays.
- 2-D arrays : An array that has 1-D arrays as its elements is called a 2-D array. These are often used to represent matrix or 2nd order tensors.
- 3-D arrays : An array that has 2-D arrays (matrices) as its elements is called 3-D array. These are often used to represent a 3rd order tensor.

### Check Number of Dimensions?
- NumPy Arrays provides the ndim attribute that returns an integer that tells us how many dimensions the array have.

### Access Array Elements
- Array indexing is the same as accessing an array element.
- You can access an array element by referring to its index number.
- The indexes in NumPy arrays start with 0, meaning that the first element has index 0, and the second has index 1 etc.

### NumPy Array Slicing
- Slicing in python means taking elements from one given index to another given index.
- We pass slice instead of index like this: [start:end].
- We can also define the step, like this: [start:end.:step]. 
- If we don't pass start its considered 0
- If we don't pass end its considered length of array in that dimension
- If we don't pass step its considered 1
