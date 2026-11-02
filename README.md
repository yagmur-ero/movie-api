# Movie API

A simple REST API built with Node.js and Express as a Backend Development course exercise. Movies are kept in memory, so they reset when the server restarts.

## Run

```
npm install
node app.js
```

The server runs at `http://localhost:3000`.

## Endpoints

| Method | Path          | Description        | Status codes |
|--------|---------------|--------------------|--------------|
| GET    | `/movies`     | Get all movies     | 200          |
| GET    | `/movies/:id` | Get a movie by id  | 200, 404     |
| POST   | `/movies`     | Add a new movie    | 201, 400     |

POST body example:

```json
{ "title": "Blade Runner", "director": "Ridley Scott", "year": 1982 }
```

## Testing

Requests are in `requests.http` (VS Code REST Client). They were also tested with Postman.
