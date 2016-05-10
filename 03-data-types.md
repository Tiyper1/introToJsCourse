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
The object Type is a container for named values, called properties and methods, where properties are values or variables that are associated with a JavaScript object, and methods or functions are actions that are associated with a JavaScript object.

    /*
     * There are 3 ways to create an object in JavaScript.
     *  Using Object Initializers ( Object Literal )
     *  Using Object Constructor function
     *  Using Object.create method
    */
    
    //Example of creating an object Using Object Initializers
    var car = {
        "year" : 2016,
        "make" : "honda",
        "model" : "pilot",
        "color" : "gray",
        "doors" : 4,
    }
    
    console.log( car.make );
    
    //Example of creating an object using a Object Constructor function 
    var car = new Object();
    
    car.year = 2016;
    car.make = "honda";
    car.model = "pilot";
    car.color = "gray";
    car.doors = 4;
    
    console.log(car.model);
    
    //Example of creating an object using the Object.create method
    
    var car = Object.create ({});
    
    car.year = 2016
    car.make = "honda";
    car.model = "pilot";
    car.color = "gray";
    car.doors = 4;
    
    console.log(car.color);

#### typeof
To find out what data type a value has you can use the typeof method 

    // Numbers
    typeof 37 === 'number';
    typeof 3.14 === 'number';
    typeof Math.LN2 === 'number';
    typeof Infinity === 'number';
    typeof NaN === 'number'; // Despite being "Not-A-Number"
    typeof Number(1) === 'number'; // but never use this form!
    
    
    // Strings
    typeof "" === 'string';
    typeof "bla" === 'string';
    typeof (typeof 1) === 'string'; // typeof always returns a string
    typeof String("abc") === 'string'; // but never use this form!
    
    
    // Booleans
    typeof true === 'boolean';
    typeof false === 'boolean';
    typeof Boolean(true) === 'boolean'; // but never use this form!
    
    // Undefined
    typeof undefined === 'undefined';
    typeof declaredButUndefinedVariable === 'undefined';
    typeof undeclaredVariable === 'undefined'; 
    
    
    // Objects
    typeof {a:1} === 'object';
    
    // use Array.isArray or Object.prototype.toString.call
    // to differentiate regular objects from arrays
    typeof [1, 2, 4] === 'object';
    
    typeof new Date() === 'object';
    
    
    // The following is confusing. Don't use!
    typeof new Boolean(true) === 'object'; 
    typeof new Number(1) === 'object'; 
    typeof new String("abc") === 'object';
    
    
    // Functions
    typeof function(){} === 'function';
    typeof class C {} === 'function';
    typeof Math.sin === 'function';
    
    
### Demo Invoice JavaScript App

#### index.html
    <!doctype html>
    <html>
        <head>
            <meta charset="utf-8">
            <title>Demo App</title>
        </head>
        <body>
            <script src="./js/main.js"></script>
        </body>
    </html>
#### main.js
    /*
     * File main.js
     * App Name : Demo Invoice JavaScript App 
     */
    var car = {
      "year" : 2017,
    	make : "honda",
      model : "pilot",
      doors : 4,
      color : "black",
      price : 35000,
      sunRoof : true,
      radio : true,
      cdPlayer : false,
      spareTire : null,
      priceOfSatifaction : 1e309,
      
      invoice : function(){  	    
        return "The " + this.year + " " + this.make + " "  + this.model +  " comes with " + this.door + " doors and is 	         available in the color as long as it's " + this.color + ", for the special price of " + this.price + ". Act now cause the price of your satisfaction is " + this.priceOfSatifaction;
      }
    }
    
    //Write the return value of the car.invoice method to the HTML file
    document.write.log(car.invoice());
    
    


