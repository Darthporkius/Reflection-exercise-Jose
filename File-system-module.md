# File system module
This is an npm module better known as fs.
It's purpose is to manipulate files in variuos ways such as reading and writing.

```javascript
//To install. Pending the package.json exsists.
npm install file-system --save

//the module must be required
var fs = require('fs');

//code example
//fs.readFile is beining used within a promise to read the "target" file.
var userdata = function (target) {
	return new Promise( function(resolve,reject) {
		fs.readFile(target, 'utf-8', function (err,data) {
			if (err) return reject(err)
			resolve (JSON.parse(data))
		})
	})
}

```