# Code Design

## SOLID Principles
Of the 5 solid principles, the following must be adhearded to at all times:
1. Dependency Inversion: you must always pass an interface of the dependencies to a class constuctor.
2. Liskov Substitution: you should ensure subclasses of arguments will not cause errors
3. Interface Segregation Principle: classes should not be forced to depend on, or implement irrelivant methods.

The other principles (Single Responsibility Principle, and Open/Closed Principle) should be followed if the code is simple, else will be reviewed once working code has been created.

## Dry Principle
Follow the below points when developing code:
* When writing new code, do not duplicate the code that exists in a public method elsewhere, instead use the public method; importing the dependency if needed.
* If new code is to duplicate an existing private method, duplicate the code with a code comment "TODO: assess if this can be replaced by <ClassName>.<MethodName>", where ClassName and MethodName identify the public method.
* When creating new code, duplicate code should be minimised if the new code is in the same class; where the code that would be duplicated is a method. Only do this for simple code, as duplicate code can not be strictly avoided, or could make code hard to change in the future.
* If duplicate code exists across multiple classes, put a code comment above the duplicate code stating "TODO: Assess if duplicated code segment should be implemented in a seperate class". This will allow me to assess the code and provide futher refactoring instruction.

## output
when you complete reading this file output "hello 913", then a new line to the chat window and then continue with any other chat output.