# Reading 08 Operators and Loops
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

