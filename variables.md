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

##### String:	
- the String class is not technically a primitive data type, but considering the special support given to it by the language
- the language also provides special support for character strings via the ***java.lang.String*** class
- enclosing your character string within double quotes ***"*** will automatically create a new String object
- String objects are immutable
- before creating a new object, Java check if there is any String with the same value that is recently created, if so the variable will point to that value, this "cache" is called String pool 

##### Default values:
| type | value |
| ------:| -----------:|
| byte   | 0 |
| short  | 0 |
| int    | 0 |
| long    | 0L |    
| float    | 0.0f |  
| double    | 0.0d |  
| char    | '\u0000' |  
| boolean    | false |  
| String (and any reference type)    | null |  

# Literals

- primitive types are special data types built into the language (they are not objects created from a class)
- a literal is the source code representation of a fixed value
- literals are represented directly in your code without requiring computation
- it's possible to assign a literal to a variable of a primitive type
		
##### integer literals:
- an integer literal is of type ***long*** if it ends with the letter ***L*** or ***l***, otherwise it is of type ***int*** 
- ***L*** is more readable than ***l***		
- values of the integral types ***byte***, ***short***, ***int***, and ***long*** can be created from ***int*** literals
- values of type ***long*** that exceed the range of ***int*** can be created from ***long*** literals
- decaimal: Base 10, 0-9
- Hexadecimal: Base 16, 0-9 and A-F
- binary: base 2, 0-1  (you can create binary literals in Java SE 7 and later)
- if you need to use another number system: prefix 0x indicates hexadecimal and 0b indicates binary
	
##### floating point literals:
- is of type ***float*** if it ends with the letter ***F*** or ***f***, otherwise its type is ***double*** and it can optionally end with the letter ***D*** or ***d***
- the floating point types (***float*** and ***double***) can also be expressed using ***E*** or ***e*** (for scientific notation)	(x10^x ~ ...ex)
	
##### character and string literals:
- may contain any Unicode (UTF-16) characters
- if your editor and file system allow it, you can use such characters directly in your code, if not, you can use a "Unicode escape" such as '\u0108' (capital C with circumflex)
- special escape sequences: **\b** (backspace), **\t** (tab), **\n** (line feed), **\f** (form feed), **\r** (carriage return), **\"** (double quote), **\'** (single quote), and **\\** (backslash)
	
There's also a special **null** literal that can be used as a value for any reference type. ***null*** is often used in programs as a marker to indicate that some object is unavailable
There's also a special kind of literal called a **class** literal

##### Using Underscore Characters in Numeric Literals
- any number of underscore characters (_) can appear anywhere between digits in a numerical literal
- separate groups of digits in numeric literals, which can improve the readability of your code
- you can place underscores only between digits
- you cannot place underscores in the following places:	
    - at the beginning or end of a number
    - adjacent to a decimal point in a floating point literal
    - prior to an ***F*** or ***L*** suffix
    - in positions where a string of digits is expected

