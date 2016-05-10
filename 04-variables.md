# Variables

In the previous module you have seen some examples where we used variables to output values that were assigned to it.
So variables are containers that you can assign values, functions, or any object to which will then be stored in memory for later use. To Declare a variable you have to use the optional keyword **var** followed by the name of the variable with an optional value. 

Note: Declaring a variable is optional but is not best practice 

#### Examples of variable

    //A variable with no value 
    var a;
    
    console.log(a) //returns undefined
    
    //A variable with a value 
    var b = "Hello, World!";
    
    console.log(b); //returns Hello, World!
    
    //Assigning an object to a variable 
    var c = {
        firstname : "john",
        lastname : "doe",
    };
    
    console.log(c.firstname); //returns john
    
    //Assigning a function to a variable
    var d = function(){
        return "Hello, World!";
    }
    
    console.log(d()); //returns Hello, World!
