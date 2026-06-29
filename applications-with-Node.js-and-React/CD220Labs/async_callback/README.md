# async_callback

Explores all three patterns of asynchronous JavaScript programming.

## Files

| File | Description |
|---|---|
| `ExampleAsyncCallBack.js` | Basic callback using `setTimeout` |
| `ExampleAsyncIO.js` | Async file I/O with callbacks |
| `ExampleSyncIO.js` | Synchronous file I/O for comparison |
| `asyncPromise.js` | Creating and consuming Promises |
| `asyncPromiseBookApi.js` | Fetching book API data with Promises |
| `asyncAwaitBookApi.js` | Same API call using async/await |
| `asyncAxiosRequest.js` | HTTP requests with Axios |
| `jsonParse.js` | Parsing JSON from a local file |

## What I Learned

- **Callbacks** — passing a function as a parameter to be called later (`setTimeout`, `fs.readFile`)
- **Promises** — using `new Promise((resolve, reject))`, `.then()`, and `.catch()`
- **Async/Await** — writing cleaner async code with `async` functions and `await`
- Reading files synchronously with `fs.readFileSync`
- Making HTTP requests with `axios`
- Parsing JSON data from files and APIs

## Technologies Used

- Node.js
- Axios

---

**Author:** Ndatimana Assa
