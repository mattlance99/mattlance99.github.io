---
layout: post
title:      "Continuous integration, continuous delivery and continuous deployment"
date:       2019-06-17 20:54:06 +0000
permalink:  continuous_integration_continuous_delivery_and_continuous_deployment
---


Continuous integration, continuous delivery and continuous deployment. 

Working in a an agile environment you might hear terms like continuous integration, continuous delivery and continuous deployment. 
Believe it or not there’s lots of confusion concerning the distinction between these three terms. More surprising is that the interpretations are not always consistent even between Developers of the same company.  Lets define the terms.

Continuous integration is a method that allows Developers to merge their commits into the main branch without being concerned about OTHER Developers commits. Developers are encouraged to make small commits and make commits often. The commits are tested immediately by creating a build with the changes and running against a suite of automated tests. If the build fails the commits need to be reverted and resolved. 

Assuming you have continuous integration set up the next logical step is continuous delivery. Continuous delivery involves two main components. The first component is confidence in your post build test automation. Passing your post build automated test suite means that the build is solid enough to be deployed to the public. The goal here is that ANY build you select (after running the automation) can be released to the public. 
The second component is that you have an automated release (or semi-automated) release process in which you can easily deploy the build you choose at any time. 

Continuous deployment is more or less a combination of the two and then some. It means that as a developer you can make a commit and that commit is immediately deployed to the public, assuming that it passes all of your automation. The only thing stopping a change from being deployed is a test that fails. This type of environment is ideal for making quick changes readily available to customers. Its the fastest way to fix bugs, add new product features and make enhancements. 

The principles themselves encourage good practices. Smaller and more frequent commits generally mean less regressions introduced. Deploying changes quickly allows customers to see enhancements or bug fixes immediately. Most importantly Developers develop without fear of breaking anything major. 
