# For loops
Used to go through an array and do something at every
position

```javascript

//Array
var myArray = [
	"picard",
	"kirk",
	"janeway"
];

//for loop
for (i=0; i<myArray.length; i++) {
	console.log(myArray[i]);
}

```

# while loops
The while loop will keep going through the lines
of code within it as long as the specified conditions are true.

```javascript

var lives = 10;

while (lives < 0) {
    console.log('You are alive.');
    lives--;
}

```
