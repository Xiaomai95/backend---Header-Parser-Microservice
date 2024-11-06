# Request Header Parser Microservice

This project is a very simple Header Parser Microservice that parses the headers requested from the client, built using the Express framework. Once the request is complete, the API responds with a JSON object containing the user's IP address, language, and software. 

## Key Features:

- API Endpoint: GET /api/:whoami? : parses a ==:whoami== object which is then used to request ==headers== from the client.

- Error Handling: if GET request fails a JSON object with an error message is sent in respone.

## Example Resposes:
`/api/whoami` => `{"ipaddress":"::ffff:159.20.14.100","language":"en-US,en;q=0.5",
"software":"Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:50.0) Gecko/20100101 Firefox/50.0"}`

`/api` => `{"error":"Handler request failed"}`

## Installation & Usage

    Clone the repository.
    Run npm install to install dependencies.
    Start the server with npm start or node index.js.
    Access the API locally at http://localhost:3000/api or on the port specified in process.env.PORT.


