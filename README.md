# IBLIS-APPSYNC

_**Test and develop locally AWS AppSync with DynamoDB using Serveless Framework.**_

Repository for this medium article: [Serverless GraphQL with AWS AppSync and DynamoDB](https://medium.com/@vdelacou/serverless-graphql-with-aws-appsync-and-dynamodb-3dcbe29f026e)

Please read the article if you have any questions

## Why

The purpose is to automatize the deployment of all the resources needed to create the GraphQL API. Also for development it's more convenient to keep track of the change in a git repository. All of this is not possible by using only the AWS AppSync dashboard UI. Also it takes a lot of time to change all the resolvers one by one. Serverless Framework can help us to deploy the DynamoDB and the AWS AppSync server and upload all the resolvers.


## Features

* GraphQL API with one mutation to add an object and one query to see all objects
* GraphQL API with API_KEY security
* Automatic deployement and setup of DynamoDB
* Works totally offline, no need to deploy if you do not want to

## Library and Tools

* [Serverless](https://serverless.com/) To help us deploying our API
* [serverless Appsync Plugin](https://github.com/sid88in/serverless-appsync-plugin) To deploy, update or delete the AWS AppSync API's with ease.
* [Altair GraphQL Client](https://chrome.google.com/webstore/detail/altair-graphql-client/flnheeellpciglgpaodhkhmapeljopja) Chrome extension GraphQL client to test the API
* [Serverless Offline](https://github.com/dherault/serverless-offline) For using serveless offline
* [Serverless DynamoDB Local](https://github.com/99xt/serverless-dynamodb-local) For install in your machine DynamoDB
* [Serverless AppSync Offline](https://github.com/aheissenberger/serverless-appsync-offline) For exposing the GraphQL API with AppSync Offline


## Deploy

Install and follow [instructions](https://serverless.com/framework/docs/providers/aws/guide/installation/) to setup serverless with AWS

`npm install`

`serverless deploy`

## Test locally

`serverless dynamodb install --localPath ./bin`

`serverless offline start`


## Contribute

1.  [Fork](https://help.github.com/articles/fork-a-repo/) this repository to your own GitHub account and then [clone](https://help.github.com/articles/cloning-a-repository/) it to your local device
2.  Make the necessary changes and ensure that the tests are passing
3.  Send a pull request


## Known issues

* None for the moment


## License

Please, refer to LICENSE file
