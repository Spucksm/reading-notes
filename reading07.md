# Reading 07 Programming with JavaScript
## Control flow
    * control flow- is the order in which the computer executes statements in a script.
    * code is run in order from the first line in the file to the last line, top to bottom, unless the computer runns across the ( extremely frequent) structures that change the control flow, such as conditionals and loops.
    * example: a script is used to validate user data from a webpage form. the script submits validated data, should a user leave a field empty, the script prompts the user to fill it in. a conditonal structure or if...else, runs.
        * conditionals
        * loops
        * functions

## Functions
    * fundamental building blocks in JS. similar to aprocedure- a set of statements taht performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. to use a function, you must define it somewhere in the scope from which you wish to call it.
### defining functions
    * function declarations
        * function definition (also called a function declartion, or function statement) consists of the "function" keryword, followed by:
            * the name fo the function
            * a list of parameteres to the function, enclosed in parentheses and separated by commas.
            * The JS statements that define the function, enclosed in curly brackets, "{...}"
            * function square(number) {return number * number;}
            * the function square takes one pareameter, called number. the function consists of one statement that says to return the parameter of the function (that is, number) multiplied by itself. The statement return specifies the value returned by the function:
                * return number * number;
            * primitive parameters (such as a number) are passed to functions by value; the value is passed to the function, but if the function changes the value of the parameter, this change is not reflected globally or in the calling function.
            * If you pass an object (ie. a non-primitive value, such as "array" or a user-defined object) as a parameter and the function changes the object's properties, that change is visible outside the function.
### Predefined functions
    * "eval()"- evaluates JS code represented as a string.
    * "uneval()"- method creates a string representation of the source code of an object.
    * "isFinite()"- determines whether teh passed value is a finite number. If needed, the parameter is first converted to a number.
    * "isNaN()"- determines whetere a value is "Nan" or not. 
    * "parseFloat()"- parses a string argument and returns a floating point number.
    * "parseInt()"- parses a string argument and returns an interger of the specified radix (the base in mathematical numeral systems).
    * "decodeURI()"- decodes a Uniform Resource Identifer (URI) previously created by "encodeURI"
    

