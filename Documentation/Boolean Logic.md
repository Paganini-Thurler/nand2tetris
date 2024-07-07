# Boolean algebra 

It's common to hear: "Computers work with ones and zeros or with binary digits". This statement is correct, but it misses the important 
explation of how can a value like 0 or 1 create something so complex as a computer. The study of boolean algebra and logic can explain with depth the why and how.


## Boolean theorems 

Any Boolean function can be expressed using only And, Or, and Not operators.
Any Boolean function can be expressed using only Nand operators.



## Boolean notation

- AND  x Ʌ y, x + y 
- OR   x V y, x . y
- NOT  ¬x, !x

## Boolean algebra

### Commutative laws

- AND x . y = y . x
- OR x + y = y + x

### Associative laws

- AND x . (y . z) = (x . y) . z
- OR x + (y + z) = (x + y) + z

### Distributive laws

- x. (y + z) = (x . y) + (x . z)
- x + (y . z) = (x + x) . (x + z)

### De Morgan's laws

- ¬(x . y)=¬x + ¬y
- ¬(x + y)=¬x . ¬y

### Indemptent laws

- x . x = x
- x + x = x

These properties can be used to simplify boolean expressions. Why is it useful? Because its possible given a truth table synthesize a equivalent
boolean expression. That can be done by using the rule of the sum of products https://www.allaboutcircuits.com/textbook/digital/chpt-7/converting-truth-tables-boolean-expressions/

## Boolean functions

![A list of boolean functions](./Images/boolean_functions.png)