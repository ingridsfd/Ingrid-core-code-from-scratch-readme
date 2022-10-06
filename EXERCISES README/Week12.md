# Week challenges (Monday) 💻

Work on your project

# Week challenges (Tuesday) 💻

Work on your project

# Week challenges (Wednesday) 💻

[Age Prediction API](https://github.com/corecodeio/devguide-fundamentals-2022-03/blob/main/src/technologies/2022/week12/exercises/e00/API-3.md) 👶-👴

This is the logic in the index.js file:

![image](https://user-images.githubusercontent.com/98929413/194185620-a61cd234-4962-4bc6-b6bd-7bc45ee7f0e8.png)

Here's the documentation for [req.params.id](https://expressjs.com/en/api.html#req.param)

```JavaScript
const express = require('express'),
    port = 3000,
    app = express(),
    root = "/api/age/"

app.get(root + ':id', (req, res) => {
    const name = req.params.id
    const age = ageRandom()
    const result = {
        name: name,
        age: age,
        days: ageDays(age)
    }
    res.send(result)
})

app.get(root, (req, res) => {
    res.send({ error: `Missing parameter 'name' was expected.` })
})

const ageRandom = () => {
    return Math.floor((Math.random() * 98) + 1)
}

const ageDays = (age) => {
    return Math.floor(age * 365)
}

app.listen(port, () => {
    console.log(`Listening on port: ${port}`)
});
```

Here's the testing in Postman:

![image](https://user-images.githubusercontent.com/98929413/194185732-592e7b9f-8b9e-47b1-987d-a95a9297bfa6.png)


[NSA Secrets Box API - Hacking Challenge](https://github.com/corecodeio/devguide-fundamentals-2022-03/blob/main/src/technologies/2022/week12/exercises/e01/API-4.md) 👨‍💻

# Week challenges (Thursday) 💻

Work on your project
