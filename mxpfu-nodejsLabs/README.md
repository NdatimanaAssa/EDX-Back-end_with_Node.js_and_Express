# mxpfu-nodejsLabs

A REST API built with Express.js to manage a list of users stored in-memory.

## Project Structure

```
mxpfu-nodejsLabs/
├── index.js          ← Express app entry point
└── routes/
    └── users.js      ← User CRUD routes
```

## Running the Project

```bash
npm install
npm start
# Server runs on http://localhost:5000
```

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/user` | Retrieve all users |
| GET | `/user/:email` | Retrieve a single user by email |
| POST | `/user` | Add a new user via query params |
| PUT | `/user/:email` | Update a user's fields by email |
| DELETE | `/user/:email` | Delete a user by email |

## What I Learned

- Setting up an Express server and mounting a router with `app.use()`
- Using `express.Router()` to separate route logic
- Route parameters with `req.params` and query strings with `req.query`
- Filtering and mutating an in-memory array as a data store
- Partial updates — only modifying fields that are provided in the request

## Technologies Used

- Node.js
- Express.js

---

**Author:** Ndatimana Assa
