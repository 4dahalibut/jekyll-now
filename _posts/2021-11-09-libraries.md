---
layout: post
title: Building Software Libraries
---
* You can’t understand every package which is in your service
* Consumable environments act as services but are used as libraries. (amazon specific thing here)
* library breakages cause delay between release and regression, as you don't notice until somebody uses it later? 
* keep fewer codepaths (cyclomatic complexity)
* think about what other software might be running on service
* You can explicitly version library versions to prevent against breaking changes, where customers use a version of the library explicitly and have to explicitly update that version to get any new breaking changes. 
* Client’s shouldn’t need to write boilerplate to use your library
* libraries should be self-documenting - especially by throwing checked exceptions on edge cases
* As a library owner, you have to be aware of any assumptions youre making about the outside world. 
* Once you release a libary, you really don’t want to need to touch it, because you may break people
* This means that you have to do a really good job at requirement gathering, and then don’t touch code unless it NEEDS to be touched. 
* Be paranoid about changes to your package. 
* Test your code with actual customers before releasing it publicly. 
* You want to depend on as few packages as possible as a library, this makes it way easier to consume. 
* Be cognizant about the logs and exceptions you spew, definitely log and except, but not too much
* Link to wikis inside of exception messages. However wikis can get out of date
* Libraries should be: 
		* Reliable
		* Intuitive
		* Secure
		* Efficient
		* Maintainable
		* Universal 
		* Debuggable
		
- notes gleaned from a talk by Rob Atlas
