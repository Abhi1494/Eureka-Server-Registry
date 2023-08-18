===========steps to create eureka server============

1. create the spring project and add these below dependency

    a. add the netflix eureka server dependency
    b. add spring cloud bootstrap dependency to enable the cloud features

2. Add @EnableEurekaServer annotations in main class(e.g: EurekaRegisteryApplication)

3. Add these below properties in application.properties which will disabled the project to be not the register as client in eureka server
    eureka.client.register-with-eureka = false
    eureka.client.fetch-registry = false
4. register the another microservice as client in eureka server.