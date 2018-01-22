Reviewing the fundamentals of Js I found a topic that was very unclear. Upon reading various sources, specially this source by Joshua Clanton, and speaking to my mentor everything slowly started to fall into place.
What hoisting does is that it “hoists” variable and function declarations to the top. Variable example:
```
console.log(test); //returns undefined
var test = "I am a test string";
console.log(test); //returns "I am a test string";
```
What is happening here is that the scope looks for the variable “test” and finds it declared. Since its declared after its call Js acknowledges its existence but not its definition.
Function example:
```
var val = 4; 
//Function Expression
var printVal = function() {
     return 8; 
};  
//Function Declaration
function printVal() {  
   var val = 6;     
   return val + 5; 
}
printVal(); // returns 8
```
In this example the function declaration is hoisted to the top. In javascript function declarations get hoisted over function expressions. When the printVal() function is called, the function expression lies at the end of the code thus returning 8.
