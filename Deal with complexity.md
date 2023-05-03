Deal with complexity
====================


Tools and technics
------------------
Cleal architecture 

Domain-Driven Design or Lightweight DDD 

Tools and technics in detail
----------------------------
### Domain-Driven Design
#### How to use it and what it is.
Most of the classes in domain module represent creatures or notions from the real world. 

Dev team works closely with Domain experts or Business Analyst (if they represent domain Experts).

The majority of methods represent actual business operations.
`vessel.dischargeCargoFrom(bay)` intead of `vessel.remove(bay)`

#### When to apply 
When the domain is really complex.  

#### Benefits
Requirements and intentions will be understandable from code even 5 years from now.
Maintainability is high, cause it is obvious what is happening in the code.

#### Find more
[Book: Learning Domain-Driven Design: Aligning Software Architecture and Business Strategy](https://www.amazon.sg/Learning-Domain-Driven-Design-Aligning-Architecture/dp/1098100131/)
 
### Lightweight DDD
#### How to use it and what it is.
Basically just a good Object-Oriented Design. Use ValueObjects instead of primitive types and it will reduce complexity dramatically. 

#### When to apply 
When the domain is not so complex or dev team does not have access to Domain Experts

#### Benefits
Instead of having many screens of code in the Service layer or in  UseCases u will have many maintainable tiny classes each of them testable independently

### Clean Architecture
#### How to use it and what it is.
It is a clear and unambiguously interpreted set of rules for structuring code. 
#### When to apply
It is a sensible default for any service. The exception is service without business logic at all, such as BFF. But be careful: every service looks like candy at the beginning but the domain complexity will hit you in a couple of months
#### Benefits
A good foundation for Domain-Driven design or lightweight DDD.
Separate infrastructure from core domain quite well. 
Highly testable solution
#### Find more
[Book: Clean Architecture: A Craftsman's Guide to Software Structure and Design](https://www.amazon.sg/Clean-Architecture-Craftsmans-Software-Structure/dp/0134494164)
