# Cookies
Cookies are files that are stored client side.
They are used to store information like userID's and data entered into the DOM. 
This way the information isn't lost if the session times out or if the page reloads.

Just like jquery the cookie library must be copypasted into teh project in the form of a js file.
The file must then be called from within the DOM just like jquery.

```javascript
//To parse the cookies to a readable object format
//cookie-parser is needed.
npm install cookie-parser --save

//require the cookie-parser and the app must use it.
const cookieparser = require( 'cookie-parser' )

app.use( cookieparser( ) )

```

Now you are ready to work with cookies.