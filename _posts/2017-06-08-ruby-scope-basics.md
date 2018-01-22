So I was reviewing some of the basics of ruby to fill in holes in my understanding. Something I liked a ton was the scoping of variables in ruby.
There are variable types for 4 scopes:

```
$globalVar
@@classVar
@instanceVar
localVar
```

Each is assigned a turf of its own. $globalVars are available to the complete program. This means they can be read and modified anywhere.

@@classVars keeps its domain within classes.

@instanceVars are assigned to instances of a class.

localVars are scoped to a class, method or block depending on where they were defined.

How to access these variables?
All but the $globalVars must be accessed via methods created in their home scope and the attribute accessor (attr_accesor).
