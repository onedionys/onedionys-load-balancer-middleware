<h1 align="center">Welcome to One Dionys - Load Balancer Middleware! 👋 </h1>

<p align="center">Middleware to distribute traffic evenly across multiple backend servers, improving application scalability and availability. 💖 </p>

<p align="center">
<img src="https://img.shields.io/github/contributors/onedionys/onedionys-load-balancer-middleware?style=flat-square">
<img src="https://img.shields.io/github/issues/onedionys/onedionys-load-balancer-middleware?style=flat-square">
<img src="https://img.shields.io/github/stars/onedionys/onedionys-load-balancer-middleware?style=flat-square"> 
<img src="https://img.shields.io/github/forks/onedionys/onedionys-load-balancer-middleware?style=flat-square">
<img src="https://img.shields.io/github/last-commit/onedionys/onedionys-load-balancer-middleware.svg?style=flat-square">
<img src="https://img.shields.io/github/languages/code-size/onedionys/onedionys-load-balancer-middleware?style=flat-square">
<img src="https://img.shields.io/github/license/onedionys/onedionys-load-balancer-middleware?style=flat-square">
</p>

## 💾 Requirements

* `Web Browser` - Can be used as an emulator to build applications. Example [Chrome, Firefox, Safari & Opera].
* `Internet` - Because many use CDN and to make it easier to find solutions to all problems.

## 🎯 How To Use

#### Example Syntax

```javascript
const express = require('express');
const loadBalancerMiddleware = require('./src/loadBalancerMiddleware');

const app = express();

const servers = [
    { url: 'http://server1.com', weight: 1 },
    { url: 'http://server2.com', weight: 2 },
    // Add more servers as needed
];

app.use(loadBalancerMiddleware(servers));

// Add your routes and other middleware here

app.listen(3000, () => {
    console.log('Server is running on port 3000');
});
```

#### Explanation

* This middleware implements a basic load balancing algorithm to distribute incoming requests among multiple servers. It takes an array of server objects, each containing the server URL and its weight. The middleware then routes requests to the servers based on their weights.

#### Return Value

* The middleware function returns an Express middleware function that can be used in an Express application. This middleware should be placed early in the middleware stack to ensure that all requests are properly load balanced before reaching other middleware or route handlers.

## 📆 Release Date

* v1.0.0 : 17 March 2024

## 🧑 Author

* Facebook : <a href="https://www.facebook.com/theonedionys"> Oned Ionys</a>
* Instagram : <a href="https://www.instagram.com/onedionys/"> @onedionys</a>
* Twitter : <a href="https://twitter.com/onedionys"> @onedionys</a>
* LinkedIn :  <a href="https://www.linkedin.com/in/onedionys/"> @onedionys</a>

## 📝 License

* Copyright © 2024 One Dionys
* **One Dionys - Load Balancer Middleware is an open source project licensed under the MIT license**

## ☕️ Suppport & Donation

Love One Dionys - Load Balancer Middleware? Support this project by donating or sharing with others in need.

<a href="https://www.buymeacoffee.com/onedionys"><img src="https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black"/> </a>

**Made with ❤️ One Dionys**
