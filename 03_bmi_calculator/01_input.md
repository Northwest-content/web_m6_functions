So now we reached the level that we want to get inputs from the user from the website itself rather then using `prompt`, this is the project: ![img](https://lh3.googleusercontent.com/WUsm6ydMrM6Vd8TkVvUirkhngMV-L8nzWzPcaEFcJeTQwKCdUFFaUBrZx5LOLq0oDdvpqcLHu3toySuE188yyvTRqQXQMlh_mcx8XVMoR84C0IPnqVy2K8RpPe0pGUPshi6QrixD)BMI calculators only takes from the user his/her height and weight, then tells them if they are: 

- Underweight
- Normal
- Overweight
- Obese
- Extremly obese

Using this equation:

![img](https://lh3.googleusercontent.com/wAFwMMfJAXlj6xs9DHyuMhRwybflGhTFnTVFKu4wpax07r99HAvOKKfgshO7-jsiqrqkYQn0I1YMsXx7_5vJXtPYqa8U5jZ5_wgZn_-IvUOa_4YlMojTGDHcohS1bE-lUTpoaw1X)

Based on this image, we will know what to say to the user:![img](https://lh3.googleusercontent.com/ZK96UhvBmGpVpPaVvV0du8-6dQ7dO6UEdbuXG77QbuYC6jTEyvUKIJG_sdyS0KIjbG9O3NqpHrIFOsG9FJ_zUI4UvudG9G6RsRKzlM-PMlo-6DcMTD5hlZtxSb0c00lSxxmsxOXU)Now lets learn 🔥😎

As you see having prompt is nice, but might annoy the user 😅. How about changing the way that we take our input? `HTML` is here to the rescue with an `<input>`.

The `<input>` tag has a friend called `<label>`

To look like:

````html
<label> Enter value</label>
<input>

````

In our calculator this is our `HTML`: 

````html
<body class="container">
    <h1>BMI Calculator</h1>
    <div>
        <label>Enter Height</label>
        <input>
    </div>
    <div>
        <label>Enter Weight</label>
        <input>
    </div>

    <div class="button" id="submit">Get Result</div>

    <div>
        <p>Result: </p>
        <p id="result"></p>
    </div>
</body>
````

Now we will add our `script.js` and start playing 🔥