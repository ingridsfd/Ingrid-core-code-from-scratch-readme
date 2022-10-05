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

These are the results:

API Code construction:

![image](https://user-images.githubusercontent.com/98929413/193965823-59955e6a-5493-4808-a498-4ca5b98168e6.png)

Terminal confirming API correct installation:

![image](https://user-images.githubusercontent.com/98929413/193966151-8d50beb7-9325-4cf6-896c-a07a872c7a70.png)

For ping:

![image](https://user-images.githubusercontent.com/98929413/193965641-cc3ca3b2-a555-480d-9d91-edc0d6e10989.png)

For pong:

![image](https://user-images.githubusercontent.com/98929413/193965720-47b1b99a-8094-4a9a-93c3-5b1835b1747c.png)


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
