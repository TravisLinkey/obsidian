
2024-09-01 21:40

# Table of Contents
- [Overview](#overview)
- [Code](#code)
- [Scripts](#scripts)

### Overview
Use these commands to setup a node server

- **Create npm project**
`mkdir project && cd project && npm init -y`

- **Install express and dependencies**
`npm i express dotenv`

- **Install typescript dependencies**
`npm i -D typescript @types/express @types/node`

### Code
```javascript
import express from 'express';
import dotenv from 'dotenv';

dotenv.config();

const app = express();
const port = process.env.PORT;

app.get('/', (req, res) => {
  res.send('Express + TypeScript Server');
});

app.listen(port, () => {
  console.log(`[server]: Server is running at http://localhost:${port}`);
});
```

### Scripts 
```json
{
    "scripts": {
        "build": "npx tsc",
        "start": "node dist/index.js",
        "dev": "nodemon src/index.ts"
      },
    "compilerOptions": {
        ...
        "outDir": "./dist"
        ...
      }
}
```

### References
- [[Node]]

