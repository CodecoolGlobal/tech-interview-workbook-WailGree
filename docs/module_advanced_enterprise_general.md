# General enterprise questions

## Software engineering

### Architectures

#### What is n-tier (or multi-tier) architecture?
In multi-tier architecture software is engineered to have processing, data management and presentation functions physically and logically separated.
This means that the different functions are hosted on several machines or clusters.
N-tier architecture is separated in three different tiers:
1. Logic tier
2. Presentation tier
3. Data tier
  
#### What are microservices? Advantages and disadvantages?
Microservices are a way of breaking large software projects into loosely coupled modules, which communicate with each other through simple Application Programming Interfaces (APIs).
Advantages of microservice:
1. Smaller and faster developments
2. Scalability
3. Ease of understanding 
4. Improved fault isolation
5. Eliminate vendor or technology lock-in 

Disadvantages of microservices:
1. Communication between services is complex
2. More services equal more resources	
3. Global testing difficulty	
4. Debugging problems can be harder	
   
#### What is Separation of Concerns?
*Separation of concerns is a software architecture principle for separating an application in distinct sections, so each section addresses a separate concern. The overall goal of SoC is to establish a well-organized system where each part fulfils a meaningful and intuitive role while maximizing its ability to adapt to change.*

#### What is a layered design and why is it important in enterprise applications?
Layered architecture are n-tiered patterns where the components are organized in horizontal layers. This is the traditional method for designing most software and is meant to be self-independent. All components are interconnected but not dependent on each other.
Layered architecture has 4 layers

1.	Presentation layer – contains all categories related to the presentation layer
2.	Business layer – business logic
3.	Persistence layer – used for function like object-relational mapping
4.	Database layer – where all data is stored

Using a layered design for an enterprise application has a series of benefits, such as easy to test as components because are separated on different layers and easy to implement.

#### What is Dependency Injection?
Dependency Injection (DI) is a design pattern used to implement IoC. It allows the creation of dependent objects outside of a class and provides those objects to a class through different ways. Using DI, we move the creation and binding of the dependent objects outside of the class that depends on them. 

The Dependency Injection pattern involves 3 types of classes. 

1.	Client Class: The client class (dependent class) is a class which depends on the service class 
2.	Service Class: The service class (dependency) is a class that provides service to the client class. 
3.	Injector Class: The injector class injects the service class object into the client class. 

#### What is the DAO pattern? When and how to implement?
The Data Access Object (DAO) pattern is a structural pattern that allows us to isolate the application/business layer from the persistence layer (usually a relational database, but it could be any other persistence mechanism) using an abstract API.

The functionality of this API is to hide from the application all the complexities involved in performing CRUD operations in the underlying storage mechanism. This permits both layers to evolve separately without knowing anything about each other.

#### What is SOA? When to use?
Service-Oriented Architecture (SOA) is a style of software design where services are provided to the other components by application components, through a communication protocol over a network.

The primary motivator for companies to switch to an SOA is the ability to reuse code for different applications. By reusing code that already exists within a service, enterprises can significantly reduce the time that is spent during the development process.

### Testing
#### What are unit test, integration test, system test, regression test, acceptance test? What is the major difference between these?
#### What is code coverage? Why is it used? How you can measure?
#### What does mocking mean? How would you do it 'manually' (i. e. without using any fancy framework)?
#### What is a test case? What is an assertion? Give examples!
#### What is TDD? What are the benefits?
#### What are the unit testing best practices? (Eg. how many assertion should a test case contain?)
#### What is arrange/act/assert pattern?

### DevOps
#### What is continuous integration? Why is CI important?
#### Why are tests important in the CI workflow?
#### Name some software that help the CI workflow!
#### What is Continuous Delivery?
#### What is Continuous Deployment?
#### What is DevOps?

### Software Methodologies
#### What kind of software-lifecycle models do you know?
#### What is a UML diagram? What kind of diagram types do you know?
#### What is a UML class diagram? What are the typical elements?
#### What kind of design patterns do you know? Bring at least 3 examples.
#### What is the purpose of the Iterator Pattern?
#### What do you know about the SOLID principles?
#### How would you separate data storage code and business logic code (which uses stored data) in an application?

## Computer science

### Data Structures
#### What is the difference between Stack and Queue data structure?
#### What is a graph? What are simple graphs? What are directed graphs? What are weighted graphs?
#### What are trees? What are binary trees? What are binary search trees?
#### How can you store graphs in programs? What are the advantages/disadvantages per each?
#### What are graph traversal algorithms? What is BFS, how does it work? What is DFS, how does it work?
#### How does dictionary work?
#### Why is it important for keys in a hashmap to have an immutable type? (Consider string for example.)

### Algorithms
#### What is QuickSort? Describe the main logic of this sorting algorithm.

## Software design

### Security

#### What is OAuth2?
#### What is Basic Authentication?
#### What is CORS, why it’s needed in browsers?
#### How can you initialize a CSRF attack?
#### What is JWT used for? Where to store it on client side?

### Threaded programming

#### When do you need to use threads in an application?
#### What is a daemon thread?
#### What is the difference between concurrent and parallel execution of code?
#### What is the most important problem developers are faced when using threads?
#### In what kind of situations can deadlocks occur?
#### What are possible ways to prevent deadlocks from occurring?
#### What does critical section or critical region mean in the context of concurrent programming?
