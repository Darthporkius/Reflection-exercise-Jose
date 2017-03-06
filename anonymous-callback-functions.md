# Anonymous callback functions
This is an anonymous function that is called
after something else is done. 

```javascript
var myArray = [
	"picard",
	"kirk",
	"janeway"
];
​
myArray.forEach(function (captain){
console.log(captain);
});

//the function that does the console.log is 
//an anonymous callback function.

```