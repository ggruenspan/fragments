# Fragments

The project was developed utilizing Node.js and the Express module, which is hosted on Amazon Web Services and is complemented by the use of AWS Cognito, DynamoDB, S3 and Docker.

# To Run

`npm i`- installs necessary dependencies for running locally

`npm start` - to start running the server at `node src/index.js`

Server should start successfully on `localhost:8080` with an health check and a logger message should show `Server started` and `Cognito JWKS cached`.

# To Test

`npm run dev ` - run the server in development mode

`npm run debug ` - runs the server in debug mode

`nodemon` is configured and will keep monitorning for code changes and restarting the server.

# Docker image

You can either find the dockerized image here: [gerredg/fragments](https://hub.docker.com/r/gerredg/fragments/tags)

OR simply run

`docker pull gerredg/fragments:latest`

#### Valid Fragment Conversions

List of valid conversions:

| Type               | Valid Conversion Extensions    |
| ------------------ | ------------------------------ |
| `text/plain`       | `.txt`                         |
| `text/markdown`    | `.md`, `.html`, `.txt`         |
| `text/html`        | `.html`, `.txt`                |
| `application/json` | `.json`, `.txt`                |
| `image/png`        | `.png`, `.jpg`, `.webp`, `gif` |
| `image/jpeg`       | `.png`, `.jpg`, `.webp`, `gif` |
| `image/webp`       | `.png`, `.jpg`, `.webp`, `gif` |
| `image/gif`        | `.png`, `.jpg`, `.webp`, `gif` |
