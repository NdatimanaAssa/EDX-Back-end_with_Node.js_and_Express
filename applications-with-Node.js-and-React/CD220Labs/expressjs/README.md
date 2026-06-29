# expressjs

Multiple Express.js servers covering all core backend concepts from routing to authentication.

## Files

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

## What I Learned

- Setting up an Express server and defining routes
- Route parameters (`req.params`) and query strings (`req.query`)
- Middleware pipeline and `next()`
- App-level vs router-level vs custom middleware
- Error handling middleware
- Serving static assets with `express.static()`
- JWT (`jsonwebtoken`) for token-based authentication
- Sessions with `express-session`
- User registration and login flow

## Technologies Used

- Node.js
- Express.js
- jsonwebtoken
- express-session

---

**Author:** Ndatimana Assa
