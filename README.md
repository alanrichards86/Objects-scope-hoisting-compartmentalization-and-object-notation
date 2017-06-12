## Scope, hoisting and compartmentalization

### Answer the following:
In you own words, explain the concepts of scope, hoisting, compartmentalization.

Scope is how things are / where tings are located in the coding sphere and how we access them.
Hoisting is an order of operations of sort. How things are supposed to be layed out in the code.
Compartmentalization is how the code is contained / structured.
### Provide examples for all three, below:

#### Scope:
 var hi = 'hi';     <----- Global Scope. Can be accessed anywhere.

function hello (){
  var hey = 'dear';   <---- Local scope. Can only be accessed in this function.
}
#### Hoisting:

function hi() {
  console.log(pickle);    <---This would get dropped below the variable and the variable would be brought above it.
  var pickle = "this is a good pickle";    <------ var pickle would be brought to the top of the function and the assingment with the string would be brought below it.    
    console.log(pickle) would fall to the bottom because it is read last in this setup.
}


#### Compartmentalization:

function() {

(function (){
  This function is Compartmentalized away from everything thing else. Its variables would not be accessable because of local scope coming into play. The function does not have to be an IFFY but its just being used as an example.
  })();
}
