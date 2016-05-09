# Data Types

JavaScript supports six types of data types. Of the six data types five of them are primitive data types

### Primitive Data Types

- string
- number
- boolean
- undefined
- null

### Non Primitive Data Types
- object

### The String Type
- The string data type is used to represent textual data
- it is a set of elements of 16-bit unsigned integer values
- Each element string occupies a position  in the String
    - for example the first element is at index 0 and the next one is at index 1, and so on 

#### Examples
     /*
      * A JavaScript string can be surrounded by double-quotes or single-quotes
      * which ever you use doesn't matter just make sure you are consistant 
      * you can also escape a double or single quote with in the string which
      * you will see in the below example
      */
      
      //String surrounded by a single quote 
      console.log('Hello, World!');
      
      //String surrounded by a double quote
      console.log("Hello, World!");
      
      //Escaping a single quote 
      console.log('Dont\'t');
      
      //Escaping a double quote
      console.log("This is a \"quote\"");
      
      //using a single quote inside a double quote 
      console.log('This is a "quote"');

#### The Number type

##### Whole Numbers and Floats
The number type can be an integer whole number such as 1 or 2 or 3, or floating point decimals or floats such as 3.14159 either way JavaScript will treat them as a number.

    //Whole number
    console.log( 1 );
    
    //Floats
    console.log( 3.14159);

##### Octal and Hexadecimal Numbers
If a number starts with a **0x**, then it is treated as a **hexadecimal** (base16) notation, which is used for color codes when working with css.

    //Hexadecimal Number
    console.log(0xAF); // Where A Represents 10, F represents 15
    
If a number starts with a **zero** it is considered to be in **octal** (base 8) notation

    //An Octal Number
    console.log(047) //4 eights and 7 units

#### Exponential Notation
You can represent a number as exponential notation or scientific notation, which is shorthand for multiply by 10 to the power of.

    //Example of Exponential Notation
    console.log(1e6); // or 1 multiplied by 10 to the power of 6 (or a million)
    
#### Boolean Type
The Boolean type represents a logical entity and can have two valets **true**, and **false**

    //This will return a true value
    console.log(1==1) //returns true because 1 is equal to 1
    
    //This will return a false value
    console.log(1==2) //returns false because 1 is not equal to 2
#### Undefined type
A variable that is not been assigned a value will return undefined.
    
    //This statement will return undefined
    console.log(a); //we never assigned a value to a so it will return undefined
    
    //This state will return a value
    var a = "Hello, World!";
    console.log(a); //This will return Hello, World!, because we have defined the variable a 

#### Null type
The Null type has the value of null assigned to the varaible;

    //The varaible has null value assigned to it 
    var a = null;
    console.log(a);
    
#### Object Type

#### typeof




