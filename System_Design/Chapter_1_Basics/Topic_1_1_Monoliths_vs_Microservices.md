# Chapter 1 : Basics

## 1.1 Monoliths vs Microservices

<br>

### *Should you choose Monoliths or Microservices ?*

<br>

### **Monolith**

#### Advantages:
1. Small team size
1. Deployments are easy
1. Less duplication
1. Calling different service is faster as the code lies in the same machine

#### Disadvantages:
1. New hires, need to understand whole context of the system.
1. Deployments are complicated. Any change in code requires deployment.
1. Single point of failure.

<br>

### **Microservices**

#### Advantages:
1. Easier to scale, design
1. New developers can understand easily as they dont need to understand the whole system. You can assign a single microservice to them first.
1. Parallel development is easy
1. Greater visibility to understand which service is used more and can be scaled accordingly.
1. Needs a smart archietect to design well.
1. It is best to be used for large system.

<br>

### *How do you decide whether a service should be a separate microservice or not ?*

<br>

A good rule is to see whether the service is calling only one other service or not. If yes, then don't separate it out. Else create it into separate microservice.

For eg.

If you have service 1 calling only service 2, then package both of them into single service.

