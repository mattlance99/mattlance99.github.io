---
layout: post
title:      "Testing Your Frontend Using Cypress.io"
date:       2019-06-24 00:55:40 +0000
permalink:  testing_your_frontend_using_cypress_io
---


Earlier last week I had the pleasure of speaking to a Developer about writing tests. More specifically I asked him if he practiced Test Driven Development, the practice of initially writing an automated test that fails, followed by writing some code that fixes the failure. The Developer refactors to make the code more efficient and then you repeat the cycle.  He stated that generally he does’t write tests because it takes too long. This is a very common answer. 

Last week I was introduced to Cypress.io,  an End-to-End testing framework that allows you to easily create front-end and UI tests.  The tests you design mimic the behavior of a web application user. Cypress.io is fairly new and looks to be the next big tool in Testing, perhaps overtaking Selenium(the standard front end testing tool). Cypress.io should eliminate any excuses for not writing tests. Getting up and running doesn’t take long. 

When reviewing the instructions I immediately get excited, the commands start off exactly like the commands I used when I first started learning React/Redux. 

npm install cypress 

OK good. The install begins and as I’m waiting I start to read the documentation. I’m seeing some cool features. Cypress takes screenshots of each step of your test cases and captures various states of the product. This makes debugging easy. You can see exactly what the UI looked like at the time of any failures.  

Next (how familiar)….npx cypress open. The product launches, and it has an intuitive layout. The UI is divided vertically down the middle, split into two screens. The left side will show the results of the tests, the right side displays the actual web page you are testing. Its an actual chrome version of the site. 
Open up your favorite text editor to where Cypress is installed. On the left of you text editor you can see your tree structure. Create a new file “my_test.js” under examples(below ‘integration’). 

Enter the following text:

describe("Verifies you can visit www.espn.com", function() {
  it("visits espn website", function() {
    cy.visit("https://www.espn.com");
  });
});

Save the file. The test inside Cypress.io immediately kicks off. You can actually see the ESPN website on the right side of the UI. The test on the left runs, you should see a passing test. You just successfully tested whether or not you can visit ESPN.com. Congratulations!

After learning only a few commands, I started to put together the building blocks of a test suite. On Day One. 
The value in Cypress.io is obvious. If anything running the product as you develop can easily spot regressions, and correctly fail during Test Driven Development. I look forward to becoming an expert in this testing tool, it will be an excellent investment in time. 
