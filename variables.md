# Variables

There are four types of variables:
- **Instance variable** (non static fields): objects store their individual states in 'non static field' (can be accessed through the instance)
- **Class variable** (static fields): any field declared with the static modifier (it tells the compiler that there is excatly one copy of this variable in existence), these fields share its values among all of the class' object (instance) 
- **Local Variable**: a method often store its temporary state in local variables (depends on the location in which the variable is declared)
	are only visible to the methods in which they are declared, they are not accessible from the rest of the class
- **Parameters**: declared in the methods specifications

Every variable has three attributes: ***name***, ***type***, ***value***.

####Naming: 
-case-sensitive, unicode letters and digits, beginning with a letter, $ or _ (underscore)
-the convention is to always begin your variable names with letter (and the dollar sign is never used at all)
-white space is not permitted
-if the name is consists of more than one word, capitalize the first letter if each subsequent word
-constant values: capitalize every letter and separating subsequent words with underscore (By convention the underscore character is never used elsewhere) 

e.g.: variables: `exampleVariable1`, `_exampleVariable2`, constants: `GRAVITY_ON_EARTH`, `PI`

####Type:
-Java is a type specific language, that means every variable has a type.
-We diferrentiate 2 category within types: ***primitive*** and ***reference***:
+primitive types are the built in types that are already declared by the language
+reference types are the classes


