# Variables

There are four types of variables:
- **Instance variable** (non static fields): objects store their individual states in 'non static field' (can be accessed through the instance)
- **Class variable** (static fields): any field declared with the static modifier (it tells the compiler that there is excatly one copy of this variable in existence), these fields share its values among all of the class' object (instance) 
- **Local Variable**: a method often store its temporary state in local variables (depends on the location in which the variable is declared)
	are only visible to the methods in which they are declared, they are not accessible from the rest of the class
- **Parameters**: declared in the methods specifications

Every variable has three attributes: ***name***, ***type***, ***value***.

#### Naming: 
- case-sensitive, unicode letters and digits, beginning with a letter, $ or _ (underscore)
- the convention is to always begin your variable names with letter (and the dollar sign is never used at all)
- white space is not permitted
- if the name is consists of more than one word, capitalize the first letter if each subsequent word
- constant values: capitalize every letter and separating subsequent words with underscore (By convention the underscore character is never used elsewhere) 

e.g.: variables: `exampleVariable1`, `_exampleVariable2`, constants: `GRAVITY_ON_EARTH`, `PI`

#### Type:
- Java is statically-types, which means that all variables must first be declared before they can be used.
- We diferrentiate 2 category within types: ***primitive*** and ***reference***:
+ primitive types are the built in types that are already declared by the language
+ reference types are the classes

##### Primitive types:
- predefined by the language and is named by reserved keywords
- primitive values do not share state with other primitive values

+ **byte**:     
    - 8-bit signed two's complement integer
    - has a minimum value of -128 and a maximum value of 127 (inclusive)
    - useful for saving memory in large arrays, be used instead of ***int*** where their limits help to clarify the code
				
+ **short**:    
    - 16-bit signed two's complement integer
    - has a minimum value of -32,768 and a maximum value of 32,767 (inclusive)

+ **int**:	    
    - 32-bit signed two's complement integer		
    - has a minimum value of -2^31 and a maximum value of 2^31-1 (inclusive)
    - in JSE 8 and later you can use the ***int*** to represent an unsigned 32-bit integer which has a minimum value of 0 and a maximum value of 2^32-1
    - if there is an overflow the counting continues from Integer.MIN in a cycle
		
+ **long**:	    
    - 64-bit signed two's complement integer		
    - has a minimum value of -2^63 and a maximum value of 2^63-1 (inclusive)
    - in JSE 8 and later you can use the ***long*** to represent an unsigned 32-bit integer which has a minimum value of 0 and a maximum value of 2^64-1
		
+ **float**:	
    - a single-precision 32-bit IEEE 754 floating point
    - this data type should never be used for precise values, such as currency
		
+ **double**:   
    - double-precision 64-bit IEEE 754 floating point
    - for decimal values, this data type is generally the default choice
    - this data type should never be used for precise values, such as currency
		
+ **boolean**:  
    - has only two possible values: ***true*** and ***false***
		
+ **char**:	    
    - single 16-bit Unicode character
    - It has a minimum value of '\u0000' (or 0) and a maximum value of '\uffff' (or 65,535 inclusive).


