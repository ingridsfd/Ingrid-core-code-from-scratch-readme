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

# Week challenges (Thursday) 💻

Work on your project
