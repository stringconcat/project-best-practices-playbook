Deal with complexity
====================
Tools and technics
------------------
Cleal architecture
Domain-Driven Design or Lightweight DDD. 

Tools and technics in detail
----------------------------
### Domain-Driven Design
#### How to use it and what it is.
Most of the classes in domain module represent creatures or notions from the real world. Close collaboration with Domain experts and BA.
The majority of methods represent actual business operations.
#### When to apply 
When the domain is really complex.  
#### Benefits
Requirements and intentions will be understandable from code even 5 years from now.
Maintainability is high, cause it is obvious what is happening in the code.
 
### Lightweight DDD
#### How to use it and what it is.
Basically just a good Object-Oriented Design. Use ValueObjects instead of primitive types and it will reduce complexity dramatically. 
#### When to apply 
When the domain is not complex
#### Benefits
Instead of having many screens of code in the Service layer or in  UseCases u will have many maintainable tiny classes each of them testable independently

### Clean Architecture
#### How to use it and what it is.
It is a clear and unambiguously interpreted seat of rules for structuring code. 
#### When to apply
It is a sensible default for any service. The exception is service without business logic at all, such as BFF. But be careful: every service looks like candy at the beginning but the domain complexity will hit you in a couple of months
#### Benefits
A good foundation for Domain-Driven design or lightweight DDD.
Separate infrastructure from core domain quite well. 
Highly testable solution
