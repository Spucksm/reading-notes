# Reading 08 Operators and Loops
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
            * _**Following info was pulled from reading material**_ I don't understand this [relational operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)
            * // Arrays
var trees = ['redwood', 'bay', 'cedar', 'oak', 'maple'];
0 in trees;        // returns true
3 in trees;        // returns true
6 in trees;        // returns false
'bay' in trees;    // returns false (you must specify the index number,
                   // not the value at that index)
'length' in trees; // returns true (length is an Array property)

// built-in objects
'PI' in Math;          // returns true
var myString = new String('coral');
'length' in myString;  // returns true

// Custom objects
var mycar = { make: 'Honda', model: 'Accord', year: 1998 };
'make' in mycar;  // returns true
'model' in mycar; // returns true
    * instanceof
        * returns true if the specified object is of the specified object type.
        * objectName instanceof objectType
### Operator precedence
    * The precedence of operators determines the order tehy are applied when evaluting an expression. You can override operator precedence by using parentheses.
        * member ".[]"
        * call/create instance "() new"
        * negation/increment "! ` - + ++ -- typeof void delete"
        * multiply/divide "* / %"
        * addition/subtraction "+ -"
        * bitwise shift "<< >> >>>"
        * relational "< <= > >= in instanceof"
        * equality "== != === !=="
        * bitwise-and "&"
        * bitwise-xor "^"
        * bitwise-or "|"
        * logical-and "&&"
        * logical-or "||"
        * conditional "?:"
        * assignment "= += -= *= /= %= <<= >>= &= ^= |= &&= ||= ??="
        * comma ","
### Expressions
    * is any valid unit of code that resolves to a value
    * every syntactically valid expression resolves to some value but conceptally, there are two types of expressions: with side effects (for example: those that assign value to a variable) and those that in some sense evaluate and therefore resolve to a value.
    * the expression "x = 7" is an example of the first type. This expression uses the = operator to assign the value seven to the variable x. the expression itself evaluates to seven.
    
