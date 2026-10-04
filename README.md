# COMP3123 Lab 4

Mechel Fernando — 101352126

An Express application with query, path, and JSON body parameters.

## Run

```bash
npm install
npm run dev
```

The server runs at http://localhost:3000. Use `npm start` to run without nodemon.

## Requests

| Method | URL | Result |
| --- | --- | --- |
| GET | /hello | Hello Express JS |
| GET | /user | Default user: Pritesh Patel |
| GET | /user?firstname=John&lastname=Doe | John Doe |
| POST | /user/John/Doe | John Doe |
| POST | /users | Returns the JSON array sent in the body |
| GET | /instruction.html | Serves the provided instructions |

For POST /users, select Body → raw → JSON in Postman and send:

```json
[
  { "firstname": "Pritesh", "lastname": "Patel" },
  { "firstname": "John", "lastname": "Doe" },
  { "firstname": "John", "lastname": "Rome" }
]
```

Import `COMP3123-exec04.postman_collection.json` into Postman to load all six requests. Start the server first, send each request, and capture screenshots showing the method, URL, status, and response. Save the screenshots in a `screenshots` folder before pushing to GitHub and making the final submission ZIP.
