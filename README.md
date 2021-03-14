# MERN

## Client

Folder:

```javascript
├─ client /*Front End React*/
│  ├─ public 
│  │  ├─ assets
│  │  │  └─ img
│  │  │     ├─ home.svg
│  │  ├─ css
│  │  │  ├─ Home.css
│  │  ├─ js
│  │  │  ├─ Homejs
│  │  ├─ index.html
│  │  ├─ manifest.json
│  │  └─ robots.txt
│  ├─ src
│  │  ├─ actions /*Action Redux*/
│  │  │  ├─ authActions.js
│  │  │  └─ types.js
│  │  ├─ assets /*CSS, Image for Components*/
│  │  │  └─ logo.svg
│  │  ├─ components /*Components*/
│  │  │  ├─ App
│  │  │  │  ├─ App.css
│  │  │  │  └─ App.js
│  │  ├─ lib /*Lib*/
│  │  │  └─ bootstrap
│  │  │     ├─ bootstrap.css
│  │  ├─ reducers /*Reducers Redux*/
│  │  │  ├─ authReducer.js
│  │  │  ├─ errorReducer.js
│  │  │  └─ index.js
│  │  ├─ routes /*React Routine*/
│  │  │  ├─ PrivateRoute.js
│  │  │  └─ PublicRoute.js
│  │  ├─ utils
│  │  │  └─ setAuthToken.js
│  │  ├─ App.test.js
│  │  ├─ index.css
│  │  ├─ index.js /*Main react file*/
│  │  ├─ reportWebVitals.js
│  │  ├─ setupTests.js
│  │  └─ store.js
│  ├─ .dockerignore
│  ├─ .eslintcache
│  ├─ .gitignore
│  ├─ Dockerfile /*Docker file => build React image*/
│  ├─ README.md
│  ├─ package-lock.json
│  ├─ package.json
│  └─ yarn.lock
```

Create react:

```bash
npx create-react-app client
```

Start:

```powershell
npm start
```

Build:

```
yarn build
```

connect server nodejs

```json
{
	"...": "...",
  	"proxy": "http://localhost:5000/",
    "...": "...",
}

```

## Server
Folder:

```javascript
├─ server /*Server NodeJS*/
│  ├─ .idea
│  ├─ bin
│  │  └─ www
│  ├─ config
│  │  └─ passport.js
│  ├─ model
│  │  ├─ User.js
│  │  └─ initdb.js
│  ├─ routes
│  │  └─ api
│  │     ├─ admin.js
│  │     ├─ transaction.js
│  │     └─ users.js
│  ├─ test
│  │  └─ users.test.js
│  ├─ utils
│  │  └─ convert.js
│  ├─ validation
│  │  ├─ login.js
│  │  └─ register.js
│  ├─ views
│  │  └─ error.ejs
│  ├─ .ENV
│  ├─ .docker.env
│  ├─ .dockerignore
│  ├─ .gitignore
│  ├─ Dockerfile
│  ├─ app.js
│  ├─ package-lock.json
│  ├─ package.json
│  └─ utils.js
```

port

```javascript
var port = normalizePort(process.env.PORT || "5000");
```

# MERN

Folder:

```javascript
├─ client
├─ server
├─ test
│  └─ example.test.js
├─ .gitignore
├─ README.md
├─ docker-compose-dev.yml
├─ docker-compose-prod.yml
├─ docker-compose.yml
├─ package-lock.json
├─ package.json
└─ yarn.lock
```

start mern

```javascript
npm start
```

Build client:

```powershell
cd client && npm install && npm install --only=dev --no-shrinkwrap && npm run build
```

React build:

```javascript
app.use(express.static("./../client/build"));
```

Run server

```powershell
cd server && npm start
```
