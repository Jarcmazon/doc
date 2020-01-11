# Jarcmazon



## Introduction

Jarcmazon is my personal project to build a simple online shop. This isn't just the shop application, this try to cover the whole company with its different areas and interactions. 

I'm not an expert about ecommerce or retail concepts so I will invent my own company structure, departments and interactions. 

With this project I want to put into the scene everything that sounds currently (methodology and technology):

- Architectures & Techniques: microservices, microfrontends, CQRS, EDA, Kafka,...,etc (with theirs patterns, languages, tools, and frameworks)
- CI / CD: methodologies, tools,...,etc...
- Big Data, Real time and Analytics: Kafka, Spark, Cassandra, etc...
- Platforms: Docker, Kubernetes, Openshift, AWS, GCP, Azure, infrastructure as a code, Terraform, Ansible...,etc
- Logging and Monitoring: Prometheus, Grafana, ELK,...,etc



## Jarcmazon

### What is Jarcmazon?

Jarcmazon is just a company selling different products in two different ways:

- **Products stored directly in its own warehouse:** these products are directly bougth to manufacturers and stored into Jarcmazon warehouse, so there is an internal stock and in this case, Jarcmazon is the seller.
- **Products sold by external sellers:** in this case, Jarcmazon is just the application where the final user buys the product but not the final seller. It's just a middleware. There isn't an internal stock but a permanent communication with the different sellers is neccessary in order to offer a good service to the final user. 



### Key points

Jarcmazon offers a platform where users can buy products and manage their orders. **Users** are registered in Jarcmazon so every **communication** with the final user is managed by Jarcmazon. If the product is bought to a provider (second case), Jarcmazon is the middleware between user and provider. 

The same with the **payments**: payments are managed by Jarcmazon. Users do the payment to Jarcmazon and Jarcmazon pays to the final provider (at the end of every month for all the products sold, for instance).

What about **refunds**? Refunds are also managed by Jarcmazon. Users send the product to Jarcmazon and Jarcmazon manages the products returned (and their quality) and return the money to the user. In the case of external seller, Jarcmazon will return the money to the user in advance but after that it will request to the seller the total amount of money of all the products returned by the user in a period of time (a month, for instance).

To Jarcmazon, the **user satisfaction** is so important so quality of sellers is crucial. Sellers have to guarantee a maximum delivery time of five days. If many users complain about a concrete seller and its delivery time, that seller is removed from the platform. The same if a seller has many returns.