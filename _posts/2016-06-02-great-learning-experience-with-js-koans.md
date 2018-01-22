I am going through the JS centric frontend of my course at bloc. My mentor gave me the Javascript Koans (http://GitHub%20-%20mrdavidlaing/javascript-koans:%20Koans%20to%20learn%20Javascript) resource and its helping me learn. So far in my curriculum I had felt I needed some extra practice. JS Koans was the answer.
A new thing I learned today while going through JS Koans :
When a variable is defined but later made equal to another variable, both variables are updated with changes.

```
var array = [1, 2, 3];
var newArray = array;
newArray[1] = "two";
console.log(array[1]);
//returns "two"
```
