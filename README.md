clone and run<br>
```bash
npm i
node server.js

```
check, browse to<br>
[http://localhost:3000/?number=30](http://localhost:3000/?number=30)<br>
<br>
install loadtest, artillery and nodemon<br>
[loadtest](https://www.npmjs.com/package/loadtest)<br>
[artillery](https://www.npmjs.com/package/artillery)<br>
[artillery eco](https://ecologi.com/artilleryio)<br>

```bash
npm install nodemon --save-dev
```
add in package.json<br>

```json
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "start": "nodemon app.js"
}
```

run the scripts with
```bash
npm start
```

new terminal, get a report
```bash
sudo npm install -g loadtest
loadtest -n 1000 -c 100 --rps 200 http://localhost:3000?number=20
```

new terminal, install artillery
```bash
sudo npm install -g artillery
```
run the artillery test, get a load test report.<br>

How to update npm<br>
add
```bash
"package": "\*" to package.json
```
run 
```bash
npm update --save
```
