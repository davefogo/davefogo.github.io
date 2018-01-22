A fun thing I learned while working on HeyChat! (web app for chatting based on Angular and Firebase) is how to clear an input element of text after it has been submitted. It’s actually quite easy:
The first step is to have your html element labled with an ng-model directive (an angular directive) and your submit button with a type=”submit”:

```
<input type="text" ng-model="textInput">Enter your text here</input>
<input type="submit"></input>
```

The second step is to assign ng-submit to the form that encapsulates the input field labeled above.

```
<form ng-submit="submit()">
  <input type="text" ng-model="textInput">Enter your text      here</input>
</form>
```

The last step has you set the $scope.textInput to null in your corresponding controller. This must be done inside the function that is fired on submission.

```
var sendMessage = function() {
 //your function content
 $scope.textInput = null;
};
```

Using this technique will allow you to have the text you entered in an input element dissapear after submission.
