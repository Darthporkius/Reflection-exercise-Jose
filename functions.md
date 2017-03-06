# Functions
A function is a set of instructions that belong together.

Two kinds of functions:
	* Named functions: Will work when it is called.
	* Anonymous functions: Will work automatically ones it's turn arrives within the scope.

## Named function
```javascript

//myFunction is the name of this function.
//Input is a variable that the function needs to opperate.
function myFunction(input) {
	console.log('This is a function!');
	var derp = 4 + 3 - input;
	console.log(derp);
}
//Call function
myFunction(3);

```

## Anonymous function
```javascript

var blarg = 3;

function() {
	var derp = 4 + 3 - blarg;
	console.log(derp);
}
```