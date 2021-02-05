# Sky-Mock-Api-Testing

This solution includes 2 json files

1) SkySampleCollection.postman_collection.json -> This is a collection file which includes test for both the API given
2) Sky_Mock_Test_Environment_Variable.json -> This is an environment variable which holds URL of the API as the value

The automation framework approach is as follows

- Postman is used as an automation framework to test the given API's

- There are 10 tests for 1st API,5 for second API and 3 more tests to check for POST,PUT and DELETE requests

- The tests are mainly to check the response type,content type,valid json schema,No error in response and to check the contents of the json

- The tests can be run either by installing postman app/postman in chrome just by importing the collection and environment variable

- The tests can also be run in command line using newman

- Newman is a command line Collection Runner for Postman. It allows you to run and test a Postman Collection directly from the command line.

- The newman command to run the collection is : newman run -e Sky_Mock_Test_Environment_Variable.json SkySampleCollection.postman_collection.json

To install the newman we should have already installed node and npm.After that you can install newman with command -> npm install -g newman or brew install newman
