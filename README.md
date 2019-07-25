# LAB - 11

## API Server

### Author: Pratiibh Bassi

### Links and Resources
* [submission PR](http://xyz.com)
* [travis](http://xyz.com)
* [back-end](http://xyz.com) (when applicable)
* [front-end](http://xyz.com) (when applicable)

#### Documentation
* [api docs](http://xyz.com) (API servers)
* [jsdoc](http://xyz.com) (Server assignments)

### Modules#### 
#### `app.js` where all the `app.use` lives in; required in `index.js`
#### `memory.js` class `Model` with `CRUD` & `sanitize` method
#### `mongo.js` class `Model` with `jsonSchema` and `CRUD` functions
#### `supergoose.js` combines SuperTest and Mongoose Memory Server
#### `swagger.js`  
#### `v1.js` handles all model routes
#### `404.js` 404 not found error
#### `500.js` 500 server error
#### `model-finder.js` middleware function `load` with a `list` that returns any model
#### `categories-models.js` class `Categories`extends from `Model` in `mongo.js` with `categories-schema.js` required in
#### `categories-schema.js` categories schema with name & desciption
#### `people-model.js` class `People` that extends from `DataModel` in `memory.js`
#### `products-model.js` extends from class Model in `mongo.js` with `products-schema.js` required in
#### `products-schema.js` schema with name, description, categories, & price
#### `todo-models.js` extends from Model in `mongo.js` with `todo-schema.js` required in
#### `todo-schema.js` schema with text, category, assignee, difficulty, & complete

##### Exported Values and Methods
#### `get` get something from database
#### `create` create something
#### `update` update something
#### `delete` delete something
#### `sanitize` removes any illegal characters

### Setup
#### `.env` requirements
* `PORT` - 3000
* `MONGODB_URI` - MONGODB_URI=mongodb://localhost:27017/class09

#### Running the app
* `nodemon`
* `localhost: 3000/docs`
* `live-server`
* `npm run jsdoc`
* Entrypoint: index.js
* Endpoint: GET /api/v1/:model
  * Returns a JSON object with requested model
* Endpoint: GET /api/v1/:model/:id
  * Returns a JSON object with requested id
* Endpoint: POST /api/v1/:model
  * Returns a JSON object with created created value
* Endpoint: DELETE /api/v1/:model/:id
  * Returns a JSON object without the deleted value
* Endpoint: PUT /api/v1/:model/:id
  * Returns a JSON object updated keys
  
#### Tests
* `npm test` to run test

#### UML
Link to an image of the UML for your application and response to events
