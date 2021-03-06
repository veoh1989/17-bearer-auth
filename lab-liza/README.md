# Lab 17 - Bearer Authorization

**Author**: Liza Oh

## Overview
Basic authorization middleware and signup/signin routes

## Getting Started
The user must:
* Npm init their project
* Brew Install HTTPIE/Use Postman
* Brew Install Mongo
* Npm i to install packages

#### Configuration
* `package.json`
* `.eslintrc`
* `.gitignore`
* `.env`
* `.test.env`

## Examples:
**POST example:**
```
http POST :3000/api/v1/signup username=testuser password=testpassword email='test@test.com'
```

**GET example:**
```
http -a testuser:testpassword :3000/api/v1/signin
```

## Running the tests
* `/api/signup`
* `POST` - test **400**, if no request body has been provided or the body is invalid
* `POST` - test **200**, if the request body has been provided and is valid
* `/api/signin`
* `GET` - test **401**, if the user could not be authenticated
* `GET` - test **200**, responds with token for a request with a valid basic authorization header

## Built With
* [Javascript](https://www.javascript.com/)
* [npm](https://www.npmjs.com/)
* [jest](https://www.npmjs.com/package/jest)
* [body-parser](https://www.npmjs.com/package/body-parser)
* [cors](https://www.npmjs.com/package/cors)
* [express](https://www.npmjs.com/package/express)
* [jsonwebtoken](https://www.npmjs.com/package/json-web-token)
* [mongoose](http://mongoosejs.com/docs/api.html)
* [faker](https://www.npmjs.com/package/Faker)
* [superagent](https://www.npmjs.com/package/superagent)