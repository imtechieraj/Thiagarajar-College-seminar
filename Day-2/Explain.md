# Start BackEnd Setup

### 1. Create New Repo for server

```
git clone <repo url>
```

### 2. NPM init

```
npm init 
or 
npm init -y
```

### 3. Create  Node server and Run

```js
const express = require('express');
const app = express();

app.use(express.json());
```

>.         The `express.json()` method in Express.js is a built-in middleware function that is used to parse incoming requests with **JSON payloads**. It is based on the `body-parser` middleware, and it helps extract JSON data from HTTP request bodies so that it can be accessed as a JavaScript object in your route handlers.
### 4.  Install Bcrypt and JWT

```
npm i jwt
npm i jsonwebtoken
```

```js
const bcrypt = require('bcryptjs');
const jwt = require('jsonwebtoken');

```
### 5. Install Mongoose 

```
npm i mongoose
```

``` js
const mongoose = require('mongoose');
```

### 6. DB connection

```js
const uri = "mongodb+srv://wissenskill:hOODUfqG4BZO49Ct@usermanagement.glmti.mongodb.net/myapp?retryWrites=true&w=majority&appName=UserManagement";

  

mongoose.connect(uri)

.then(() => console.log('MongoDB connected'))

.catch(err => console.error(err));
```
### 7. Create User Schema

```js
//userSchema.js

const mongoose = require('mongoose');

const UserSchema = new mongoose.Schema({

username: { type: String, required: true },

email: { type: String, required: true },

password: { type: String, required: true }

});

module.exports = mongoose.model('User', UserSchema);
```

import server.js

```js
const User = require('./userSchema');
```

### 8. Register API Creation

```js
app.post('/register', async (req, res) => {

const { username, email, password } = req.body;

const hashedPassword = await bcrypt.hash(password, 10);

const newUser = new User({ username, email, password: hashedPassword });

await newUser.save();

res.status(201).send({status:true,message:"User Registered"});

});
```

### 9. Login API

```js
app.post('/login', async (req, res) => {

const { username, password } = req.body;

const user = await User.findOne({ username });

if (!user) return res.status(400).send({ status: false, message: "User not found" });

  

const isMatch = await bcrypt.compare(password, user.password);

if (!isMatch) return res.status(400).send({ status: false, message: "Invalid credentials" });

  

const token = jwt.sign({ id: user._id, username: user.username, email: user.email }, "secret", { expiresIn: '1h' });

res.json({ token });

});
```

### 10.  Postman : API Testing


### 11. API Integration 

Install axios

```js
npm i axios
```


```js
axios.post('http://localhost:5000/register', {username, email, password}).then((result)=>{

console.log(result)

navigate('/login');

}).catch((error)=>{

console.log(error.response.data)

});
```