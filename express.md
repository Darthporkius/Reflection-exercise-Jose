# Express
Express is used to create routes and routers.

```javascript
//express must be installed
npm install express --save

//it must be required
const express = require('express')

//express must be run within the application.
const app = express()

//code example of a route
app.get('/', function (req,res) {
	res.render('index')
})

//To create a router
//Routers are commonly created in a separate js file. So it must me exported to the app.js for use.
const router = express.Router()

//require the router in the app.js with the router file location. example
const routers = require( __dirname + '/routers/datarouter')

//Set a url to the initiate the router within your app.js. example
app.use('/users', routers)



```