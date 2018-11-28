# Cucumber App
Behaviour-driven development (BDD) extends the Test-Driven Development (TDD) approach by the ‘desired behaviour’ of a software. It is designed to ensure a collaboration between business analysts and developers with explicitly written down scenarios. The basic structure for BDD is:

> **Story**: Returns go to stock

> As a store owner
In order to keep track of stock
I want to add items back to stock when they're returned.

> **Scenario 1**: Refunded items should be returned to stock
Given that a customer previously bought a black sweater from me
And I have three black sweaters in stock.
When they return the black sweater for a refund
Then I should have four black sweaters in stock.

> **Scenario 2**: Replaced items should be returned to stock
Given that a customer previously bought a blue garment from me
And I have two blue garments in stock
And three black garments in stock.
When they return the blue garment for a replacement in black
Then I should have three blue garments in stock
And two black garments in stock.

This project´s goal is to achieve an automated generation of tests from the definitions of the scenarios. 

### Start
To start the frontend and backend application: ``npm start``

### 1. Prototype
The scope of the first prototype is to cover web applications and integrate Github.com as issue tracking tool. The issues from the Github are used to createTherefore the test scenarios will be only cover some basic web application elements. 
The first prototype shall include following elements:
- Button
- Input field
- Radio
- Checkbox
- 'Website'

Demo Prototype: Coming soon ...

### 2. Visualization
## 2.1 Use Case Diagram
![alt text](https://github.com/fr4gstar/Cucumber/blob/master/docs/1.%20Use%20Case.png "Workflow Diagram")

## 2.2 Example: Workflow for viewing and creating a scenario
![alt text](https://github.com/fr4gstar/Cucumber/blob/master/docs/2.%20Workflow.png "Use Case Diagram")

### Additional Features we have in mind for further stages:
- Test Reporting
- Templates Feature
- E2E Test execution (e.g. selenium)
- Additional integration of other project management and issue tracking tool (Jira, Redmine etc.)
- Integration in project mangement and issue tracking tools as a plugin
- Extend the scope to native applications (Java, C# etc.)
- Include additional steps
- Steps editor
- Github authorisation and include own repositories

### Reference Projects
- Cucumber UI: https://github.com/ankur-kushwaha/Cucumber-UI
- Xray for Jira: https://www.getxray.app/
- CukeTest: http://cuketest.com/

### License
Copyright (c) 2018 Adesso AG
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
