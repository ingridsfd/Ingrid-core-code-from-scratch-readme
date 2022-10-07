# Week challenges (Monday) 💻

Work on your project

# Week challenges (Tuesday) 💻

Work on your project

# Week challenges (Wednesday) 💻

[Age Prediction API](https://github.com/corecodeio/devguide-fundamentals-2022-03/blob/main/src/technologies/2022/week12/exercises/e00/API-3.md) 👶-👴

This is the logic in the index.js file:

![image](https://user-images.githubusercontent.com/98929413/194202208-b79c027f-cbee-40eb-95a2-2576f26d6570.png)

Here's the documentation for [req.params.id](https://expressjs.com/en/api.html#req.param)

[Documentation #2](https://stackabuse.com/get-query-strings-and-parameters-in-express-js/)

```JavaScript
import express from 'express';
import bodyParser from 'body-parser';
	
var app = express();
var app_port = 3000;
app.use(bodyParser.urlencoded({ extended: false }));

app.use(bodyParser.json());

app.listen(app_port, function(){
	console.log('Server is running on port ' + app_port);
});

app.get('/', function (req, res) {
	const name = req.query.name;
	const edad = randomAge();
	const days = convertDays(edad);
	const result = {
		name: `${name}`,
		edad: `${edad}`,
		days: `${days}`
	};
	res.send(result);
});

const randomAge = () => { 
	return Math.floor((Math.random() * 98) + 1);
};

const convertDays = (edad) => {
	return edad * 365;
};
```

Here's the testing in Postman:

![image](https://user-images.githubusercontent.com/98929413/194202407-1f349c17-5213-448f-93d9-72ccf3b410af.png)


[NSA Secrets Box API - Hacking Challenge](https://github.com/corecodeio/devguide-fundamentals-2022-03/blob/main/src/technologies/2022/week12/exercises/e01/API-4.md) 👨‍💻

In this exercise we started by understanding the JavaScript type coercion:

This is the general view of the repo cloned:

![SBA0](https://user-images.githubusercontent.com/98929413/194485820-7123850c-fedb-4fa6-8909-7dba9a848235.gif)

We notice that takes a parameter "role" through a request body inside the API.

Then, it has two other JavaScript files linked to it:

![SBA0 1](https://user-images.githubusercontent.com/98929413/194486188-01e49267-617a-420f-8ae8-73c9061537bd.gif)

Here we see that the language of JavaScript starts interpreting the type coercion for the conditionals described. Where if roles it's not true, it will move to compare to the content of boolean 'role'. JavaScript will start comparing them to the values which are numbers, but according to the documentation, if JS if there are primitive values, in the end, it'll see them as bigger, lesser or equal to the number value types. Therefore, it will say they are false and return true to a string.

So, when testing in the Postman app. We first run in the terminal:

![SBA1](https://user-images.githubusercontent.com/98929413/194487102-7ee34284-db77-4781-b277-41eb970e7056.gif)

And then the host is running in port 8080, we test in Postman. 

![SBA2](https://user-images.githubusercontent.com/98929413/194487257-6a92068e-b189-4798-8126-28dd177e8906.gif)

So we remember that is a modification in the 'Body' with the method GET, and we add the primitive value to string.

We hit send:

![SBA3 0](https://user-images.githubusercontent.com/98929413/194487420-c1a0e068-d70f-4319-a1f7-550b2ea701c4.gif)

And finally, we obtain the data we were looking for:

![SBA3](https://user-images.githubusercontent.com/98929413/194487469-a2e3756d-ba4d-4043-bd93-df1d679ee20e.gif)

...and, we're in:



# Week challenges (Thursday) 💻

Work on your project
