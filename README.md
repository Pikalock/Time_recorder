# How to install the tool in your pc


## how to use the Time_recorder

add your events in the input box,then click`start`,it will record your time spent on the events.
It's easy to open `index.html` in a browse , and if you want to use it as a desktop app , please follow ⬇️

### 1.make sure you have installed node.js

after installed node.js,initate your program:
`npm init your-project-name
`

then use npm to install electron:
`npm install electron`
### 2. create a new file `main.js` and start the app in this file.
then edit it like:

`const { app, BrowserWindow } = require('electron');

function createWindow() {
    const win = new BrowserWindow({
        width: 800,
        height: 600,
        webPreferences: {
            nodeIntegration: true
        }
    });
    win.loadFile('index.html');
}

app.whenReady().then(createWindow);`


### 3. run your program
* add commands in `package.json`:

`"scripts": {
    "start": "electron ."
}`

* `npm start`


### 4. the problems you may meet:
1. errors happen when you install electron
`npm cache clean --force
`
`rm -rf node_modules
`
`npm install electron --save-dev
`
`npm start
`
2. still fail to download

`npm install -g nrm
`
`nrm ls
`this command will list the source you can choose to use[usage:`nrm use npm
`]

example:
`npm ---------- https://registry.npmjs.org/
yarn --------- https://registry.yarnpkg.com/
tencent ------ https://mirrors.cloud.tencent.com/npm/
cnpm --------- https://r.cnpmjs.org/
taobao ------- https://registry.npmmirror.com/
npmMirror ---- https://skimdb.npmjs.com/registry/`

`nrm use tencent
`

### after you change the origin source,download it again.

If you still got problems with the download or the app, contact with `pikalock2024@gmail.com`✨✨✨





