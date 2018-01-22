To determine the prototype chain of a given object in JS look at the definition of the object. If the object was created using new:

```
var myObj = new aObject();
myObj -> aObject.prototype -> Object.prototype -> null
```

Create an object using create:

```
myObj = Object.create(aObject);
myObj -> aObject -> Object.prototype -> null
```

Create a function:

```
myFunc = function(){ };
myFunc -> Function.prototype -> Object.prototype -> null
```
Create an array:

```
myAry = [];
myAry -> Array.prototype -> Object.prototype -> null
```
