# A Copy and edit for an MVC Generator using VYNL as base

## What's Inside
Using this repository: https://github.com/kenaszogara/vynl as a base , I am changing few things to make it my tools library, don't use it 

Use: https://www.npmjs.com/package/vynl

## Initialize Project

$ npm install -g bentomvc

```
In the blank directory
$ bentomvc init
```

Our project directory after

```
.
|--auth
|    └──auth.js
|--config
|    └──config.json
|--docs
|    |--paths
|    |    |--index.js
|    |    └──users.js
|    └──schemas
|         |--index.js
|         └──users.js
|--migrations
|--models
|--routes
|--app.js
└──swagger.js

```
$ bentomvc generate:api -m <model_name> -f <fields>
```

### generate:model

```
$ bentomvc generate:model -m <model_name> -f <fields>
```

### generate:controller

required: model_name

```
$ bentomvc generate:controller -m <model_name>
```

### generate:route

required: route_name

```
$ bentomvc generate:route -r <route_name>
```

### generate:swagger

required: model_name, fields

```
$ bentomvc generate:swagger -m <model_name> -f <fields>
```

## Manual

```
BENTO-MVC CLI

bentomvc [command]

Commands:
  bentomvc init                             Initializes project
  bentomvc generate:api                     Generates Model/Migration/Controller/Route/SwaggerDoc
  bentomvc generate:model                   Generates Model/Migration
  bentomvc generate:controller              Generates Controllers
  bentomvc generate:route                   Generates Routes
  bentomvc generate:swagger                 Generates Swagger Documentation

Options:
  --help      Show help
```
