# node-express-lambda

A minimal [Express](https://expressjs.com/) API with a single function that calculates 
an [approximation to pi](https://www.google.com/search?q=calculate+pi+monte+carlo&oq=calculate+pi+monte+carlo&aqs=chrome.0.0l6.4335j0j7&sourceid=chrome&ie=UTF-8#kpvalbx=0) wrapped as an AWS lambda and deployed with serverless.

To run this, you'll need an AWS account and the CLI installed and configured 
with an access key. 
In addition, you'll need the [serverless framework](https://serverless.com/) and [npm](https://www.npmjs.com/) installed. 

Then follow these steps,

Clone the repository

````
git clone 
````

Deploy to AWS

````
sls deploy
````

When the deployment is complete, serveless will provide you the endpoint and API key.

You can execute the resulting lambda by sending a GET to the endpoint, passing an x-api-key header.
There is one optional parameter ?count that defines how many iterations of the Monte Carlo
simulation to run (default is 10000).