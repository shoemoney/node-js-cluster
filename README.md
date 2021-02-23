clone<br>
```bash
npm i
node server.js

```
go to: http://localhost:3000/?number=30<br>
[loadtest](https://www.npmjs.com/package/loadtest)<br>
[artillery](npm i artillery)<br>
[artillery eco](https://ecologi.com/artilleryio)<br>
npm install nodemon --save-dev<br>
Add in package.json:<br>

```json
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "nodemon app.js"
}
```

run: npm start<br>
new terminal: sudo npm install -g loadtest<br>
run: loadtest -n 1000 -c 100 --rps 200 http://localhost:3000?number=20<br>
update npm: add "package": "\*" then run $npm update --save<br>
sudo npm install -g artillery<br>
