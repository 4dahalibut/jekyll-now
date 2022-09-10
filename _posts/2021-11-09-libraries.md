---
layout: post
title: Building Software Libraries
---
* No service owner understands every package in their software.
* If there is a bug in your library, noticing the regression will be delayed after the release, as you don't notice until somebody uses that release. 
* Keep fewer codepaths (cyclomatic complexity)
* think about what other software might be running on service. 
* You can explicitly version within package names to prevent against breaking changes, if you want to be super careful. 
* Clients shouldn’t need to write boilerplate to use your library
* Libraries should be self-documenting - especially by throwing checked exceptions on edge cases.
* As a library owner, you have to be aware of any assumptions you're making about the outside world. 
* Once you release a library, you really don’t want to need to touch it, because you may break people. 
* This means that you have to do a really good job at requirements gathering, and then don’t touch code unless it NEEDS to be touched. 
* Be paranoid about changes to your package. 
* Test your code with actual customers before releasing it publicly. 
* You want to depend on as few packages as possible as a library, this makes it way easier to consume. 
* Be cognizant about the logs and exceptions you spew, definitely log and except, but not too much.
* Link to wikis inside of exception messages. However, wikis can get out of date. 
* Libraries should be: (Reliable, Intuitive, Secure, Efficient, Maintainable, Universal, Debuggable)
* It is possible to create a service that is interacted with as a library, which is beneficial in some situations
		

- notes gleaned from a talk by Rob Atlas
