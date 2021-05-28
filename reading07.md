# Reading 07 Programming with JavaScript
## Control flow
    * control flow- is the order in which the computer executes statements in a script.
    * code is run in order from the first line in the file to the last line, top to bottom, unless the computer runns across the ( extremely frequent) structures that change the control flow, such as conditionals and loops.
    * example: a script is used to validate user data from a webpage form. the script submits validated data, should a user leave a field empty, the script prompts the user to fill it in. a conditonal structure or if...else, runs.
        * conditionals
        * loops
        * functions
## Operators
    * JavaScript has aht efollowing types of operators.
        * assignment 
        * comparison
        * Arithmetic
        * bitwise
        * logical
        * string
        * conditional (ternary)
        * comma
        * unary
        * relational
    * JavaScript has both binary and unary operators, and one special ternary operator, the conditional operator.
        * binary operator requires two operands, one before the operator and one after the operator:
            * operand1 operator operand2
            * 3+4 or x*y
        * unary operator requires a single operand, either before or after the operator:
            * operator operand
            * operand operator
            * x++ or ++x
        * Assignment operators
            *assigns a value to ites left operand based on the value of its right operand. the simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. x = y assigns the value of y to x
            * compound assignment operators
                * there are a lot [compound assignment operators table](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)
            * Return value and chaining- like most expressions, assignments like x =y have a return value. it can be retrieved by eg assigning the expression or logging it:
                * const z = (x = y); // or equivalently: const z = x = y;

                console.log(z); // Log the return value of the assignment x = y.

                console.log(x =y); // Or log the return value directly.
            * destructuring- more complex assignments, makes it possible to extract data from arrays or objects using a syntax that mirros the construction of array and object literals.
                * var foo + ['one', 'two', 'three'];
                // without destructuring
                var one = foo[0];
                var two = foo[1];
                var three = foo[2];
                //with destructuring
                var [one, two, three] = foo;
        * Comparison operators
            * compares its operans and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values. strings- compared based on standard lexicorgraphical ordering, using Unicod values. most cases, if the two operands are not of the same type, JS attempts to convert them to an appropriate type for the comparison. generally results in comparing the operands numerically. sole exceptions to type conversion within comparison involve the === and !== operators, which preform strict equality and inequality comparisons. These operators do not attempt to convert the operands to comppatible types before checking equality. 
            * comparison operators
                * equal (==) returns true if the operands are equal. 3 == var1 "3" == var1 3 == '3'
                *not equal (!=) returns true if the operands are not equal. var1 != 4 var2 != "3"
                * strict equal (===) returns true if the operands are equal and of the same type. 3 === var1
                * strict not equal (!==) returns true if the operands are of the same type but not equal, or are of different type. var !== "3" 3 !== '3'
                * Greeater than (>) returns true if the left operand is greater than the right operand. var2 > var 1 "12" > 2
                * greater than or equal (>=) Returns true if the left operand is greater than or equal to the right operand. var2 >= var1 var1 >= 3
                * less than (<) returns true if the left operand is less than the right operand. var1 < var2
                * less than or equal (<=) returns true if the left operand is less than or equal to the right operand. var1 <= var2 var2 <= 5
    * Arithmetic operators
        takes numerical values (either literals or varibales) as their operands and returns a single numerical value. stand arithmetic operators are addition (+), subtraction (-), multiplication (*), and division (/). these work as they do in most other programming languages when used with floating point numbers
    * bitwise operators
        * teats their operands as a set of 32 bits (zeros and ones), rather than as decimal, hexadecimal, or octal numbers.
    * logicl operators
        * typically used with Boolean (logical) values; when they are, they return  a boolean values, However, the && and || opertors actually return the values of one of the specified operands, so if the ese opertors are used with non-Boolean values, they may return a non-Boolean value.
    * String operators
        * In addition to the comparison operators, which can be used on sting values, the concatenation operator (+) concatentes two string values together, returning another string that is the union of the two operand strings.
            * console.log('my' + 'string'); // console logs teh string "my string".
            * the shorthand assignment opertor += can also be used to concatenate strings.
                * var mystring = 'alpha';
                * mystring += 'bet'; // evaluates to "alphabet" and assigns this values to mystring.
    * Conditional (ternay) operator
        * is the only JS operator that takes tree operands. the operator can have one of two values based on a condition. the syntax is:
            * condition ? val1 : val2
        * if condition is true, the operator has the value of val1. otherwise it has the value of val2. you can use the conditional operator anywhere you would use a standard operator.
            *var status = (age >=18) ? 'adult' : 'minor';
            * this statement assign the value "adult" to the variable status if age si eighteen or more. otherwise it assigns the value "minor' to status
    * Comma Operator
        * (,) evaluates both of its operands and returns the value of the last operand. this operator is primarily used  inside a "for" loop, to allow multiple variables to be updates each time through the loop. It is regarded bad style to use it elsewhere, when not necessary. Often  two separate statements can and should be used instead.
            *example- if "a" is a 2-dimensional array with 10 elements on a side, the fllowing code used the comma operator to update two variable at once. the code prints the values of the diagonal elements in the array: var x = [0,1,2,3,4,5,6,7,8,9] var a = [x, x, x, x, x]; for (var i = 0, j = 9; i <= j; i++, j--) // console.log('a[' + i + '][' +j + ']= ' + a[i][j]);
    * Unary opertors
        * is an opertion with only one operand.
        * delete
            *deletes an object's proper. the syntax is: 
            * delete object.property;
            * delete object[propertykey];
            * delete objectName[index];
            * delete property; //legal only within a wtih statement
            * where "object is the name of an object, "property" is an existing property, and "propertyKey" is a string or symbol referring to an existing propery.
            * the fourth form is legal only within a "with" statement, to delete a property form an object, and also for properties of the global object.
            *If the delete operator succeeds, it removes the property from the object. trying to access it afterward will yield "undefined". The "delete" operator returns true if the operation is possible; it returns false if the operation is not possible.
            * x = 42; // implicitly creates window.x var y= 43; var myobj = {h: 4}; // create object with property h
            * delte x; // returns false (cannot delte if created implicitly)
            * delete y; // returns false (cannot delte if declared with var)
            * delete math.pi; // returns false (cannot delte non-configurable properties)
            * delete myobj.h; // returns true (can delete user-defines properties)
    * relational operators
        * compares its operands and returns a Boolean value based on whether the comparison is true.
        * in
            * returns true if the specified property is in the specified object.
            * propNameOrNumber in objectName
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
    

