A great way to get values from the DOM when working in anguar is the ng-model directive. Before I learned this shortcut

```
document.getElementById(“element”) 
```

was the norm. The ng-model binds the value of a certain element marked in the html:

```
<input type="text" ng-model="example"></input>
```

and makes it available to the corresponding controller’s $scope:

```
var elementValue = $scope.example;
```
