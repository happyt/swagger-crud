## Skeleton project for Swagger

[https://github.com/swagger-api/swagger-node](https://github.com/swagger-api/swagger-node)

Added CRUD interface using [https://scotch.io/tutorials/speed-up-your-restful-api-development-in-node-js-with-swagger](https://scotch.io/tutorials/speed-up-your-restful-api-development-in-node-js-with-swagger)

Added CRUD back end stems to give a simple CRUD test, without permanent storage. Needs db.

### To start server in mocking mode
swagger project start hello-world -m

### To start server in server mode (will restart on changes)
swagger project start hello-world

### To change/edit the yaml interface (separate window)
swagger project edit

### To see the docs interface
Add the dist folder from swagger-ui, changed the url ref inside, to swagger.yaml, browse to url:port/docs


### Installation
npm install -g swagger


### Directory structure
```
swagger project create the-collection

-- api  
---- controllers
---- dist           -- swagger-ui interface
------ hello_world.js - main code interface
---- helpers
---- mocks
---- swagger
------ swagger.yaml

— config
—— db.js            -- database functions, currently in-memory array
---- default.yaml

-- test
---- api
------ controllers
-------- hello_world.js
------ helpers

-- app.js
-- package.json
```

