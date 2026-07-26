# Node.js Backend Arsenal 🚀

Welcome to the **Node.js Backend Arsenal**, the ultimate high-velocity snippet collection engineered for production-grade Node.js development.

If you are tired of typing the exact same boilerplate code for Express controllers, Mongoose schemas, JWT middleware, and AWS SDK commands, this extension is your cheat code.

This toolkit completely eliminates boilerplate by providing over **170+ highly optimized, opinionated snippets** covering everything from basic routing to complex Node.js system architecture.

---

## 🔥 Features
- **Massive Ecosystem Coverage**: Includes advanced boilerplates for **Express, Mongoose, JWT, Bcrypt, AWS S3, Redis, Socket.io, Axios, Jest**, and native Node modules (`path`, `fs`, `os`, `crypto`, `cluster`, `child_process`).
- **Built for Pure Speed**: Drop in an entire authentication middleware, an S3 upload function, or a multi-core cluster scaling block in exactly three keystrokes.
- **Opinionated & Secure**: All snippets default to modern async/await syntax, standard error forwarding (`next(error)`), and strict HTTP status codes.

---

## ⚡ Sneak Peek: The Prefix Arsenal

### Core Express & Control Flow
- `expressapp` - Complete `server.js` scaffold with CORS and JSON parsing.
- `ec` / `mw` - Async Controller & Middleware boilerplates with built-in try/catch.
- `route`, `rget`, `rpost`, `rid` - Instant REST route scaffolding.
- `ratelimit`, `cookieparser`, `multer` - Scale your app with security and upload middlewares.

### Database (Mongoose)
- `mconn`, `mschema` - Establish connections and scaffold rich models instantly.
- `mfind`, `mfid`, `mupsert`, `minsert` - Instantly drop in standard or advanced database queries.
- `mtrans` - Scaffold an entire atomic transaction block (`session.startTransaction()`).

### Real-Time & External APIs
- `ioinit`, `ioon`, `ioemit` - Scaffold a Socket.io server and listeners on top of Express.
- `axiosg`, `axiosp`, `fetchj` - Rapidly drop in HTTP clients for external microservices.

### Auth, Crypto & Caching
- `bhash`, `bcomp` - Password hashing and validation.
- `jwtsign`, `jwtverify` - Sign tokens and scaffold complete Bearer token guard middlewares.
- `redisconn`, `redisget`, `redsetex` - Setup robust caching layers via `ioredis`.

### Advanced Node Built-ins
- `cluster` - Multi-core horizontal scaling boilerplate.
- `cpexec`, `cpspawn` - Execute shell scripts via `child_process`.
- `streamread`, `streampipe` - High-performance data streaming operations.

---

## 🛠️ Usage
Simply type the prefix in any `.js` or `.ts` file and hit `Tab` or `Enter` to instantly scaffold the code block. Use `Tab` to rapidly navigate through the variable placeholders within the generated code.

Stop typing boilerplate. Start shipping.

---
**Author**: Viswaranjan  
**License**: MIT
