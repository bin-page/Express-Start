# Express-Start

```js

$ npm install express-generator -g

$ express react-backend

$ cd react-backend

$ npm i

// bin/www
var port = normalizePort(process.env.PORT || '3333');


$ npm install -g create-react-app

$ create-react-app client

Installing packages. This might take a couple of minutes.
Installing react, react-dom, and react-scripts...

+ react@16.8.6
+ react-scripts@2.1.8
+ react-dom@16.8.6
added 1842 packages from 718 contributors and audited 36240 packages in 67.239s
found 63 low severity vulnerabilities
  run `npm audit fix` to fix them, or `npm audit` for details

Success! Created client at C:\Users\noten\OneDrive\바탕 화면\github\Express-Start\react-backend\client
Inside that directory, you can run several commands:

  npm start
    Starts the development server.

  npm run build
    Bundles the app into static files for production.

  npm test
    Starts the test runner.

  npm run eject
    Removes this tool and copies build dependencies, configuration files
    and scripts into the app directory. If you do this, you can’t go back!

We suggest that you begin by typing:

  cd client
  npm start

Happy hacking!


// client/package.json 
{
  "proxy": "http://localhost:3333"
}

```