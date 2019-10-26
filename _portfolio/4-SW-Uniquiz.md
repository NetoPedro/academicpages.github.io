---
title: "Uniquiz"
excerpt: "Social Network for Portuguese students and teachers <br/>"
topic: "Software Engineering"
collection: portfolio
---


Uniquiz is a social network that has as main goal the approximation between students and professors and the improvement of student grades. The idea is to be a fully featured study platform in which the students will be able to rely on. 


[Uq1](https://raw.githubusercontent.com/NetoPedro/netopedro.github.io/master/images/uq1.jpg)
[Uq2](https://raw.githubusercontent.com/NetoPedro/netopedro.github.io/master/images/uq2.jpg)
[Uq3](https://raw.githubusercontent.com/NetoPedro/netopedro.github.io/master/images/uq3.jpg)

To implement, a microservices approach was used. The current implementation has 7 Go microservices, each one dealing with their specific database. The databases engines in use are 2 MySQL, 1 Neo4J, 2 Redis, 2 MongoDB, and 1 RethinkDB. 
To power up search use cases an ElasticSearch instance was used. 

In terms of the gateway, the implementation used the Spring Cloud Netflix stack to ensure functionalities like Load Balancing. 

The frontend application was developed in AngularJS. 

The development process had several environments coordinated through a Jenkins instance and the deployment was made in containers. 

Since this started as a project for the internship, the report can be accessed through ISEP's archives. There the implementation and architecture are fully detailed. 

