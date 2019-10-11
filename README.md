# Seed-Test
Behaviour-driven development (BDD) extends the Test-Driven Development (TDD) approach by the ‘desired behaviour’ of a software. It is designed to ensure a collaboration between business analysts and developers with explicitly written down scenarios.

*   Check out the [Tutorial](https://github.com/adessoCucumber/Cucumber/wiki/Tutorial)


## What is Seed-Test?
Seed-Test is a website user interface testing tool, which uses approaches of behaviour-driven development and the notation of Gherkin to enable developers and business users to execute automated tests for their website. It can be tested on the official [website](https://cucumber-app.herokuapp.com/).

We are greateful for any testing and feedback, so please help us by filling out this [feedback form](https://cucumber-app.herokuapp.com/feedback)

## Bugs, Problems ...
Please contact us via mail seed-test@adesso.de

## Installation
To install and use the application localy, clone the repository.
It is necessary to install [NodeJS](https://nodejs.org/en/).
Install Angular 7:
```
npm install -g @angular/cli 
```
Then install all necessary node modules:
```
npm install
```

For the frontend server, remember to change the link to the backend server in the api-service.ts file.
To run the frontend server switch to the frontend folder and use this command:
```
cd frontend
ng serve
```
To run the backend server switch to the backend folder and use this command:
```
cd backend
npm start
```

CAUTION: Currently the our test database is connected so if you want to use your own database more info will be provided soon.




### License

Copyright (c) 2018 Adesso AG Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
