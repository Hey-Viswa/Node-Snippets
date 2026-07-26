# Node.js Backend Arsenal - Documentation

This document explains exactly what each snippet does and the boilerplate code it generates.

## 🚀 Core Console & Debugging
- `clg`: `console.log()`
- `clv`: Logs a variable with its name for debugging (`console.log('var:', var)`)
- `cle`: `console.error()`
- `clw`: `console.warn()`
- `clt`: `console.table()`

## ⚡ Control Flow & Async
- `tryc`: Standard async `try/catch` block that forwards errors via `next(error)`
- `ife`: Standard `if/else` block
- `prom`: Creates a `new Promise((resolve, reject) => { ... })`
- `iife`: Creates an async Immediately Invoked Function Expression `(async () => { ... })()`
- `sleep`: Creates a promise-based sleep function `await sleep(ms)`

## 📦 Modules (CommonJS & ES6)
- `req`: `const module = require('module');`
- `mexp`: `module.exports = { ... };`
- `imp`: `import module from 'module';`
- `expd` / `exp`: `export default ...` / `export const ...`

## 🌐 Express Framework Setup
- `expressapp`: Scaffolds a complete `server.js` file with CORS, JSON parsing, and `app.listen()`
- `erouter`: Scaffolds a complete Express `router` file
- `corssetup`: `app.use(cors({ origin: process.env.CLIENT_URL, credentials: true }));`
- `helmetsetup`: `app.use(helmet());`
- `bodyparser`: Configures Express to parse JSON and URL-encoded bodies.
- `staticdir`: Sets up a public static directory.

## 🛤️ Express Routes & Controllers
- `route`: Standard Express route shell (`router.get`, `router.post`, etc.)
- `rget`, `rpost`, `rput`, `rpatch`, `rdel`: Specific REST method route shells.
- `rid`: Scaffolds an Express route with an `:id` parameter + a built-in Mongoose 404 check.
- `rparam`: Scaffolds a `router.param()` middleware block.
- `ec`: Async Express controller function scaffold.
- `mw`: Async Express middleware function scaffold with `next()`.
- `errhandler`: Global Express error handler `(err, req, res, next)`.

## ❌ HTTP Responses
- `s200`, `s201`, `s204`: Fast success JSON responses (OK, Created, No Content).
- `e400`, `e401`, `e403`, `e404`, `e409`, `e422`, `e500`: Standard error JSON responses.

## 🗄️ Database (Mongoose)
- `mconn`: Robust `connectDB` function to establish MongoDB connection.
- `mschema` / `mmodel`: Mongoose schema and model export block.
- `mfind`, `mfindone`, `mfid`: Database read queries (`find`, `findOne`, `findById`).
- `mcreate`, `msave`, `mupd`, `mdel`: Database write and mutate queries.
- `mpop`, `mcount`, `magg`: Advanced queries (Populate, Count Documents, Aggregate pipelines).
- `mvirt`, `mindex`, `mpre`, `mpost`: Schema virtuals, indexes, and middleware hooks.
- `m404`: Drops in an early return 404 guard `if (!doc) return res.status(404)...`

## 🔒 Security, Crypto & Auth
- `bhash` / `bcomp`: Bcrypt hash and compare passwords.
- `jwtsign` / `jwtverify`: Sign JWTs and fully guard routes with Bearer token authentication middleware.
- `randhex`: Generates a random secure hex string using `crypto.randomBytes`.
- `uuidv4`: Generates a UUID v4.

## 📁 Modern File System (fs/promises)
- `fsread`, `fswrite`, `fsapp`: Read, write, and append files asynchronously.
- `fsunlink`, `fsmkdir`, `fsstat`, `fsdir`: Delete files, make directories, check stats, and read directory contents.

## 🧪 Testing Suite (Jest & Supertest)
- `desc`, `it`: Jest `describe` and `it` blocks.
- `beforea`, `beforee`, `aftera`, `aftere`: Jest setup and teardown blocks.
- `exp`, `exprej`: Jest `expect` and `expect.rejects` assertions.
- `stget`, `stpost`, `stput`, `stdel`: Supertest request testing blocks.

## ⚡ Redis Caching (ioredis)
- `redisconn`: `ioredis` connection block.
- `redisget`, `redisset`, `redsetex`: Cache fetching and setting (with EX expiry).
- `reddel`, `redflush`: Clear specific keys or flush the entire Redis database.

## ☁️ AWS S3 (v3 SDK)
- `s3init`: `S3Client` instantiation boilerplate.
- `s3up`, `s3down`, `s3del`: AWS SDK V3 commands (`PutObject`, `GetObject`, `DeleteObject`).
- `s3url`: Generates a presigned URL.

## 💻 Native Node.js Built-ins
- `pathjoin`, `pathres`, `pathbase`, `pathext`: Extracts and formats file paths.
- `eventset`, `eventon`, `eventemit`: Scaffold `EventEmitter` classes and listeners.
- `osinfo`, `osplat`: Extract CPU, memory, and platform information.
- `cpexec`, `cpspawn`: Execute shell scripts or spawn child processes.
- `cluster`: Massive multi-core scaling boilerplate using `cluster.fork()`.
- `streamread`, `streamwrite`, `streampipe`: High-performance streams and data pipelines.
- `cryptohash`: SHA-256 hashing.
- `utilprom`, `utilinsp`: Promisify callbacks and deep-inspect objects.
- `urlparse`: Extract search parameters from query strings.
