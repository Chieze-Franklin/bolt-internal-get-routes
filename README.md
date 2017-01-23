# bolt-internal-get-routes

Internal Bolt module used to get all the routes exposed by the Bolt server.

## Installation

```sh
$ npm install bolt-internal-get-routes
```

## Use

```js
var express = require('express');
var getRoutes  = require('bolt-internal-get-routes')

var app = express();
var summary = getRoutes.summary(app);
console.log(summary.paths);
console.log(summary.routes);
console.log(summary.lines);
```

### Note

This is an internal module and should not be used in 3rd party apps.