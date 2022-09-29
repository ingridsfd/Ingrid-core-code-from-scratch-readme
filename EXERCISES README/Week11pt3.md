# Week challenges (Thursday) 💻

## Forrest Gump Ping-Pong API 🏓

Use Express JS to build the API.

Use any port you want for the API.

The API has to be able to respond to the "ping" request with the "pong" message.

Use /api/buba-gump as the root route for the API.

Make sure your API responds to the request using JSON e.g.:
{
"message": "pong"
}
Use Postman to test your API.

Optional but desirable, make your API capable of responding to any player move:

If the user makes the "ping" move, your API should respond with "pong".

If the user makes the "pong" move, your API should respond with "ping".

Do you feel stuck?

## Delayed Response API ⏳

Create a simple REST API that receives a request containing a number that represents a delay in milliseconds. The API should respond to the request after the delay specified in the request has expired.

API Requeriments:
Use Express JS to build the API.

Use any port you want for the API.

The API should use route parameters to get the desired delay:

- Request example
- Here 3000 indicates a delay of 3000 milliseconds
  http://localhost:3000/api/delay/3000
  Your API should have just one request handler.

You can send any response you want after the delay has expired.

If no delay is provided in the request, the API should use 1000 as default.
