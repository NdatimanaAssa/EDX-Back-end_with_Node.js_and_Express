# Back-end Development with Node.js and Express

## Course Overview
This repository contains all the labs and projects completed during the **Back-end Application Development with Node.js and Express** course on EDX. The course covers building server-side applications using Node.js, Express.js, and integrating with React on the front end.

---

## Repository Structure

```
EDX-Back-end_with_Node.js_and_Express/
├── applications-with-Node.js-and-React/
│   └── CD220Labs/
│       ├── http_server/        ← Building HTTP servers with Node.js
│       ├── async_callback/     ← Async programming: callbacks, promises, async/await
│       ├── expressjs/          ← Express.js server, routing, middleware, authentication
│       ├── react_pages/        ← First React page using CDN
│       ├── react-apps/         ← React app created with Create React App
│       ├── react_class_component/ ← React class components and functional components
│       ├── props_and_states/   ← React props and state management
│       └── todoapp/            ← Todo app built with React
└── mxpfu-nodejsLabs/
    └── routes/
        └── users.js            ← REST API with Express: GET, POST, PUT, DELETE
```

---

## Projects & What I Learned

### 1. `http_server`
Built a raw HTTP server using Node.js built-in `http` module without any framework.

- Creating an HTTP server with `http.createServer()`
- Using `require()` to import custom modules
- Returning time-based greetings using `getHours()`
- Understanding the difference between returning a string vs a Date object
- Listening on a port with `server.listen()`

---

### 2. `async_callback`
Explored all three patterns of asynchronous JavaScript programming.

- **Callbacks** — passing a function as a parameter to be called later (`setTimeout`, `fs.readFile`)
- **Promises** — using `new Promise((resolve, reject))`, `.then()`, and `.catch()` to handle async results
- **Async/Await** — using `async` functions and `await` to write cleaner async code
- Reading files with `fs.readFileSync`
- Making HTTP requests with `axios`
- Parsing JSON data from files and APIs

---

### 3. `expressjs`
Built multiple Express.js servers covering all core concepts.

| File | What it covers |
|---|---|
| `expressServer.js` | Basic Express server with GET and POST routes |
| `expressRouting.js` | Express Router with separate routers for users and items |
| `expressAppLevelMiddleware.js` | Applying middleware at the application level |
| `expressRouterMiddleware.js` | Applying middleware at the router level |
| `expressUserDefinedMiddleware.js` | Writing custom middleware functions |
| `expressErrorHandling.js` | Handling errors in Express |
| `expressErrorRoutingAppLevel.js` | Error handling at route and app level |
| `expressStaticPages.js` | Serving static files with `express.static()` |
| `expressTemplate.js` | Using template engines to render views |
| `expressWithAuthentication.js` | JWT authentication and session management |

Key concepts learned:
- Setting up an Express server and defining routes
- Route parameters (`req.params`) and query strings
- Middleware pipeline and `next()`
- JWT (`jsonwebtoken`) for token-based authentication
- Sessions with `express-session`
- User registration and login flow

---

### 4. `react_pages`
- Writing a React component directly in an HTML file using CDN links
- Understanding how React renders to the DOM without a build tool

---

### 5. `react-apps`
- Scaffolding a React project using Create React App
- Understanding the project structure (`public/`, `src/`)
- Running and building a React app

---

### 6. `react_class_component`
- Writing React components as ES6 classes
- Difference between class components and functional components
- Using `render()` method to return JSX

---

### 7. `props_and_states`
- Passing data to components using **props**
- Managing dynamic data inside components using **state**
- Updating the UI when state changes

---

### 8. `todoapp`
- Building a complete todo application with React
- Managing a list of items in state
- Adding and removing items dynamically

---

### 9. `mxpfu-nodejsLabs`
Built a REST API with Express.js to manage a list of users.

- **GET** `/users` — Retrieve all users
- **GET** `/users/:email` — Retrieve a single user by email
- **POST** `/users` — Add a new user via query params
- **PUT** `/users/:email` — Update any user attribute (`firstName`, `lastName`, `email`, `DOB`)
- **DELETE** `/users/:email` — Delete a user by email

Key concepts learned:
- Express Router (`express.Router()`)
- Route parameters (`req.params`) and query strings (`req.query`)
- Filtering and mutating in-memory arrays as a data store
- Partial updates — only modifying fields that are provided in the request

---

## Technologies Used
- Node.js
- Express.js
- JWT (jsonwebtoken)
- express-session
- Axios
- React (Create React App)
- JavaScript (ES6+)

---

**Author:** Ndatimana Assa
