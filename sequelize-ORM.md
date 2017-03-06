# Sequelize ORM
ORM stands for Object Relational Mapping.
Sequelize is used to create tables and manipulate databases with javascript. 

```javascript
//Sequelize must be required
const sequelize = require( 'sequelize' )

//An existing database must be declared.
const db = new sequelize( 'name-of-db', 'username', 'password', {
  host: 'localhost',
  dialect: 'postgres'
} )
//The dialect refers to the database management app
//you are using.

``` 
Afther these two steps you are ok to create tables and to populate them.

Sequelize works with promises.