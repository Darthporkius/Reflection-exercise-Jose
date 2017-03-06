# Promises
It is a way to chain functions together while passing the
returned data to the next upcomming function.

```javascript

//Here we construct a promise within the userdata
//variable so we can use it multiple times.
var userdata = function (target) {
	return new Promise( function(resolve,reject) {
		fs.readFile(target, 'utf-8', function (err,data) {
			if (err) return reject(err)
			resolve (JSON.parse(data))
		})
	})
}

//Here we call the promise within the app.get.
//We can us .then to add something to do ones
//the promise is done. The result of the promise is
//passed into the .then. I this case it is parsedUserdata.
app.get( '/allusers', function (req,res) {
	userdata( __dirname + '/users.json').then(function (parsedUserData) {
		res.render('allusers', {
		parsedUserData	
		})
	}).catch (console.log.bind(console))
})

```