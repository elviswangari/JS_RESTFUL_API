# BUILDING RESTFUL API USING NODE EXPRESS MONGO

we'll be using the latest javascript and to do so we install babel inorder to convert ES6 TO ES5

```
npm i --save-dev @babel/core @babel/cli @babel/node @babel/preset-env
```

also nodemon and body-parser to parse our code

```
npm i nodemon body-parser
```

next is to set up babelrc

```
{
  "presets": ["@babel/preset-env"]
}
```

next we create a script where we start nodemon on our script inside package.json

some test code 
```
import express from 'express';

const app = express();
const port = 5000;

app.get('/', (req, res) =>
  res.send(`Node and express server runningon port ${port}`)
);

app.listen(port, () =>
  console.log(`your server is running on port ${port}`)
);
```

to run our server we use
```
npm start
```

next is to set up our directory structure

