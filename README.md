# Express-Start

```js

// 트리의 형식으로 디렉토리 내용을 나열
$ npm install -g tree-cli

$ tree -l
// C:\Users\noten\...\github\Express-Start\react-backend
├── app.js
├── bin
├── client
├── node_modules
├── package-lock.json
├── package.json
├── public
├── routes
└── views

$ tree -I node modules
// C:\Users\noten\...\github\Express-Start\react-backend
├── app.js
├── bin
├── client
├── node_modules
├── package-lock.json
├── package.json
├── public
├── routes
└── views

directory: 6 file: 3


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

마지막으로 React App project에서 proxy를 설정합니다. 
client 폴더에는 package.json 파일이 있는데, 파일에는 사용하는 react, react-dom 등에 대한 dependency가 정의되어 있고, 프로그램이 실행될때 사용되는 script도 정의되어 있습니다. 그러면 scripts 아래에 proxy라는 item을 아래와 같이 추가해줍니다.

proxy를 추가함으로써 React App은 실제 3000번 port에서 작동중임에도 불구하고 호출은 Express backend가 존재하는 3001번 port로 호출하게 됩니다. 이렇게 하는 이유는 cross-origin-resource-sharing 문제를 피하기 위함입니다. CORS는 나중에 다시 포스팅하도록 하겠습니다.

```

# errors

./src/App.js
  Line 2:  'logo' is defined but never used  no-unused-vars
  2 행 : '로고'가 정의되었지만 결코 사용되지 않은 행을 사용하지 않았습니다.

Search for the keywords to learn more about each warning.
각 경고에 대해 자세히 알아 보려면 키워드를 검색하십시오.

To ignore, add // eslint-disable-next-line to the line before.
무시하려면 이전에 줄에 // eslint-disable-next-line을 추가하십시오.