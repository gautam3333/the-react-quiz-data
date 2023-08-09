<p>This repository is about how to create a json server</p>

#### Package
`npm install json-server cors json-serve`

#### Code
```
'use strict';

const jsonServer = require('json-server');
const server = jsonServer.create();
const router = jsonServer.router('questions.json');
const middleware = jsonServer.defaults();
const port = process.env.PORT || 8080;
server.use(middleware);
server.use(router);

server.listen(port);

```
