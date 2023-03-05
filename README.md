# Galactus

This repo hosts the code for **Galactus**, the centralised backend for Skedulr. Galactus interfaces with all the other micro-services in the Skedulr stack.

The following files are present.

```
.
├── controllers
│   └── user.controller.js
├── db
│   ├── bookings.js
│   ├── organisations.js
│   └── users.js
├── routes
│   └── user.route.js
├── client_secret.json
├── .env.example
├── .gitignore
├── index.js
├── package.json
├── package-lock.json
├── .prettierrc
└── README.md
```

## Running It 🏃

1. Either install mongodb or [setup the mongodb docker container](https://hevodata.com/learn/docker-postgresql/) or set up an Atlas instance.

2. Create a DB by accessing the `mongosh` shell.

3. Replicate the `.env.example` file as `.env`. Edit the environment variables with the DB details and microservice URLs.

4. Then the usual drill. `npm install` and then `npm run dev` to start a dev instance

5. Generate a `client-secret.json` from the Google Cloud console.
