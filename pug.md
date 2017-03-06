# Pug
Pug is a templating language for javascript.
It is only used in the front end. It is possible to pass
data from the backend to pug so it can be renderd and manipulated. 

It is possible to de functions in pug.

Indentacions are very important in pug. You can use spacings of tabs but never
bolth. It will break the code. 

```pug
doctype	html
html
	head
		title = userspage
	body
		div.container
			h1 Welcome to Date4Less
			hr
			img(src="https://68.media.tumblr.com/18bbc815e4c641246df8a28c9633d392/tumblr_mtjxfgMy9K1s3figho1_400.gif") 
			hr
			a( href="/adduser" ) Register.
				a( href="/allusers") Our Users.
			hr
			h2 Search for a mate.
			form( action="/search", method="post")
				input( type="text", name="search", placeholder="Find a lass or lad")
				input( type="submit")
			block content	

```

For pug to work the view engine must be set to pug
and the file with the pug file must be declared.
```javascript

//declare the file with the pug files.
app.set('views', __dirname + '/views')

//Set the view engine to pug.
app.set('view engine', 'pug')

```