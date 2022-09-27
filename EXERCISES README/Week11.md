# Week Challenges (Monday) 💻
Time to catch up ⏱️ or play with the React project
# Week Challenges (Tuesday) 🐣
## Node.JS Core Understanding Learning Exercise 🧠

**1. What is Node.JS?** Node is a runtime environment that allows JavaScript to track where functions are called considering that the stack only excecutes one functiona at a time.

**2. What problem does Node.JS solve?**
[Looking for personal opinions](https://www.quora.com/What-is-Node-js-really-trying-to-solve-Is-there-a-technology-mature-enough-to-choose-as-an-alternative-for-Node-js), we encounter Node.JS mainly solves allowing to use a collection of JS libraries. Allows to use ECMAScript. There are no vendor controlling the server-side options.

**3. What is the V8 Javascript Engine?**

**4. Is Node.JS really necessary in the Development ecosystem?**

**5. What is the difference between Node.JS and any other browser?**

**6. What is NVM and Why is it useful for Node.JS developers?**

## Node.JS Module System Core Understanding Learning Exercise 🧠

**1. What is a Javascript Module?**

**2. Why are Javascript Modules necessary?**

**3. What module standards are available in Node.JS?**

**4. What are the differences between ESModules and CommonJS modules?**

**5. Which types of modules exist in Node.JS?**

## Node.JS Module System Practice 💻

Time to put into practice what you learned about Node.JS modules 😁.

Create a new Node.JS project, name it: <your-nickname>/modules
  
Create a new module, name it: operations.js
  
Inside operations.js implement two functions, one for the sum operation and one for the subtract operation.
  
Create a new module, name it: main.js
  
Import the functions implemented in operations.js and use them in any way in main.js.

## Client-Server Model Learning Exercise 🧠

**1. What is a Server?**
  
**2. What is a Client?**
  
**3. Is a server just another physical computer?**
  
**4. Why do we refer to a certain class of applications as Servers?**
  
**5. What is the difference?**
  
**6. Is there any similarity between human communication and the client-server model?**
  
**7. Is the client-server model applicable only to the Web?**
  
**8. Can you mention any other example of this model outside the Web?**
  
# Week Challenges (Wednesday) 🐤

## APIs Core Understanding Learning Exercise 🧠

**1. What is an API?**
  
**2. What is a Protocol?**
  
**3. Is the term API only applicable to the communication of programs over the Internet?**
  
**4. Why is structured communication between two programs important?**
  
**6. Do we humans use APIs when communicating without technology?**
  
**7. Is an API just another program or a standard?**
  
**8. Do you know any API? Can you list at least 5 examples of APIs?**

## From JSON to REST Learning Exercise 🧠

**1. What is HTTP?**
  
**2. What is JSON?**
  
**3. Is JSON the same as a plain Javascript object?**
  
**4. What is REST?**
  
**5. Is REST a programming language, framework, technology, or architecture pattern?**
  
**6. What is a Resource in REST?**
  
**7. What is a resource identifier?**
  
**8. What is an HTTP method?**
  
**9. What HTTP methods does REST use within its architecture rules?**
  
**10. Why do we use HTTP methods in REST and how do they relate to resources?**
  
**11. Is REST the same as HTTP?**

## REST API Clients Learning Exercise 🧠
**1. Install Postman in your computer, follow [this](https://learning.postman.com/docs/getting-started/installation-and-updates/) guide**
  
**2. Watch (this)[https://www.youtube.com/watch?v=VywxIQ2ZXw4] course about how to use Postman to interact with APIs**
  
**3. Answer the questions:**
* Postman only works with REST APIs?
* Is there an alternative to Postman?

## Express.JS Core Understanding Learning Exercise 🧠

Read about the Chain of Responsibility design pattern [here](https://refactoring.guru/es/design-patterns/chain-of-responsibility).

**1. Express JS Hello World:**

* Create a new Node.JS project using NPM.
  
* Install Express.JS as an external dependency in your project following [this](https://expressjs.com/es/starter/installing.html) guide.
  
* Create an Express.JS Hello World application following [this](https://expressjs.com/es/starter/hello-world.html) guide.

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

  * Request example
  * Here 3000 indicates a delay of 3000 milliseconds
  http://localhost:3000/api/delay/3000
  Your API should have just one request handler.

You can send any response you want after the delay has expired.

If no delay is provided in the request, the API should use 1000 as default.
