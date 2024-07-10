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


These properties can be used to simplify boolean expressions. Why is it useful? Because its possible given a truth table synthesize a equivalent boolean expression. That can be done by using the rule of the sum of products https://www.allaboutcircuits.com/textbook/digital/chpt-7/converting-truth-tables-boolean-expressions/

## Boolean functions

![A list of boolean functions](./Images/boolean_functions.png)


## Logic gates diagrams 

![Logic gates diagrams](./Images/logic_gates_symbols.png)

## Proving the theorems 

![Boolean functions from NAND](./Images/basic_gates_from_nand.png)

By reacreating the NOT, AND and OR from NAND its possible to prove that both theorems are valid by using an existance proof.

- NOT is created by only inputing one varible into the terminals of a NAND gate.
- AND is created by inputing the output of a NAND gate into the terminals of another NAND gate.
- OR is  created by inputing x and y into NOT gates followed by a NAND gate

## Why?

![Logic gates from switches](./Images/basic_gates_from_switches.png)
It is much simpler to construct ANDs, ORs and NOTs with switches, so why would someone build logic gates with nand? A possible explanation is standardtization. All the other gates are built in different ways, but when a manufacture uses the same building block over and over, even if the design requires more parts, the standardtization winns on volume and easy of manufacture.

## Multiplexer and Demultiplexer

The multiplexor was constructed by using the truth table and extracting the boolean expression using the sum of products rule and than reducing the expression using the boolean identies. 

![Multiplexer simplification](./Images/multiplexer_simplification.png)

But the demultiplexer taught an important lesson. It can be constructed from the truth table, but it should be viewed as independent parts not summed together as the multiplexer was. It is not a sum.

![Demultiplexer simplification](./Images/demultiplexer_simplification.png)