# Boolean-Function-Simplifier
Program minimizes boolean functions to use the lowest number of logic gates.

# Introduction
Here is a short runthrough of how the user interacts with the program. The user will input names for each boolean variable and then enter in information from the truth table in the form of minterms. With this information, the program performs the [Quine-McCluskey method](https://en.wikipedia.org/wiki/Quine%E2%80%93McCluskey_algorithm) to reduce the function to the lowest number of terms which it then outputs. The purpose of this program is to reduce the cost and complexity of circuits and is especially usefull when the function has lots of boolean variables.

# Structure of Program
The program loosely adheres to the[ Model-view-controller](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller) software design pattern. The view and controller, parts which interact with the user are put together in one file "UserInterface.py". Once this file has the information, it calls upon the "CalculateAnswer.py" file to run the calculations. To do this "CalculateAnswer.py" utilizes methods from the "GetCoreMinterms.py" and "BooleanFunctionSimplifier.py". Once the answer is calculated, it then goes back into "UserInterface.py" to display for the user.
