# Definitions #
 - Unary Operator
   * A unary operator is an operator that takes only a left hand or right hand component.
 - Binary Operator
   * A binary operator is an operator that takes a left and right hand component.
 - Block
   * A block is a separated sequence on lines of codes intended to operate as a unit of logic to be managed by one a various control structures.
 - Right Hand Side (RHS)
   * RHS indicates the value or variable on the right side of an operator.
 - Left Hand Side (LHS)
   * LHS Indicates the value or variable on the right side of an operator.
 - Expression
   * An expression is any sequence of values and variables and operators which can be reduced to a single return value.
 - Primitive
   * In JavaScript, number, string, and boolean are the primitive types. A primitive is any value or variable that is not a an object.
 - Object
   * Is a data structure containing multiple other values that can either be primitives or other objects.
 - Array
   * An array is a data structure containing values indexed and accessed through number values.
 - Value
   * A value is data itself, either represented by a literal or held by a variable.
 - Variable
   * A variable is a reference to a value used to access, track, and manipulate a value.
 - Literal
   * A literal is a representation of data in typed code.
 - Scope
   * Scope is a big concept.
 - Function
   * A function is a block of code for later execution that has a signature, zero or more parameters, and a return value.
 - Message
   * A message is the name of a function and arguments used to call a function.
 - Signature
   * A signature is the name of a function and parameters it accepts.
 - Parameter
   * Parameters are the variables that a function is known to accept and use as defined by its signature.
 - Argument
   * Arguments are the values given to a function when it is called by a message.
 - Return Value
   * Return value is a value that an expression evaluates to or a function is set to return.
 - Anonymous Function
   * Anonymous functions are functions that do not include a name as part of their signature.
 - Method
   * Methods are functions that belong to objects for the purpose of manipulating or reading them.
 - Property
   * A properties are the subvalues of objects.
 - Type Coercion
   * Type coercion is the feature of Javascript that allows values of different types to be evaluated against each other. Common side effects and features of type coercion include:
     + Primitives can have methods and properties by being coerced into object versions of their types.
     + null, undefined, 0 , and  "" all evaluate to false
     + String values that are numbers can be compared to number values
     + Non-string values can be concatenated to strings easily.
 - The Law of Demeter
   * Objects should be loosely coupled and agnostic about each other.
   * Don't trust strangers.
   * https://www.google.com/webhp?hl=en#hl=en&q=law+of+demeter
 - The Principle of Least Astonishment
   * People are part of the system. The design should match the user's experience, expectations, and mental models.
   * Explote and attend to the knowledge base of your users (fellow programmers).
   * https://www.google.com/?gws_rd=ssl#q=Principle+of+least+astonishment

# Operators #
 Operator    | Left Hand Side(LHS) | Right Hand Side(RHS)         | Expression Returns                   | Example
-------------|---------------------|------------------------------|--------------------------------------|--------
 +           |number               |primitive                     |Sum of LHS and RHS                    |`12+6; //Expression returns 18` <br> `12+"6"; //Expression returns 18`
 +           |string               |primitive                     |Concatentation of LHS and RHS         |`"12"+"6"; //Expression returns 126` <br> `"12"+6; //Expression returns 126` <br> `"The cow is " + "blurple?!"; //Expression returns "The cow is blurple?!"`
 -           |Primitive            |primitive                     |Difference of LHS and RHS             |`12-6; //Expression returns 6`
 -           |n/a                  |primitive                     |Negative value of RHS                 | `- 12; //Expression returns -12` <br> `- "12";//Expression returns -12`
 *           |primitive            |primitive                     |Product of LHS and RHS                |`12*6; //Expression returns 72`
 /           |primitive            |primitive                     |Quotient of LHS and RHS               |`12/6; //Expression returns 2`
 %           |primitive            |primitive                     |Remainder of LHS and RHS              |`12%6; //Expression returns 0` `13%6; //Expression returns 1`
 !           |n/a                  |primitive                     |The opposite of RHS's truthiness      |`!2;//Expression returns false` <br> `!0;//Expression returns true` <br> `!true;//Expression returns false` <br> `!"Door Knob";//Expression returns false` <br> `!null;//Expression returns true` <br> `!undefined;//Expression returns true` <br>
 instanceof  |function/object      |function/object               |Tests whether LHS inherits from RHS   |`function a() {};` <br> `function b() {};` <br> `var c = new a();` `a instanceof b;//Expression returns false` <br> `c instance of a;//Expression returns true;`
 typeof      |n/a                  |object/function/primitive     |String representation of value's type |`typeof "this";//Expression returns "string"` <br> `typeof 5;//Expression returns "number"` <br> `typeof true;//Expression returns "boolean"` <br> `typeof [];//Expression returns "object"`

