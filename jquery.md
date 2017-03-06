# jQuery
It's a javascript library. It is used to manipulate the front end. It is used for things like animations.

It must be copypasted into the project and called as a src from within the DOM.

The file containing the jquery code must also be called from within the DOM. 

```javascript
//Code example
$( document ).ready( function(  ){
	console.log( 'DOM has loaded' )
	$( 'p' ).hide( )
	$( 'h1' ).click( function( ){
		console.log( 'H1 has been clicked' )
		$( this ).hide( )
		$( 'p' ).slideDown( 5000 )
	} )
} )


```