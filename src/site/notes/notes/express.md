---
{"dg-publish":true,"permalink":"/notes/express/","dgHomeLink":true,"dgPassFrontmatter":false,"dgShowBacklinks":true,"dgShowLocalGraph":true}
---

# ExpressJS

"Hello World" with ExpressJS:
```js
const express = require('express');
const server = express();

server.get('/', (request, response) => {
  return response.json({ message: 'Hello World!' });
});

server.listen(3000)
```
