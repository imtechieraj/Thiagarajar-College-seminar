```javascript

// navbar.js
import React from 'react';

import { AppBar, Toolbar, Typography, Button } from '@mui/material';

import { Link } from 'react-router-dom';

  

const Navbar = () => {

return (

<AppBar position="static">

<Toolbar>

<Typography variant="h6" component="div" sx={{ flexGrow: 1 }}>

Material UI App

</Typography>

<Button color="inherit" component={Link} to="/">

Home

</Button>

<Button color="inherit" component={Link} to="/about">

About

</Button>

<Button color="inherit" component={Link} to="/contact">

Contact

</Button>

<Button color="inherit" component={Link} to="/register">

Register

</Button>

<Button color="inherit" component={Link} to="/login">

Login

</Button>

</Toolbar>

</AppBar>

);

};

  

export default Navbar;
```

```javascript
//Home Page
import React from 'react';

import { Typography } from '@mui/material';

  

const Home = () => {

return (

<div>

<Typography variant="h2">Welcome to Home Page</Typography>

</div>

);

};

  

export default Home;
```


```javascript 

import './App.css';

import { BrowserRouter, Routes, Route } from 'react-router-dom';

import Home from './components/Home';

import About from './components/About';

import Contact from './components/Contact';

import Register from './components/Register';

import Login from './components/Login';

import Navbar from './components/Navbar';

  

function App() {

return (

<div className="App">

<BrowserRouter>

<Navbar />

<Routes>

<Route path="/" element={<Home />} />

<Route path="/about" element={<About />} />

<Route path="/contact" element={<Contact />} />

<Route path="/register" element={<Register />} />

<Route path="/login" element={<Login />} />

</Routes>

</BrowserRouter>

</div>

);

}

  

export default App;
```