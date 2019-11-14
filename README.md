# API Project: URL Shortener Microservice for freeCodeCamp

## User Stories

1. I can POST a URL to `[project_url]/api/shorturl/new` and I will receive a shortened URL in the JSON response. Example : `{"original_url":"www.google.com","short_url":1}`
2. If I pass an invalid URL that doesn't follow the valid `http(s)://www.example.com(/more/routes)` format, the JSON response will contain an error like `{"error":"invalid URL"}`. HINT: to be sure that the submitted url points to a valid site you can use the function `dns.lookup(host, cb)` from the dns core module.
3. When I visit the shortened URL, it will redirect me to my original link.

### Creation Example:

* POST [project_url]/api/shorturl/new - body (urlencoded) : url=https://www.google.com

### Usage:

* https://fobabs-url-shortener-microservice.glitch.me/BK9ExvC

### Will redirect to:

* https://nodejs.org/en/docs/guides/debugging-getting-started/

### To run this project locally:

1. To begin this project, make sure you have mongodb installed on your local computer. You can follow the instructions by clicking [here](https://docs.mongodb.com/manual/installation/).
  
2. You'll need to clone this repository
```bash
$ git clone https://github.com/fobabs/url-shortener-microservice.git
$ cd url-shortener-microservice
```
3. To install the dependencies used for the project, run
```bash
$ npm install
```
4. If you have the devDependency located in package.json installed globally, you can skip this step, otherwise install it using
```bash
$ npm install --only-dev
```
5. create a .env file and input the following:
```
PORT=4100
DATABASE=mongodb://localhost:27017
```
6. Start up the server
```bash
$ npm start
```
7. If you wish to visualize your database with a GUI, you can download either [NoSQLBooster](https://nosqlbooster.com/downloads) or [MongoDB Compass](https://www.mongodb.com/download-center/compass). There are several other MongoDB GUIs you can use too.

**NOTE**: The server is available at either `http://localhost:4100` OR `http://127.0.0.1:4100` 