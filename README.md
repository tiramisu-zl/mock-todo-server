# Todo mock server

This mock server is built by [json-server](https://github.com/typicode/json-server). All the mocked data are put in file `db.json`. 

## Start mock server

Please clone or download this project to your local, and use `npm` or `yarn` to install the dependences and start server:

```
npm install
npm start
```

Or

```
yarn install
yarn start
```

Then you can access `http://localhost:3001/todos/` to see if the server is started correctly.

## APIs

You can refer the document of [json-server](https://github.com/typicode/json-server) to see the full APIs. 

Also here are some APIs you might want to use:

### Get todo list

```
GET http://localhost:3001/todos
```

The response of this request would be the json of all todos list.

### Get one todo

```
GET http://localhost:3001/todos/{id}
```

The response of this request would be the json of the todo item which match the id.

### Change one todo

```
PUT http://localhost:3001/todos/{id}
{
    "headers": {
        "Content-Type": "application/json"
    },
    "body": {MODIFIED AGENT}
}
```

Then the todo item which match which the id will be updated and be replaced with the modified todo item. 

The response of this request would be the json of the modified todo.