# Comparators #
Operator     | Expression Returns                                | Example
-------------|---------------------------------------------------|--------
 ==          |Whether LHS and RHS are equal(ish)                 |`"0" == 0;//Expression returns true` <br> `"0" == false;//Expression returns true` <br> `1 == true;//Expression returns true` <br> `"false" == false;//Expression returns false` <br> `"dog" == "doge";//Expression returns false` <br> `"dog" == "dog";//Expression returns true`
 ===         |Whether LHS and RHS are equal                      |`"12" === 12;//Expression returns false` <br> `"0" === false;//Expression returns false` <br> `1 === true;//Expression returns false` <br> `"false" === false;//Expression returns false` <br> `"dog" === "doge";//Expression returns false` <br> `"dog" === "dog";//Expression returns true`
 <           |Whether LHS is less than RHS                       |`2<5;//Expression returns true` <br> `5<2;//Expression returns false` <br> `5<5;//Expression returns false`
 <=          |Whether LHS is less than  or equal to RHS          |`2<=5;//Expression returns true` <br> `5<=2;//Expression returns false` <br> `5<=5;//Expression returns true`
 >           |Whether LHS is greater than RHS                    |`2>5;//Expression returns false` <br> `5>2;//Expression returns true` <br> `5>5;//Expression returns false`
 >=          |Whether LHS is greater than or equal to RHS        |`2>=5;//Expression returns false` <br> `5>=2;//Expression returns true` <br> `5>=5;//Expression returns false`
 !=          |Whether LHS is not equal RHS                       |`"0" != 0;//Expression returns false` <br> `"0" != false;//Expression returns false` <br> `1 != true;//Expression returns false` <br> `"false" != false;//Expression returns true` <br> `"dog" != "doge";//Expression returns true` <br> `"dog" != "dog";//Expression returns false`
 &&          |Whether LHS and RHS are true                       |`true && true;//Expression returns true` <br> `true && false;//Expression returns false` <br> `false && true;//Expression returns false` <br> `false && false;//Expression returns true`
 ǀǀ          |Whether LHS or RHS is true                         |`true ǀǀ true;//Expression returns true` <br> `true ǀǀ false;//Expression returns true` <br> `false ǀǀ true;//Expression returns true` <br> `false ǀǀ false;//Expression returns true`

# Incrementors #
Operator       | Expression Assigns                  | Expression Returns | Example
---------------|-------------------------------------|--------------------|--------
 (on right) ++ |LHS to 1 greater than previous value | New value          |`var a = 3` <br> `a++;//Returns 3 and a = 4`
 (on right) -- |LHS to 1 less than previous value    | New value          |`var a = 3` <br> `a--;//Returns 3 and a = 2`
 ++ (on left)  |RHS to 1 greater than previous value | Old value          |`var a = 3` <br> `++a;//Returns 4 and a = 4`
 -- (on left)  |RHS to 1 less than previous value    | Old value          |`var a = 3` <br> `--a;//Returns 2 and a = 2`

# Assignment #
Operator    | Expression Assigns                                | Example
------------|---------------------------------------------------|--------
 =          |Assigns LHS variable to RHS value                  |
 +=         |Assigns LHS variable to Sum of LHS and RHS         |
 -=         |Assigns LHS variable to Difference of LHS less RHS |
 *=         |Assigns LHS variable to product LHS and RHS        |
 /=         |Assigns LHS variable to quotient of LHS over RHS   |
 %=         |Assigns LHS variable to remainder of LHS over RHS  |

# Literals #
Border | Literal | Example
-------|---------|--------
 ""    | String  | `"How now blurple cow?";`
 {}    | Object  | `{ red: "fish", blue: "fish"};`
 []    | Array   | `[1,2,3,"four"];`

# Chunking #
- ()
- {}

# Logic #
 - while()
 - for(;;)
 - if()
 - else
 - else if()
 - switch() ... case :
 - function()
 - break
 - return

# Object Accessors #
 - .
 - []
