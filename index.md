# ishh.js
The simplest http server creator for beginners on node.js!


### Install
`npm i ishh.js  |   yarn add ishh.js`

### Example
```js
const { Server } = require("ishh.js")
const f = new Server({
  port: 3000 // Your port here
})
    f.start() // Start the server

f.homepage(process.cwd()+'/index.html') // Homepage to send on path:  /

f.send({
 path: "/shit",
  file: process.cwd()+'/shit.html'
       }) // this will send file shit.html to path:  /shit

f.unfoundPage(process.cwd()+'/404.html') // 404 page setup to send on unfound pages
```
