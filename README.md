## Application Overview

we’re gonna build a Node.js Express Rest API that supports Token Based Authentication with JWT ([JSONWebToken](https://www.npmjs.com/package/jsonwebtoken)). You’ll know:
   - Appropriate Flow for User Signup & User Login with JWT Authentication
   - Node.js Express Architecture with CORS, Authenticaton & Authorization middlewares & Sequelize
   - How to configure Express routes to work with JWT
   - How to define Data Models and association for Authentication and Authorization
   - Way to use Sequelize to interact with MySQL Database

## Software Requirements

- [Node](https://nodejs.org/en/download/)
- [MySQL](https://dev.mysql.com/doc/refman/5.7/en/installing.html)


## How to install

### Using Git (recommended)

1.  Clone the project from github. Change "myNodeProject" to your project name.

```bash
git clone https://github.com/Zealous-System-Pvt-Ltd/nodejs.git ./myNodeProject
```

### Using manual download ZIP

1.  Download repository
2.  Uncompress to your desired directory

### Install npm dependencies after installing (Git or manual download)

```bash
cd myNodeProject
npm install
```

### Setting up environments

1.  You will find a file named `db.config.js` on config directory of project.
2.  Change the values of the file to your environment. Helpful comments added to `db.config.js` file to understand the constants.

## Project  structure
```sh
.
├── server.js
├── package.json
└── app
    ├── config
    │   ├── auth.config.js
    │   └── db.config.js
    ├── controllers
    │   ├── auth.controller.js
    │   ├── customer.controller.js
    │   └── user.controller.js
    ├── models
    │   ├── customer.model.js
    │   ├── db.js
    │   ├── index.js
    │   ├── role.model.js
    │   └── user.model.js
    ├── routes
    │   ├── auth.routes.js
    │   ├── customer.routes.js
    │   └── user.routes.js
    └── middleware
        ├── authJwt.js
        ├── index.js
        └── verifySignUp.js

```
## How to run

### Running  API server locally

```bash
npm run dev
```

You will know server is running by checking the output of the command `npm run dev`


### Creating new models

If you need to add more models to the project just create a new file in `/models/` and use them in the controllers.

### Creating new routes

If you need to add more routes to the project just create a new file in `/routes/` and add it in `/routes/server.js` it will be loaded dynamically.

### Creating new controllers

If you need to add more controllers to the project just create a new file in `/controllers/` and use them in the routes.
