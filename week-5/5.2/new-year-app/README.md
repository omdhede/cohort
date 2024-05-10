## Todo App

This project contains a simple TODO application
It has the following features -

- Anyone can create a todo
- Anyone can see their existing todos
- Anyone can mark todo as done

// Initialize a  node project
// put a package.json

## backend using express
```javascript
// write basic express boilerplate code
// with express.json() middleware

const express = require("express")
const app = express()

app.use(express.json())

app.post("/todo", function(req, res) {

})

app.get('/todos', function(req, res) {

})

app.put("/completed", function(req, res) {
    
})
```

### Create a `types.js` file and use `zod` library
```text
npm install zod
```