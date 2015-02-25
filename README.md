# Definitions #
 - Unary Operator
 - Binary Operator
 - Block
 - RHS
 - LHS
 - Primitive
 - Value
 - Variable

# Operators #
 Operator    | Left Hand Side(LHS) | Right Hand Side(RHS)         | Phrase Returns                       | Example
-------------|---------------------|------------------------------|--------------------------------------|--------
 +           |number               |primitive                     |Sum of LHS and RHS                    |`12+6; //Phrase returns 18` <br> `12+"6"; //Phrase returns 18`
 +           |string               |primitive                     |Concatentation of LHS and RHS         |`"12"+"6"; //Phrase returns 126` <br> `"12"+6; //Phrase returns 126` <br> `"The cow is " + "blurple?!"; //Phrase returns "The cow is blurple?!"`
 -           |Primitive            |primitive                     |Difference of LHS and RHS             |`12-6; //Phrase returns 6`
 -           |n/a                  |primitive                     |Negative value of RHS                 | `- 12; //Phrase returns -12` <br> `- "12";//Phrase returns -12`
 *           |primitive            |primitive                     |Product of LHS and RHS                |`12*6; //Phrase returns 72`
 /           |primitive            |primitive                     |Quotient of LHS and RHS               |`12/6; //Phrase returns 2`
 %           |primitive            |primitive                     |Remainder of LHS and RHS              |`12%6; //Phrase returns 0` `13%6; //Phrase returns 1`
 !           |n/a                  |primitive                     |The opposite of RHS's truthiness      |`!2;//Phrase returns false` <br> `!0;//Phrase returns true` <br> `!true;//Phrase returns false` <br> `!"Door Knob";//Phrase returns false` <br> `!null;//Phrase returns true` <br> `!undefined;//Phrase returns true` <br>
 instanceof  |function/object      |function/object               |Tests whether LHS inherits from RHS   |`function a() {};` <br> `function b() {};` <br> `var c = new a();` `a instanceof b;//Phrase returns false` <br> `c instance of a;//Phrase returns true;`
 typeof      |n/a                  |object/function/primitive     |String representation of value's type |`typeof "this";//Phrase returns "string"` <br> `typeof 5;//Phrase returns "number"` <br> `typeof true;//Phrase returns "boolean"` <br> `typeof [];//Phrase returns "object"`

# Comparators #
Operator     | Phrase Returns                                    | Example
-------------|---------------------------------------------------|--------
 ==          |Whether LHS and RHS are equal(ish)                 |`"0" == 0;//Phrase returns true` <br> `"0" == false;//Phrase returns true` <br> `1 == true;//Phrase returns true` <br> `"false" == false;//Phrase returns false` <br> `"dog" == "doge";//Phrase returns false` <br> `"dog" == "dog";//Phrase returns true`
 ===         |Whether LHS and RHS are equal                      |`"12" === 12;//Phrase returns false` <br> `"0" === false;//Phrase returns false` <br> `1 === true;//Phrase returns false` <br> `"false" === false;//Phrase returns false` <br> `"dog" === "doge";//Phrase returns false` <br> `"dog" === "dog";//Phrase returns true`
 <           |Whether LHS is less than RHS                       |`2<5;//Phrase returns true` <br> `5<2;//Phrase returns false` <br> `5<5;//Phrase returns false`
 <=          |Whether LHS is less than  or equal to RHS          |`2<=5;//Phrase returns true` <br> `5<=2;//Phrase returns false` <br> `5<=5;//Phrase returns true`
 >           |Whether LHS is greater than RHS                    |`2>5;//Phrase returns false` <br> `5>2;//Phrase returns true` <br> `5>5;//Phrase returns false`
 >=          |Whether LHS is greater than or equal to RHS        |`2>=5;//Phrase returns false` <br> `5>=2;//Phrase returns true` <br> `5>=5;//Phrase returns false`
 !=          |Whether LHS is not equal RHS                       |`"0" != 0;//Phrase returns false` <br> `"0" != false;//Phrase returns false` <br> `1 != true;//Phrase returns false` <br> `"false" != false;//Phrase returns true` <br> `"dog" != "doge";//Phrase returns true` <br> `"dog" != "dog";//Phrase returns false`
 &&          |Whether LHS and RHS are true                       |`true && true;//Phrase returns true` <br> `true && false;//Phrase returns false` <br> `false && true;//Phrase returns false` <br> `false && false;//Phrase returns true`
 ǀǀ          |Whether LHS or RHS is true                         |`true ǀǀ true;//Phrase returns true` <br> `true ǀǀ false;//Phrase returns true` <br> `false ǀǀ true;//Phrase returns true` <br> `false ǀǀ false;//Phrase returns true`

# Incrementors #
Operator       | Phrase Assigns                      | Phrase Returns | Example
---------------|-------------------------------------|----------------|--------
 ++ (on right) |LHS to 1 greater than previous value | New value      |`var a = 3` <br> `a++;//Returns 3 and a = 4`
 -- (on right) |LHS to 1 less than previous value    | New value      |`var a = 3` <br> `a--;//Returns 3 and a = 2`
 ++ (on left)  |RHS to 1 greater than previous value | Old value      |`var a = 3` <br> `++a;//Returns 4 and a = 4`
 -- (on left)  |RHS to 1 less than previous value    | Old value      |`var a = 3` <br> `--a;//Returns 2 and a = 2`

# Assignment #
Operator    | Phrase Assigns                                    | Example
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
