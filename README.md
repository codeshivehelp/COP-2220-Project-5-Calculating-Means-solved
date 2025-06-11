# COP-2220-Project-5-Calculating-Means-solved

Download Here: [COP 2220 Project 5: Calculating Means solved](https://jarviscodinghub.com/assignment/project-5-calculating-means-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

In this project we will calculate the means of a set of positive numbers in three different ways.
Within this project we will also practice file IO by reading the input from a file, and outputting the
resulting calculations to a file.
Step 0: Generate a test input file as a text file. It should look something like this:
Step 1: PrintMenu function
This function has signature: char PrintMenu()
● It takes no arguments as input
● Outputs the user’s choice as a character.
Pseudocode for PrintMenu
● Prints the menu for the user
● Reads in the user’s choice as a character
● If the user’s choice is not one of the options given it prints an error message and asks
the user to enter a selection again.
● Otherwise it returns the user’s character choice.
Step 2: In the main you need a do loop that will call the PrintMenu function and contains an if
statement to complete each of the options given for choices A, B, C, D, P, W, Q. This loop
continues until the user enters the choice to quit.
Step 3: Choice A/a (enter the data). In this section of the code we will open a file, count the
number of positive elements in the file, allocate a dynamically size array of this size, and fill the
array with the positive elements
The pseudocode for choice A is as follows:
● Ask the user to input a file name. To read a string into the code do the following:
char filename[120];
printf(“Enter input filename: \n”);
scanf(” %s”, filename);
● Open the file
● If the file open is unsuccessful print an error message
● Else read through all the elements in the file and count the number of values greater
than zero in the file
● As long as there are more than 0 positive elements in the file do the following:
○ Allocate a dynamically sized array of doubles using malloc
double *a;
○ Rewind the file to move the cursor back to the beginning of the file
rewind(myfile)
○ Use a loop to fill the array with the positive numbers in the file.
● Close the file.
● If this file read was successful, set a flag that says the input was successful.
Note:
You can create a function to do some of this work if you like, however, be careful to keep your
malloc statement in the main of your code. Remember that memory declared locally in a
function, may be used for other purposes after the function is exited.
Step 4: Choice P/p, PrintArray function
The PrintArray function prints the elements of the array.
● Takes in two arguments: a pointer to an array, and the size of the array.
● It outputs nothing.
Step 5: Choice B/b, Arithmetic mean function
The Arithmetic function calculates the arithmetic mean of the numbers in the array. Given a set
of n numbers {a1, a2, a3,…an} calculate:
Step 6: Choice C/c, Geometric mean function
The Geometric function calculates the geometric mean of the numbers in the array. Given a set
of n numbers {x1, x2, x3,…xn} calculate:
Step 7: Choice D/d, Harmonic mean function
The Harmonic function calculates the harmonic mean of the numbers in the array. Given a set
of n numbers {x1, x2, x3,…xn} calculate:
Step 8: Step W/w, PrintResultsToFile function.
This function prints the calculation results to a file.
The pseudocode for this function is:
● Ask the user for an output file name
● Open the file
● If the open is not successful print an error message
● Otherwise, print the values of the three means to the file (call the functions to do so)
● Close the file
Requirements:
● Make the output of our solution match the given executable.
● Steps B, C, D, P and W must only be executed if valid input was received in part A.
● Your code must contain six functions:
○ char PrintMenu();
○ void PrintArray(double* arr, int N);
○ double Harmonic(double* arr, int N);
○ double Arithmetic(double* arr, int N);
○ double Geometric(double* arr, int N);
○ void PrintResultsToFile(double* arr, int N);
