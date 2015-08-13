---
layout: post
title: "Spring Data - Book Review"
description: "Spring Data book review"
modified: 2014-03-16 01:00:41 +0100
tags: [CRUD,JPA,Spring,Spring Data,QueryDSL]
categories: [blog]
image:
  feature: 
  credit: 
  creditlink: 
comments: true
share: true
---

Spring Data is a Spring sub project trying to simplify the implementation of data access layer in Spring applications. The Spring Data JPA sub module simplifies the implementation of a generic CRUD repository. It provides a generic interface which is then implemented using proxies. It eliminates the repetitive boiler plate code required for performing CRUD operations. Other sub modules simplify the implementation of noSQL data stores like redis or mongo.

There is a comprehensive reference documentation for Spring Data but for people who are new to spring or not very experienced with spring it can be a bit difficult. The book [Spring Data](http://www.packtpub.com/spring-data/book) from Packt Publishing can be a good start in programming of the data access layer using the Spring Data. The book focuses on the JPA and redis sub projects.

The first chapters introduces the concepts of Spring Data and Spring Redis. There are also covered the advantages of using frameworks like JPA or Redis. They explain how to setup a basic web application to use the Spring Data framework. 

The second chapter gives the reader receipes how to setup the project using the programmatic configuration, the techniques of how to configurea web application and explains the design patterns like the builder to build a new object. The chapter contrasts the traditional way of how to implement the data access layer with the advantages offered by Spring Data. The chapter shows the boiler plate code required to implement the data access using the traditional way and how that can be abstracted by implementing of a generic repository. This shows how Spring Data is able to generate the complete implementation using only an interface.

The next chapter explores several strategies available to build queries with Spring Data and explains the advantages and disadvantages of each option. It covers all the main approaches for building static and dynamic queries:

* JPA Criteria API
* convention based method name
* named query
* query annotation
* Query DSL

There is also a complete example application that is built from ground up. For each strategy there are samples for queries using JPQL and Standard SQL providing the reader a good hold on how to use this for building a real application. This chapter includes also sections on sorting and pagination.

The fourth chapter explains how to refactor the application by adding custom functionality to the repository to keep the architecture of the application clean.

The last chapters explain the design principles of a Redis data model and the key components of Spring Data Redis - template and serializers. They discuss how the CRUD application can be implemented using this sub module end explain and different storage approaches, e.g. using JSON with a string serializer to store objects as strings in JSON format. The sample contact applications is now implemented using the Redis framework. The last chapter explains also how can we use Spring Data Redis to implement the publish/subscribe messaging pattern and how it can be used as an implementation of the cache abstraction provided by Spring Framework 3.1.

This is a very simple book with simple examples. The samples are built form scratch and all the steps are clearly explained in form of tutorial (step by step). I've never been using Spring Data before. I was provided a copy of this book to make this review and it took me a few hours to read and understand the basic concepts of Spring Data. This book is compact and gives the basic knowledge of Spring Data. It can be used as a quick start into this technology. In my opinion a big advantage of this book are links to resources with more detailed material about each discussed topic. This can be especially very useful for Spring beginners.
