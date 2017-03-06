# Body parser
It is used to parse input that is comming from the DOM.

```javascript

//It must be npm installed.
npm install body-parser --save

//It must be required in the app.js
const bodyparser = require('body-parser')

//It is used by the app as middelware.
app.use( bodyparser.urlencoded( { extended: true}))  


```
