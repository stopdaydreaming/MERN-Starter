# MERN-Starter

## Basic Setup
1. touch server.js
2. `npm init -y`
3. `npm install express mongoose`

# Build the Express App
1. Require express
2. Create instance of express
3. Set the server PORT to 3001
4. Listen to the PORT
5. Add middleware
```javascript
app.use(express.urlencoded({ extended: true}));
app.use(express.json());
```
6. Add routes

** Great time to test your server using Postman **

## Add MongoDB/Mongoose to the Server
1. Require mongoose in the server
2. Setup the mongoose connection
3. Add mongoose config object to the .connect method
```
javascript
{
    useNewUrlParser: true,
    useUnifiedTopology: true,
    useFindAndModify: false,
    useCreateIndex: true
}
```
4. Add promise .then and .catch for Mongoose connection