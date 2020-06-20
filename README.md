# cypress_setup
#### Reference script: https://example.cypress.io/commands/actions

1.	What is the purpose to use  this tool?
	A rich yet simple API for interactions with automatic waiting
	Mocha, Chai, and Sinon bundled in
	A sleek dashboard with automatic reloads for Test-Driven Development
	Easy debugging
	Network traffic control for validation and mocking
	Automatic screenshots and videos
	Most testing tools operate by running outside of the browser and executing remote commands across the network. Cypress is the exact opposite. Cypress is executed in the same run loop as your application.
	Cypress runs much, much faster in comparison with the end to end tools by Selenium that we have experimented.
2.	Why this is better than other tool?
Ans: 	Most testing tools operate by running outside of the browser and executing remote commands across the network. Cypress is the exact opposite. Cypress is executed in the same run loop as your application.
3.	Why you're using this tool?
Ans: Same as 2
4. Usability:
a. Normal scripting using page object and with different browsers. and platform e.g Windows, MAC, Mobile
Page Object: It supports “Application Actions” which is similar to page object.
https://www.cypress.io/blog/2019/01/03/stop-using-page-objects-and-start-using-app-actions/
Only support Cypress’s customize Chrome browser(version could be older)
Works on Win and MAC machine. Doesn’t support mobile app.
b. Parallel execution.
While you're working in the browser - no.
When running headlessly - yes.
Cypress can run each individual file in parallel.
c. Datadriven with Assertion using csv or xlsx
Cypress has Fixture to load data with JSON format.
https://docs.cypress.io/api/commands/fixture.html#Syntax
d. Jenkins build or execution in Docker  Ans: Yes
e. Result Report
Ans: Cypress is built on top of Mocha, that means any reporter built for Mocha can be used with Cypress.
f. Advantages and drawback
1. Cypress support their customize Chrome browser(version could be older) so this may not be the good tool for testing, except for Unit testing.
2. It doesn’t support cross browser testing.
3. The structure was different to the other Selenium end to end tools, so at first you may need to spend more time understanding the structure and finding the best way to create your scripts.
4. Community: As Cypress is relatively new, the community is small. You will have trouble finding answers to problems etc.
5. Features. No file upload support. No cross-browsers testing. Who knows when these things will be covered, as for big projects these features are crucial.
6. Page Object Model. It is something that has already been proven by time. Cypress supports a different approach which could be controversial. More detail on this is here: Cypress POM
7. It's only available for only one client (language) i.e for JavaScript only. So to work with it you must know JavaScript: however this might be an advantage for JavaScript application, but I would like to put it as a disadvantages for those who have difficulties with javascript.

To setup Cypress:
Open VS code.
npm init -y
npm install cypress --save-dev
add this in package.json
    "scripts": {
      "test": "cypress open"
    }
npm bin (to get bin directory)
C:\Users\ahoss1\Desktop\doAutomate\cypresstest\node_modules\.bin> npm run test
Useful link:
https://dzone.com/articles/why-should-you-switch-to-cypress-for-modern-web-te

https://www.youtube.com/watch?v=l_Q7cbmYjDY
