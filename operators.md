# Operators

>Operators are special symbols that perform specific operations on one, two, or three operands, and then return a result.
The operators in the following table are listed according to precedence order.
When operators of equal precedence appear in the same expression, a rule must govern which is evaluated first. 
All binary operators except for the assignment operators are evaluated from left to right (assignment operators are evaluated right to left)


| Operators             | Precedence |
| --------------------- | ---------- |
| postfix	            | expr++ expr-- |
| unary	                | ++expr --expr +expr -expr ~ ! |
| multiplicative        | * "/" % |
| additive              | + - |
| shift	                | << >> >>> |
| relational            | < > <= >= instanceof |
| equality              | == != |
| bitwise AND           | 	& |
| bitwise exclusive OR  | 	^ |
| bitwise inclusive OR  | 	'|' |
| logical AND           | 	&& |
| logical OR            | 	/|//| |
| ternary               | 	? : |
| assignment            | 	= += -= *= /= %= &= ^= |= <<= >>= >>>= |
			

	Simple assignment Operator
		the most common operator
		operand from roght to left
		can also be used to assign object references
			
	Arithmetic Operators
		+	Additive operator (also used for String concatenation)
		-	Subtraction operator
		*	Multiplication operator
		/	Division operator
		%	Remainder operator
			
		The only symbol that might look new to you is "%", which divides one operand by another and returns the remainder as its result.
		You can also combine the arithmetic operators with the simple assignment operator to create compound assignments. For example, x+=1; and x=x+1; both increment the value of x by 1.
		The + operator can also be used for concatenating (joining) two strings together

	Unary Operators
		require only one operand
		+	Unary plus operator; indicates positive value (numbers are positive without this, however)
		-	Unary minus operator; negates an expression
		++	Increment operator; increments a value by 1
		--	Decrement operator; decrements a value by 1
		!	Logical complement operator; inverts the value of a boolean

		The increment/decrement operators can be applied before (prefix) or after (postfix) the operand. The code result++; and ++result; will both end in result being incremented by one. The only difference is that the prefix version (++result) evaluates to the incremented value, whereas the postfix version (result++) evaluates to the original value.
	
	The Equality and Relational Operators
		The equality and relational operators determine if one operand is greater than, less than, equal to, or not equal to another operand
		==      equal to
		!=      not equal to
		>       greater than
		>=      greater than or equal to
		<       less than
		<=      less than or equal to
	
	The Conditional Operators
		The && and || operators perform Conditional-AND and Conditional-OR operations on two boolean expressions. These operators exhibit "short-circuiting" behavior, which means that the second operand is evaluated only if needed.
		Another conditional operator is ?:, which can be thought of as shorthand for an if-then-else statement, also known as the ternary operator because it uses three operands
	
	The Type Comparison Operator instanceof
		The instanceof operator compares an object to a specified type. You can use it to test if an object is an instance of a class, an instance of a subclass, or an instance of a class that implements a particular interface
		When using the instanceof operator, keep in mind that null is not an instance of anything.
	
	Bitwise and Bit Shift Operators
		The unary bitwise complement operator "~" inverts a bit pattern; it can be applied to any of the integral types, making every "0" a "1" and every "1" a "0"
		The signed left shift operator "<<" shifts a bit pattern to the left, and the signed right shift operator ">>" shifts a bit pattern to the right.
		The unsigned right shift operator ">>>" shifts a zero into the leftmost position, while the leftmost position after ">>" depends on sign extension.
		The bitwise & operator performs a bitwise AND operation.
		The bitwise ^ operator performs a bitwise exclusive OR operation.
		The bitwise | operator performs a bitwise inclusive OR operation.

