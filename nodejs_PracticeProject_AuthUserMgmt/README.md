# nodejs_PracticeProject_AuthUserMgmt

A full authentication and user management REST API built with Express.js, JWT, and sessions. Users must register and log in before accessing the protected friends endpoints.

## Project Structure

```
nodejs_PracticeProject_AuthUserMgmt/
├── index.js          ← App entry point: auth routes + session/JWT middleware
└── router/
    └── friends.js    ← Protected CRUD routes for friends
```

## Running the Project

```bash
npm install
npm start
# Server runs on http://localhost:5000
```

## API Endpoints

### Public

| Method | Endpoint | Description |
|---|---|---|
| POST | `/register` | Register a new user with username and password |
| POST | `/login` | Login and receive a JWT stored in session |

### Protected (requires login)

| Method | Endpoint | Description |
|---|---|---|
| GET | `/friends` | Retrieve all friends |
| GET | `/friends/:email` | Retrieve a single friend by email |
| POST | `/friends` | Add a new friend |
| PUT | `/friends/:email` | Update a friend's `firstName`, `lastName`, or `DOB` |
| DELETE | `/friends/:email` | Delete a friend by email |

## Authentication Flow

1. `POST /register` — creates a user (rejects duplicates)
2. `POST /login` — validates credentials, signs a JWT, stores it in the session
3. All `/friends` requests pass through middleware that reads `req.session.authorization`, verifies the JWT with `jwt.verify()`, and either calls `next()` or returns `403`

## What I Learned

- User registration with duplicate check using `Array.filter()`
- JWT generation with `jwt.sign()` and verification with `jwt.verify()`
- Session management with `express-session` to persist the access token across requests
- Protecting routes with custom auth middleware using `req.session.authorization`
- Combining `express.Router()` with app-level middleware for clean route separation

## Technologies Used

- Node.js
- Express.js
- jsonwebtoken
- express-session

---

**Author:** Ndatimana Assa
